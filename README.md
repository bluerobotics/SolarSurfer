# SolarSurfer

Robotic solar powered surfboard propelled by the BlueRobotics T100 Thruster.

## Overview

The SolarSurfer is robotic surfboard propelled by two T100s. It will be launched from the coast of California on a 2,500 mile journey to Hawaii. It will complete the three-month trip completely autonomously.

Cause why not.

## Hardware

The following hardware is used:

* Invensense MPU-6000 for compass tilt compensation
* UBlox GPS using binary communication
* HMC5883 compass
* [BLDC Monitor](https://github.com/rjehangir/bldc_monitor)
* TTL Serial camera
* [Rock Seven RockBLOCK](http://rockblock.rock7mobile.com/) for satellite communications
* Atlas Scientific pH sensor
* Water temperature sensor w/ one-wire interface
* Airmar WS-100WX wind/temperature/pressure sensor

## Infrastructure

The complete SolarSurfer system has many moving parts. These include:

* SolarSurferMessage - a custom message format and encoding/decoding library for JavaScript and C
* SolarSurferCore - the embedded software running on the SolarSurfer; requires SolarSurferMessage
* SolarSurferAPI - an API that sends, receives, and stores SolarSurfer messages; requires SolarSurferMessage for automated encoding and decoding
* SolarSurferCommander - a private app to review telemetry and build command messages
* SolarSurferCommander - a public app to view telemetry in an engaging format

![Infrastructure](SolarSurfer Infrastructure.png)
