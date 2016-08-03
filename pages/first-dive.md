---
layout: default
title: "First Dive"
permalink: /first-dive/
nav:
- Joystick/Controller Functions: joystick-controller-functions
- Dive Modes: dive-modes
- Arming and Disarming: arming-and-disarming
- Tuning: tuning
- Pre-Dive Checklist: pre-dive-checklist
- Recording Video: recording-video
---

# {{page.title}}

This section covers the information you will need to know for your first dive and also some basic configuration to get your ROV diving well.  

## Joystick/Controller Functions

The gamepad controls the ROV during operation. It has been tested with the Microsoft Xbox controller and the Logitech F310. The function of the buttons [depends on those mapped by the user](/initial-setup/#configuring-joystickgamepad) but is usually configured to the following:

<img src="/images/controller.png" class="img-responsive" />

## Dive Modes

**Manual Mode** is normally set to Mode 1 (default mode). In this mode, the vehicle only output motor controls based on the pilot input from the joysticks. There is no feedback stabilization, heading holding, or depth holding.

**Stabilize Mode** automatically stabilizes to level roll and pitch angle and maintains heading when not commanded to turn. The vertical control is left entirely to the pilot.

**DepthHold Mode** is the same as stabilize mode with the addition of automatic depth holding. The throttle control is used to increase or decrease the holding depth.

## Arming and Disarming

By default, the vehicle is disarmed and the motor outputs are disabled. The camera servo and lights will still function when disarmed. 

When armed, the vehicle will actively try to stabilize and the pilot control inputs will be output to the thrusters.

## Tuning

There are a number of control system tuning parameters that can be adjusted to change the performance of the system. Please see the ArduCopter documentation for a detailed description of these parameters.

## Pre-Dive Checklist

To be completed.

## Recording Video

On Mac we recommend using Quicktime to record the entire screen during operation. This will save the telemetry data that is displayed on the screen as well.
