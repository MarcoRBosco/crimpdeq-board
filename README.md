# Crimpdeq board

TODO

## Where to buy

TODO

## Project Specification

TODO

### Futures

### I2C Peripherals

This board includes the following peripherals over the I2C bus:

| Peripheral               | Part number | Reference                                                                                                      | Crate                                     | Address |
| ------------------------ | ----------- | -------------------------------------------------------------------------------------------------------------- | ----------------------------------------- | ------- |
| IMU                      | ICM-42670-P | [Datasheet](https://invensense.tdk.com/download-pdf/icm-42670-p-datasheet/)                                    | [Link](https://crates.io/crates/icm42670) | 0x68    |
| Temperature and Humidity | SHTC3       | [Datasheet](https://www.mouser.com/datasheet/2/682/Sensirion_04202018_HT_DS_SHTC3_Preliminiary_D2-1323493.pdf) | [Link](https://crates.io/crates/shtcx)    | 0x70    |

TODO: Add Maxim gauge and cell load ADCs

#### I2C Bus Connection

| Signal | GPIO   |
| ------ | ------ |
| SDA    | GPIO10 |
| SCL    | GPIO8  |

TODO: Add Maxim gauge and cell load ADCs

### I/Os

The following devices are connected through GPIO:

| I/O Devices | GPIO  |
| ----------- | ----- |
| WS2812 LED  | GPIO2 |
| LED         | GPIO7 |
| Button/Boot | GPIO9 |

TODO: Add battery leds

### Power

* USB type-C (*no PD compatibility*).
* Li-Ion battery charger - MCP73831T-2ACI/OT, it charges up to 4.2V.
  * Recommendation: MCP73831T-2ACI/OT does not provide battery protection for over-current or over-discharge. For the battery (Li-Ion or Li-Po), it's recommended the ones with embedded protection
  * Limitation: reading the battery voltage is not supported.

### Pin Layout

TODO

## Project KiCad Libraries

* [Espressif KiCad Libraries v3.0.2](https://github.com/espressif/kicad-libraries/releases/tag/3.0.2)
* [UAMP KiCad Libraries v1.0.1](https://github.com/uampio/UAMP-KiCad-Libraries/releases/tag/1.0.1)

## Board Design

Top

TODO

Bottom

TODO

## Bill of Material

TODO

## Case

TODO
