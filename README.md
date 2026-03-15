# embedded-temperature-control-oven
Embedded control system for a smart mini oven with PID temperature control and safety monitoring.
# Embedded Temperature Control System for Smart Oven

This project presents the design and implementation of an embedded control system for a mini smart oven. The system automatically regulates the oven temperature using a PID controller while ensuring safety through multiple monitoring mechanisms.

## Project Overview

The goal of this project is to design a complete embedded system capable of maintaining the desired temperature inside a mini oven. The system continuously measures the internal temperature, compares it with the user-defined setpoint, and adjusts the heating power accordingly.

To ensure reliable operation, the system includes safety monitoring features such as overheat protection and door status detection.

## Key Features

- Automatic temperature regulation using PID control
- Real-time temperature measurement
- User-defined temperature and cooking time
- Safety monitoring (overheat detection, door status)
- Audible alarm using buzzer
- User interface with display and buttons

## System Architecture

The system consists of several modules:

**Sensor Module**
- Reads temperature from the oven

**Control Module**
- Computes control signal using PID algorithm

**Safety Module**
- Detects abnormal conditions (overheat, sensor failure)

**User Interface Module**
- Allows the user to configure temperature and cooking time

## System States (FSM)

The control software is implemented using a finite state machine:

- IDLE – waiting for user input
- PREHEAT – heating until target temperature
- BAKING – maintaining temperature during cooking
- PAUSED – paused when door is opened
- FINISH – cooking completed
- FAULT – system error

## Hardware Components

- Microcontroller
- Temperature sensor
- Relay for heating element
- LCD display
- Push buttons
- Buzzer
- Optocoupler isolation circuit

## Tools

- Embedded C
- Microcontroller programming
- Hardware circuit design

## Repository Structure
