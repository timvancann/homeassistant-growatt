[![Build Status](https://travis-ci.org/timvancann/homeassistant-growatt.svg?branch=master)](https://travis-ci.org/timvancann/homeassistant-growatt)

# Home Assistant Growatt sensor

A sensor to integrate Growatt solar panels into Home Assistant.
It tracks three metrics:
- today; the kWh generated today
- total; the kWh generated in total
- current; the W currently generating

## Installation

- Clone or download the component to you `custom_components` folder inside the Home Assistant configuration directory.

```yaml
git clone https://github.com/timvancann/homeassistant-growatt <hass_config>/custom_components
```
- Add the following entry into `configuration.yaml`

```yaml
# Example configuration.yaml entry
sensor:
  - platform: growatt
    username: USERNAME
    password: PASSWORD
```


Note: the component is a bit heavy on the login-side but personally haven't had any issues with that. This is on the todo list.