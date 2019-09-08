[![Build Status](https://travis-ci.org/timvancann/homeassistant-growatt.svg?branch=master)](https://travis-ci.org/timvancann/homeassistant-growatt)

# Home Assistant Growatt sensor

A sensor to integrate Growatt solar panels into Home Assistant.
It tracks three metrics:
- today; the kWh generated today
- total; the kWh generated in total
- current; the W currently generating

## Installation

- Grab the latest release and download it to your `custom_components` folder inside the Home Assistant configuration directory and unpack it.
- Or use [HACS](https://hacs.netlify.com/) to manage the installation


Add the following entry into `configuration.yaml`

```yaml
# Example configuration.yaml entry
sensor:
  - platform: growatt
    username: USERNAME
    password: PASSWORD
```

Note: the component is a bit heavy on the login-side but personally haven't had any issues with that. This is on the todo list.