# Steering System

*Subsystem of [Driverless Kart](kart.md).*

**2020 - present**

<video width="100%" controls muted playsinline>
  <source src="../videos/steering-jetson.mp4" type="video/mp4">
</video>

*Steering mechanism with the Jetson Orin in frame.*

## Overview

Mechanical and control system for autonomous steering actuation, enabling precise path following and vehicle control in autonomous racing applications.

## Key Features

- **Precise Actuation** - Accurate steering angle control for path following
- **Mechanical Integration** - Custom mounting and linkage design for racing kart
- **Control Interface** - Integration with autonomous control systems
- **Safety Features** - Manual override and fail-safe mechanisms

## Technical Details

### Implementation

- Mechanical design and integration with existing vehicle chassis
- Actuator selection, sizing, and characterization
- Control system development and tuning
- Safety and redundancy implementation

### Technologies Used

- Mechanical design and CAD
- Control systems engineering
- Actuator interfacing and control
- Safety system design

## Highlights

!!! success "Autonomous Path Following"
    Enabled precise autonomous steering control for racing applications with sub-degree accuracy.

!!! info "Safety Integration"
    Designed fail-safe mechanisms allowing seamless transition between autonomous and manual control.

## Engineering: nylon → brass sun gear

The planetary reducer's nylon sun gear kept failing at the motor shaft's D-flat — not by tooth shear, but by the bore plastically deforming around the flat under repeated direction reversals. A D-flat transmits torque through a tiny line-contact along the flat edge, and nylon **creeps** under sustained stress and creeps fast under *repeated impulsive* stress. Every reversal with any backlash loads that edge with an impact, not a smooth torque. Over thousands of reversals the bore wears round, backlash grows, impacts get harder, damage accelerates. Software mitigations (slew limits, output deadband, D-term LPF) slow the failure but can't prevent it — the root cause is material + geometry, not control.

The fix is to machine the sun in brass, leaving the planets and ring as nylon. Counterintuitively this works in our favour: the sun is the highest-duty part in a planetary (rotates fastest, every tooth engages every revolution), so making *it* the durable part is exactly correct. Wear migrates to the planets — three of them, each rotating slower than the sun, sharing load over an order of magnitude gentler per-tooth duty, and they are simple plain spur gears with no D-flat or keyway, trivially batch-printable as spares. Failure mode also upgrades: today's "sun bore rounds out → sudden total loss of steering" becomes "planet teeth wear gradually → audible/visible backlash → scheduled maintenance." Graceful degradation instead of catastrophic.

![Steering planetary gear and motor](../images/kart/steering-planetary.jpg)

## Context

Part of the [Driverless Kart](kart.md). Mechanical actuation + control loop integration with the Jetson and ESP32.
