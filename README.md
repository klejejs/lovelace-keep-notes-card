# keep-notes-card
A Lovelace custom card for [custom component Keep Notes sensor](https://github.com/klejejs/ha_keep_notes_sensor) in Home Assistant.

For installation see [this guide](https://github.com/thomasloven/hass-config/wiki/Lovelace-Plugins).


**This card requires [card tools](https://github.com/thomasloven/lovelace-card-tools).**



## Example configuration



```yaml
title: My awesome Lovelace config
resources:
  - url: /local/keep-notes-card.js
    type: js
views:
  title: My view
  cards:
    - type: custom:keep-notes-card
      entity: sensor.keep_notes_sensor
```

## Options

| Name | Type | Default | Description
| ---- | ---- | ------- | -----------
| type | string | **Required** | `custom:keep-notes-card`
| entity | string | **Required** | The entity id of Keep Notes sensor. Always `sensor.keep_notes_sensor`
| title | string | `Title of the note from sensor` | The title of the card.
