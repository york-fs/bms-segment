# Battery Management System Segment Board

![Revision](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.revision&label=Revision)
![Pad Count](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.pad_count&label=Pad%20Count)
![Via Count](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.via_count&label=Via%20Count)
![ERC Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Ferc.json)
![DRC Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Fdrc.json)

The BMS segment board is part of the car's distributed BMS design. It connects to a series string of up to 16 cells and
connects over an isolated I2C interface to the BMS master board to transfer cell voltage and temperature measurements.

[Latest Release](https://github.com/york-fs/bms-segment/releases/latest)
[Interactive BOM](https://york-fs.github.io/bms-segment/ibom.html)

## Features

* **Up to 16-Cell Voltage Measurement Frontend with Passive Balancing**
  * Utilises the MAX14921 analog frontend IC
* **Buck Converter to Derive On-Board Power From the Connected Segment**
  * Around 120 uA quiescent current consumption in standby
* **Isolated I2C Communication to the Master Board**
* **Up to 24 Connected Thermistors**
  * Four onboard thermistors spread across the cell balancers
  * Twenty external thermistors across two JST PUD connectors
* **Short Circuit Protection on the External Thermistors**
* **Daughter Board Design for Connecting Cell Taps**
  * Allows any cell tap connector to be used and the ability to use any cell count between 3 and 16

![Render Preview](https://york-fs.github.io/bms-segment/render.jpg)

## Cloning

A recursive clone must be used to download the `kicad-library` repository:

    git clone --recursive https://github.com/york-fs/bms-segment.git
