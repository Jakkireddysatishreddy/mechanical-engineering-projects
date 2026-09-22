# Minor Project

## Project Title

Design and Development of an ESP32-Based Autonomous Fire-Fighting Robot with Multi-Axis Nozzle Control

## Project Overview

This project focuses on the design and development of a compact, wheeled autonomous fire-fighting robot built around the ESP32 microcontroller. The robot detects a fire source, navigates toward it using a differential-drive chassis, and extinguishes it with a targeted water spray — without any human involvement.

The objective of the project is to combine multi-sensor directional flame detection with multi-axis nozzle positioning (horizontal, vertical, and height adjustment) to overcome the single-sensor, fixed-nozzle limitations seen in most existing fire-fighting robot designs, producing a low-cost, reproducible platform suited to warehouses, electrical control rooms, and other high-risk settings.

## Problem Statement

Existing fire-fighting robots and fixed suppression systems have the following limitations:

- Fixed suppression systems (e.g., ceiling sprinklers) activate uniformly across a zone and cannot reposition toward the actual source of a fire, making them ineffective against off-centre, unevenly spread, or elevated fires.
- Most microcontroller-based fire-fighting robots reported in the literature use single-sensor detection or a fixed-orientation nozzle, which limits precision targeting of the flame.
- Existing servo-assisted designs generally provide horizontal aiming only and do not adjust for the height of the flame, so they cannot reach fires on shelves, racks, or elevated platforms.
- IoT-enabled and networked designs add remote monitoring but remain constrained to basic, non-directional spraying, and their dependence on connectivity introduces an additional point of failure.

## Objectives

- Design a chassis-mounted fire-detection unit using three angularly placed infrared flame sensors for left/centre/right directional resolution.
- Develop a differential-drive mobility system (DC gear motors + L298N driver) controlled by an ESP32 to autonomously navigate toward a detected flame.
- Analyze and implement a two-axis servo nozzle (horizontal + vertical) combined with a lead-screw linear actuator for independent height adjustment, enabling precision targeting at varying flame positions and elevations.
- Test the complete system through repeated bench trials for detection accuracy, navigation accuracy, targeting precision, and suppression reliability.

## Methodology

1. Problem identification
2. Concept development
3. CAD modeling
4. Material selection
5. Manufacturing
6. Assembly
7. Testing
8. Results

## Software Used

- Autodesk Fusion 360
- MATLAB
- ANSYS / FEA
- AutoCAD

## Project Images

### CAD Model

![CAD Model](Images/cad_model.png)

### Prototype

![Prototype](Images/prototype.png)

### Testing

![Testing](Images/testing.png)

## Results

The developed system was tested through repeated bench trials in which a small controlled flame was placed at varying positions and heights in front of the robot.

The major results obtained were:

- The three-sensor flame detection arrangement consistently detected the fire and correctly resolved its direction (left/centre/right), giving noticeably more reliable direction estimates than a single-sensor design.
- The differential-drive navigation logic consistently steered the robot toward the detected source, with continuous sensor feedback self-correcting minor heading drift en route.
- The two-axis servo assembly reliably aligned the nozzle with the flame on arrival, and the linear actuator's height adjustment allowed the nozzle to reach flames placed at an elevation as well as at ground level — a targeting capability absent in the fixed-nozzle designs reviewed.
- The pump delivered sufficient flow to suppress the small test flames within a short interval, and the full detect-navigate-target-suppress sequence repeated reliably across multiple runs without failure.
- Two limitations were observed: sensor sensitivity degraded under strong ambient lighting, and the pump's flow rate restricts the current prototype to small-scale or early-stage fires; uneven floor surfaces also introduced minor navigation inaccuracy.

## My Contribution

- Mechanical design of the chassis, nozzle gimbal bracket, and linear height-adjustment (lead-screw) stage
- CAD modeling of the robot assembly
- Component selection (flame sensors, DC gear motors, L298N driver, servo motors, linear actuator, pump)
- Manufacturing and fabrication of mechanical parts
- Assembly and mechanical–electronics integration
- Testing across multiple flame positions and elevations
- Documentation and publication of the work (IJVRA)

## Skills Learned

- Mechanical Design
- CAD
- Manufacturing
- FEA
- Engineering Drawing
- Problem Solving

- Mechanical Design
- CAD
- Manufacturing
- FEA
- Engineering Drawing
- Problem Solving
