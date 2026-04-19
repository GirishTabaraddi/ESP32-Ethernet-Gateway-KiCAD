# Fishtracing scale beacon

## Introduction 

This product will be installed in the fishold of fishing vessels, close to the digital scale. The
digital scale has a single ethernet port which connects the head unit to a central database server
on the bridge of the vessel. Via this ethernet connection the scale beacon can capture weighing 
events and broadcast them via BLE broadcast. 

This hardware consists of a single PCB that contains:
 - A 230V to 3.3V power supply
 - A 3-port 10/100Mbps ethernet switch
 - An SPI-Ethernet bridge
 - An ESP32-S3-WROOM-1 wireless microcontroller module

This project is a professionalisation of the first prototypes  that were based on an ESP32-gateway
board from Olimex. The schematic for that design can be found in 
[docs/esp32_gateway_schematic.pdf](./docs/esp32_gateway_schematic.pdf)

## Part selection

The main parts of this project are:
 - Espressif ESP32-S3-WROOM-1-N16R2
 - Microchip LAN8710A
 - Microchip KSZ8863MLLI
 - Myrra 48021 230V to 3.3V DC-DC

# Power budget

3.3V with a maximum of 750mA should be sufficient for the design.