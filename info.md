# Features
A sensor to integrate Growatt solar panels into Home Assistant.
It tracks three metrics:
- today; the kWh generated today
- total; the kWh generated in total
- current; the W currently generating

# Configuration

Add the following entry into `configuration.yaml`

```yaml
sensor:
  - platform: growatt
    username: USERNAME
    password: PASSWORD
```
