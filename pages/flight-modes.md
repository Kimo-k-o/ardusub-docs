---
layout: default
title: "Flight Modes"
permalink: /flight-modes/
nav:
- Flight Modes: flight-modes
---

# Flight Modes

ArduSub supports several different flight modes, some of which are only available when certain sensors are present. ArduSub always operates in exactly one flight mode at any given time. ArduSub always boots in *MANUAL* mode.

## Manual

*Manual* mode passes the pilot inputs directly to the motors, with no stabilization. ArduSub (version 3.5+) always starts up in Manual mode. 

## Stabilize

*Stabilize* mode is like *Manual* mode, with heading and attitude stabilization.

## Depth Hold

*Depth Hold* is like *Stabilize* mode with the addition of depth stabilization when the pilot throttle input is zero. A depth sensor is required to use depth hold mode.

# Position Enabled Modes

These modes require an external source of positioning information. A GPS will not work underwater.

## Position Hold

*Position Hold* mode will stabilize the vehicle's absolute position, attitude, and heading when the pilot control inputs are neutral. The vehicle can be maneuvered and repositioned by the pilot.

## Auto

*Auto* mode executes the mission stored on the autopilot autonomously. Pilot control inputs are ignored in most cases. The vehicle may be disarmed, or the mode can be changed to abort the mission.

## Circle

*Circle* mode navigates in circles with the front of the vehicle facing the center point.

## Guided

*Guided* mode allows the vehicle's target position to be set dynamically by a ground control station or companion computer. This allows 'Click to Navigate Here' interactions with a map.

# Secret Menu

## Acro

*Acro* (Acrobatic) mode performs angular rate stabilization.
