# Piezoelectric Actuator
Author: Brad Nelson (bnelson@mtu.edu)
Updated: 6/13/2018

1. [Summary](#summary)
2. [BLE113 Connections](#ble113-connections)
3. [Changelog](#changelog)

## 1. Summary

## 2. BLE113 Connections
| NAME | ADDR |  DESCRIPTION |
|:---:|:---:|:---|
| ADC0 | 0.0 | Boost Measurement |
| GPIO | 1.0 | Peripheral Enable (not used) |
| GPIO | 1.1 | Boost Enable |
| GPIO | 1.2 | Relay Enable |

## 3. Changelog
#### 0.1 (6/5/18)
* Introduces LT8494 as boost converter controller for 50 V supply
* Introduces solid-state relay to control voltage supply
* Uses voltage divider to provide voltage supply feedback to BLE113
