## Table des matières

1. **[Branchements](#branchements)**
2. **[ESPHome](#esphome)**

<br/>

## Branchements

<div align="center">
    <figure>
        <div>
            <img src="/images/connect_hc-sr04.png" alt="" />
        </div>
    </figure>
</div>

<br/>

## ESPHome

```yaml
sensor:
  - platform: ultrasonic
    trigger_pin: 2
    echo_pin: 4
    name: "ESP32 distance"
    update_interval: 900s
```
