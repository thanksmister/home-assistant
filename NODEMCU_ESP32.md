<div align="center">
    <figure>
        <div>
            <img src="/images/icon_ha.png" alt="" width="128" height="128" />
        </div>
    </figure>
</div>

## Table des matières

1. **[Connexions](#connexions)**
2. **[ESPHome](#esphome)**

<br/>

## Connexions

<div align="center">
    <figure>
        <div>
            <img src="/images/icon_ha.png" alt="" width="128" height="128" />
        </div>
    </figure>
</div>

## ESPHOME

```yaml
esphome:
  name: esp32
  platform: ESP32
  board: nodemcu-32s

wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password
  fast_connect: on
  manual_ip:
    static_ip: 192.168.1.55
    gateway: 192.168.1.1
    subnet: 255.255.255.0
    #dns1:
    #dns2:

#captive_portal:

logger:

api:
  password: !secret api_password

ota:
  password: !secret ota_password

sensor:
  - platform: wifi_signal
    name: "ESP32 signal"
    update_interval: 600s
```
