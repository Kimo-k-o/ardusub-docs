---
layout: default
title: "Firmware"
permalink: /firmware/
nav:
- Firmware: firmware
- Raspberry Pi Image: images
---

# Firmware

## Overview

There are three different types of firmware:

 - Stable: The recommended build for most users.
 - Beta: A pre-release of a stable build, used for testing and bugfixes before officially labeling a build as stable. The versions for the these builds are suffixed with *-rcx*, where rc stands for release candidate, and x is a number that is incremented as the beta is updated.
 - Development: Development build, updated frequently. This build should only be used in practice by developers and advanced users. The versions for these builds are suffixed with *-dev*.

The latest stable release of ArduSub is 3.4. The current beta is 3.5-rc1, and requires a recent build of QGroundControl (later than 3.1.3) to operate. The latest development version is 3.6-dev.

## What Version is Installed?

To find out what firmware version is installed on your autopilot, [refresh your parameters](/configuring/#parameters). When the parameters are refreshed, the autopilot sends its software version information via STATUSTEXT messages. You can view these messages by clicking the *Messages* icon in QGroundControl. The *Messages* icon looks like a megaphone, or a warning sign if there are pending warnings. Here, you can see that the ArduSub version is *V3.5-rc1*.

<img src="/images/firmware/statustext-version.png" class="img-responsive img-center" style="max-height:600px;">

## Updating

It is **highly recommended** to [save your parameters](/configuring/#saving-and-loading) to a file before updating your firmware. To update your firmware using QGroundControl, go to the *Vehicle Setup Page* and click the *Firmware* tab. Plug your autopilot into the computer with a USB cable. Click ArduPilot flight stack, and choose your desired version to load. Beta and Development options are available after clicking the *Advanced settings* checkbox. *Stable* is not yet available through QGC for ArduSub. After you have selected your desired version, click *Ok* and wait for the upload to complete.

<img src="/images/firmware/qgc-upgrade.png" class="img-responsive img-center" style="max-height:600px;">
