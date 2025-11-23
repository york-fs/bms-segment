# Battery Management System Segment Board

![Revision](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.revision&label=Revision)
![Pad Count](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.pad_count&label=Pad%20Count)
![Via Count](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Finfo.json&query=%24.via_count&label=Via%20Count)
![ERC Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Ferc.json)
![DRC Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-segment%2Fdrc.json)

The distributed BMS segment board connects to a series string of 12 cells and can be queried over isolated I2C to sample
cell voltages and temperatures.

## Features

* **Isolated I2C Communication to the Master Board**
* **Accurate Voltage Measurement Using the MAX14920 Analog Frontend**
* **Passive Cell Balancing**
* **Up to 23 Connected Thermistors**
  * Three onboard thermistors around the cell balancers
  * Twenty external thermistors across two JST PUD connectors

![Preview Render](https://york-fs.github.io/bms-segment/preview.jpg)

## Cloning

A recursive clone must be used to download the `kicad-library` repository:

    git clone --recursive https://github.com/york-fs/bms-segment.git
