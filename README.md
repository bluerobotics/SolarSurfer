# SolarSurfer

Robotic solar powered surfboard propelled by the BlueRobotics T100 Thruster.

## Overview

The SolarSurfer is robotic surfboard propelled by two T100s. It will be launched from the coast of California on a 2,500 mile journey to Hawaii. It will complete the three-month trip completely autonomously.

Cause why not.

Note: The xml version of the embedded diagrams can be modified with [https://www.draw.io/](https://www.draw.io/).

## Hardware

The following hardware is used:

* qty. 1 8ft surfboard
* qty. 1 custom weighted keel
* qty. 2 [BlueRobotics T100](http://www.bluerobotics.com/thruster/) Thrusters
* qty. 2 BlueRobotics Basic ESCs
* qty. 3 [Pelican 1200](http://www.amazon.com/Pelican-1200-Case-Camera-Black/dp/B0002INQT2) cases

## Electrical

* 120 W SunPower Solar Panel for energy
* Morningstar Solar Charge Controller for power regulation
* 12V, 18Ah Sealed Lead Acid Battery
* [3DR APM 2.6](http://store.3drobotics.com/products/apm-2-6-kit-1)
* [3DR Power Module](https://store.3drobotics.com/products/apm-power-module-with-xt60-connectors) for 5V power regulation and current monitoring
* [3DR uBlox GPS with Compass](http://store.3drobotics.com/products/3dr-gps-ublox-with-compass) - for position tracking
* [3DR Radio](http://store.3drobotics.com/products/3dr-radio) for short-range telemetry
* [Hitec Optima 6 Rx](http://hitecrcd.com/products/aircraft-radios-receivers-and-accessories/2.4ghz-aircraft-receivers-modules/optima-6-6-channel-2.4ghz-receiver/product) for manual control
* [Rock Seven RockBLOCK](http://rockblock.rock7mobile.com/) for satellite communications
* [BLDC Monitor](https://github.com/rjehangir/bldc_monitor)
* TTL Serial camera
* Atlas Scientific pH sensor
* Water temperature sensor w/ one-wire interface
* Airmar WS-100WX wind/temperature/pressure sensor

![SolarSurfer Electrical](SolarSurfer%20Electrical.jpg)

## Software

The complete SolarSurfer software system has many parts. These include:

* [SolarSurferMessage](https://github.com/bluerobotics/SolarSurferMessage) - a custom message format and encoding/decoding library for JavaScript and C++
* [SolarSurferCore](https://github.com/bluerobotics/SolarSurferCore) - the embedded software running on the SolarSurfer; requires SolarSurferMessage
* [SolarSurferAPI](https://github.com/bluerobotics/SolarSurferAPI) - an API that sends, receives, and stores SolarSurfer messages; requires SolarSurferMessage for automated encoding and decoding
* [SolarSurferCommander](https://github.com/bluerobotics/SolarSurferCommander) - a private app to review telemetry and build command messages
* [SolarSurferInfographic](https://github.com/bluerobotics/SolarSurferInfographic) - a public app to view telemetry in an engaging format

![SolarSurfer Infrastructure](SolarSurfer%20Infrastructure.png)

## Test History

### future - Ocean Test No. 4 (Malibu to Monterey)

* tbd

### 2014/08/08 - Ocean Test No. 3 (Santa Monica Canyon)

* First test in open ocean, 20km distance traveled autonomously
* Testing autonomous control via SolarSurferCore
* Testing end-to-end telemetry with SolarSurferCore, SolarSurferAPI, and SolarSurferCommander

### 2014/08/07 - Santa Monica Canyon Prep

* Dry land test with thruster in a tank
* Evaluating solar performance
* Testing end-to-end telemetry with SolarSurferCore, SolarSurferAPI, and SolarSurferCommander

### 2014/07/17 - Ocean Test No. 2 (Marina del Rey)

* Testing autonomous control via SolarSurferCore
* Complete two successful figure eights!

### 2014/06/28 - Ocean Test No. 1 (Marina del Rey)

* First integrated test in a large body of water
* Manual control w/ Aurora 9 TX

### 2014/06/23 - Pool Test

* Tested thrusters mounted on surf board for the first time
* Manual control w/ Aurora 9 TX
