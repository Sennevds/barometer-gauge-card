# Barometer gauge Card

A custom gauge card to look like a barometer

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

[![GitHub Release][releases-shield]][releases]


## Options

| Name | Type | Requirement | Description | Default
| ---- | ---- | ------- | ----------- | -------
| type | string | **Required** | `custom:barometer-gauge-card`
| entity | string | **Required** | entity | `sensor.pressure`
| title | string | **Optional** | title of the card | 


## Starting a new card from boilerplate-card

### Step 1

Copy the file barometer-gauge-card.js to your www directory

### Step 2

add the following to your resources in ui-lovelace.yaml file:
```yaml
- url: /local/barometer-gauge-card.js
  type: js
```

### Step 3

add your card:
```yaml
- type: "custom:barometer-gauge-card"
  entity: ...
  title: ...
```


[Troubleshooting](https://github.com/thomasloven/hass-config/wiki/Lovelace-Plugins)

[releases-shield]: https://img.shields.io/github/release/kdw2060/hassio-custom-cards?style=for-the-badge
[releases]: https://github.com/kdw2060/hassio-custom-cards/releases