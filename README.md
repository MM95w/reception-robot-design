# 🤖 Reception & Luggage Service Robot

Mechanical design and simulation-ready development of an indoor autonomous
Reception & Luggage Service Robot.

## 📌 Project Overview

This project focuses on the mechanical design and CAD development of an
indoor service robot intended for reception, guidance and luggage
transport applications in environments such as universities, hotels
and public buildings.

The robot is designed from scratch with a focus on:

- Mechanical design
- Manufacturability
- Modularity
- Easy assembly and maintenance
- Component integration
- Low center of gravity
- ROS 2 compatibility
- Gazebo simulation
- Future autonomous navigation

---

## 🎯 Main Objectives

The project aims to develop a complete mechanical concept including:

- Mobile robot chassis
- Differential-drive system
- Motorized wheels
- Caster wheels
- Battery compartment
- Electronics compartment
- LiDAR integration
- Camera integration
- Human-machine interface
- Luggage platform
- Modular mast
- Cable routing
- Mechanical mounting systems

---

## 📐 Main Specifications

| Parameter | Target |
|---|---:|
| Overall height | ~1500 mm |
| Chassis length | 750 mm |
| Chassis width | 400 mm |
| Chassis height | ~450 mm |
| Drive wheels | 2 × Ø200 mm |
| Caster wheels | 2 |
| Payload | 20–30 kg |
| Battery envelope | 260 × 160 × 135 mm |
| LiDAR | RPLIDAR A1M8 |
| Camera | Arducam IMX519 |
| Display | Waveshare 10.1" HDMI LCD |
| Drive configuration | Differential drive |
| Target environment | Indoor |

---

## 🧩 Main Components

### Drive System

- 2 × ZLLG80ASM250-4096 PU hub motors
- Integrated wheel + motor
- Encoder feedback
- Differential-drive configuration

### Sensors

- RPLIDAR A1M8
- Arducam IMX519 camera

### User Interface

- Waveshare 10.1" HDMI LCD
- Front-facing display
- Camera mounted above the display

### Power

- Battery envelope: 260 × 160 × 135 mm
- Centralized power distribution
- Protected electronics compartment

---

## 🏗️ Mechanical Architecture

The robot is divided into several modular subsystems:

```text
                    ┌──────────────────┐
                    │   LiDAR A1M8     │
                    └────────┬─────────┘
                             │
                    ┌────────┴─────────┐
                    │  Camera IMX519   │
                    ├──────────────────┤
                    │  10.1" LCD       │
                    └────────┬─────────┘
                             │
                         Modular Mast
                             │
              ┌──────────────┴──────────────┐
              │       Luggage Platform      │
              ├─────────────────────────────┤
              │       Main Chassis          │
              │                             │
              │ Battery + Electronics       │
              │                             │
              └─────────────────────────────┘
                 ○                      ○
              Drive Wheel          Drive Wheel
