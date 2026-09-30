# XrpMazeNavigation
Overview
This repository contains the control software and system architecture for an autonomous maze-navigating robot built on the Experiential Robotics Platform (XRP). The project consists of a comprehensive Python and MicroPython codebase (2,000+ lines) designed to process real-time environmental telemetry and execute complex pathing algorithms without human intervention.

The Challenge
The core objective of this project was to engineer a fully autonomous system capable of navigating a physical maze environment. This required the robot to accurately detect boundaries, make dynamic directional decisions, and maintain structural stability and speed through continuous sensor feedback loops.

Technical Architecture
State-Machine Logic: The core navigation relies on a robust finite state machine to dictate behavioral states (e.g., searching, turning, correcting) based on immediate sensor inputs.

PID Control Loops: Proportional-Integral-Derivative (PID) controllers are implemented to maintain precise motor speeds, correct trajectory drift, and ensure smooth, low-latency execution during tight maneuvers.

Sensor Integration & Telemetry:

Inertial Measurement Unit (IMU): Tracks orientation and angular velocity to execute precise, calculated turns.

Rangefinders & Proximity Sensors: Continuously measure distance to maze walls to prevent collisions and maintain center alignment.

Color Sensors: Identify floor markers and specific environmental triggers within the testing arena.

Modular Design: The codebase is structured into scalable, isolated modules—separating sensor polling, motor control, and high-level decision logic—for efficient debugging and rapid iterative prototyping.

Video Demonstrations
(Embed your unlisted YouTube links or raw video files here)

Demonstration: Full Maze Completion

Demonstration: Sensor Calibration and PID Tuning

Hardware Specifications
Experiential Robotics Platform (XRP) base chassis

MicroPython-compatible microcontroller

Integrated multi-sensor array (IMU, Ultrasonic/Infrared Rangefinders, Optical)
