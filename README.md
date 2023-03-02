# HDMI to MIPI CSI-2 Bridge

Copyright (c) 2017-2021 [Antmicro](https://www.antmicro.com)

![HDMI-MIPI Bridge](/img/hdmi-mipi-bridge.jpg)

## Overview
This repository contains the open hardware design files for Antmicro's HDMI-MIPI Bridge, which is a video accessory converting HDMI video stream into MIPI CSI-2 counterpart. The conversion is performed using Toshiba [TC358743XBG](https://toshiba.semicon-storage.com/ap-en/semiconductor/product/interface-bridge-ics-for-mobile-peripheral-devices/hdmir-interface-bridge-ics/detail.TC358743XBG.html) HDMI interface bridge.
The board includes two independent conversion channels supporting up to two HDMI streams.

## Repository structure:

The main repository directory contains KiCad PCB project files, a [LICENSE](LICENSE), and a README.
The remaining files are stored in the following directories:

* `lib` - contains component libraries
* `doc` - contains generated schematics and other documentation
* `img` - contains graphics for this README

## Key features

* Two independent HDMI-MIPI CSI-2 conversion channels
* Converted MIPI CSI-2 data is exposed on two 4-lane interfaces
* Two assembly variants for regular HDMI and FFC connectors

## Supported platforms

The board exposes MIPI CSI-2 data on a unified 50-pin FFC connector which is electrically compatible with a variety of processing platforms designed by Antmicro.
Those platforms include: 

* [Jetson Nano / Xavier NX Baseboard](https://github.com/antmicro/jetson-nano-baseboard)
* [Jetson Orin NX Baseboard](https://github.com/antmicro/jetson-orin-baseboard)
* [Google Coral Baseboard](https://github.com/antmicro/google-coral-baseboard)
* [Apalis Smart Vision Baseboard](https://github.com/antmicro/apalis-smart-vision-baseboard)
* [TX2 Deep Learning Platform](https://github.com/antmicro/jetson-tx2-deep-learning-platform)

Please note that some additional work might be required to integrate this board with a particular host platform.
Antmicro’s services involve BSP development so you can hire us to make the necessary modifications.

## License
[Apache-2.0](LICENSE)

