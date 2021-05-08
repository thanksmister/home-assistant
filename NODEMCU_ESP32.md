## Table des matières

1. **[Branchements](#branchements)**
2. **[ESPHome](#esphome)**

<br/>

## Branchements

<div align="center">
    <figure>
        <div>
            <img src="/images/board_wroom-32.jpg" alt="" />
        </div>
    </figure>
</div>

<br/>

## ESPHome

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
