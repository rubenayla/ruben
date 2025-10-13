# Driverless Kart

## Overview

A modular autonomous kart platform designed for testing and developing self-driving technologies. This project converts a standard competition kart chassis into an autonomous vehicle, creating a practical outdoor testbed for autonomous driving algorithms and research.

The kart maintains manual drive capability while enabling autonomous operation, making it an ideal platform for validating perception, control, and actuation systems in real-world conditions.

## Key Features

- **Modular Design** - Flexible architecture for testing different autonomous driving components
- **Outdoor Testing** - Real-world environment for algorithm validation
- **Dual Mode Operation** - Switchable between manual and autonomous driving
- **Camera-based Perception** - Cone detection and path planning capabilities
- **ROS Integration** - Migration to ROS-based architecture for better modularity

## Technical Details

### Technologies Used

- **ROS** (Robot Operating System) for system architecture
- **Computer Vision** for cone detection and environment perception
- **Autonomous Control Systems** for path planning and vehicle control
- **Custom Actuation** for steering and braking
- **Telemetry & Emergency Systems** for safety and monitoring

### Architecture

The system follows a modular ROS-based architecture enabling:
- Autonomous perception and environment mapping
- Real-time control and actuation
- Emergency brake systems for safety
- Telemetry for monitoring and debugging

Currently migrating from Python-based systems to a more robust ROS implementation.

## Highlights

!!! success "Practical Testbed"
    Created the first outdoor autonomous vehicle testbed for teachers and researchers to validate their algorithms in real-world conditions.

!!! info "Modular Approach"
    Components are designed to be adaptable for future single-seater Formula vehicles, following industry safety and engineering standards.

## Media

<!-- Add images here -->
<!-- Example:
![Kart Image](../images/kart-photo.jpg)
-->

## Links

- [Full Documentation](https://um-driverless.github.io/kart_docs/) - Complete technical documentation
- [GitHub Repository](https://github.com/um-driverless/kart_docs) - Source code and development
