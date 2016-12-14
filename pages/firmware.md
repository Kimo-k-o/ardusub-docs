---
layout: default
title: "Downloads"
permalink: /firmware/
nav:
- Pixhawk Firmware: firmware
- Raspberry Pi Image: images
- Parameter Files: parameter-files
---

# Firmware

Compiled firmware is now available and can be downloaded from [firmware.ardusub.com](http://firmware.ardusub.com). See here for [instructions on how to flash the Pixhawk](/initial-setup/#loading-firmware-on-pixhawk). Firmware is available for the following hardware:

#### Pixhawk (px4-v2)

**Stable Release:** *(Coming soon, please test ArduSub-3.4-rc2 below)*

**Latest Build:** <i class="fa fa-download" aria-hidden="true"></i> [ArduSub Firmware Repository](http://firmware.ardusub.com/Sub/latest)

## Release History

**ArduSub-3.4-rc2:** *(2016-12-13)* Download [ArduSub v3.4-rc2 here.](http://firmware.ardusub.com/Sub/ArduSub-3.4-rc2/)

Notes:

- Bug fix on external barometer initialization. BRD_TYPE parameter should remain set to 2.
- Please see notes below for v3.4-rc1 as well.

**ArduSub-3.4-rc1:** *(2016-12-11)* ArduSub v3.4 is the first official stable release of ArduSub. After nearly a year of steady development, testing, and improvement, ArduSub has become one of the most capable ROV control systems available. This **release candidate** will be posted for a few weeks for testing before the official v3.4 is released. Please test and provide feedback!

Notes:

- Due to parameter reorganization, all parameters will be overwritten when updating
- Must be used with QGroundControl daily builds or stable version 3.1 (once released)
- Joystick buttons are configured by default
- PX4Firmware sensor drivers have been replaced with in-tree APM drivers. On some hardware, the barometer driver will sometimes hang until a reboot. If your pressure sensor is not detected after rebooting, set the BRD_TYPE parameter to 100 and reboot to fall back to the PX4Firmware driver. Please report back if you experience an issue with the pressure sensor and the new driver.

**Important Note for ArduSub-3.4:** Many unused and inapplicable parameters that ArduSub inherited from ArduCopter have been removed. As a consequence, after flashing V3.4-rc1, all of the parameters will be erased, and the default parameters will be loaded. **You should save your parameters before flashing this firmware.** After loading the new firmware, you can load your saved parameter file through QGroundControl. When loading your old parameter file through QGroundControl, you will see many errors about parameters that have been removed from firmware, this is okay. After you load your parameter file, you need to change the SYSID_SW_MREV parameter to 1 before rebooting in order to prevent the default parameters from being reloaded. This procedure will only have to be done when upgrading from firmware versions prior to V3.4-rc1. Subsequent releases will keep the same parameter format, so this will only have to be done once. If you are using a BlueROV2, it is recommended that you load the [Standard ArduSub Parameters](http://firmware.ardusub.com/parameters/latest/bluerov2.params) after upgrading. The upgrade process is demonstrated in the video below.

<div align="center">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/siJoON6hgq4" frameborder="0" allowfullscreen></iframe>
</div>

# Images

A fully set up image for the Raspberry Pi is available here. This image is used to set up the Raspberry Pi 3 computer as a *companion computer* for the Pixhawk autopilot. See here for [instructions on how to flash the image to the SD card](/raspi-setup/#easy-setup-with-disk-image).

<i class="fa fa-download" aria-hidden="true"></i> [Latest Ardusub-Raspbian Image](http://img.ardusub.com/ardusub-raspbian.img.gz) *(1.47 GB, Updated 2016-10-19)*

# Parameter Files

These files have the recommended parameters for ArduSub, making it easy to setup and update parameters on your vehicle. These parameters will not adjust your accelerometer calibration, compass calibration, or motor directions, but will change joystick button setup, PID controller values, and all other parameters.

<i class="fa fa-download" aria-hidden="true"></i> [Standard ArduSub Parameters](http://firmware.ardusub.com/parameters/latest/bluerov2.params)