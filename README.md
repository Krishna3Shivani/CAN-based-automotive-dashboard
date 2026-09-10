# CAN-based-automotive-dashboard
PIC18F4580-based automotive dashboard using CAN communication to exchange vehicle parameters such as speed, gear, RPM and indicators between ECUs and display them.

## Overview

This project implements a **CAN-based automotive dashboard** using the **PIC18F4580 microcontroller**.

The system uses multiple ECUs to collect and exchange vehicle-related information through the **Controller Area Network (CAN)** protocol. The dashboard displays parameters such as **vehicle speed, gear position, RPM, and turn indicators** on a character LCD.

## Features

* CAN communication between multiple ECUs.
* Vehicle speed calculation using ADC input.
* Gear position selection and display.
* RPM data transmission through CAN.
* Turn indicator control and display.
* Real-time display of vehicle parameters on CLCD.
* ECU-to-ECU communication using CAN messages.

## Hardware Used

* PIC18F4580 microcontroller

## Software and Tools

* Embedded C
* MPLAB X IDE
* XC8 Compiler
* PIC18F4580
* CAN Protocol

## System Architecture

The project consists of multiple ECUs communicating through the CAN bus.


              CAN BUS
     ┌───────────────────────┐
     │                       │
     ▼                       ▼
┌──────────┐             ┌──────────┐
│  ECU 1   │             │  ECU 2   │
│          │             │          │
│  Speed   │             │   RPM    │
│  Gear    │             │          │
└────┬─────┘             └────┬─────┘
     │                        │
     └───────────┬────────────┘
                 ▼
            ┌──────────┐
            │  ECU 3   │
            │          │
            │  CLCD    │
            │ Speed    │
            │ Gear     │
            │ RPM      │
            │ Indicator│
            └──────────┘

## Key Concepts

* CAN protocol
* CAN frame structure
* CAN arbitration
* ECU-to-ECU communication
* ADC
* Digital input handling
* Character LCD interfacing
* Switch debouncing / state-change detection
* ASCII conversion
* Interrupts
* Embedded C
* PIC18F4580 peripherals

## My Contribution

* Developed embedded C logic for the dashboard application.
* Implemented ADC-based speed calculation.
* Implemented gear selection and display logic.
* Worked with CAN communication for ECU-to-ECU data exchange.
* Implemented LCD display of vehicle parameters.
* Integrated speed, gear, RPM and indicator information at the dashboard ECU.


## Future Improvements

* Add additional vehicle parameters such as temperature and fuel level.
* Implement CAN error handling and diagnostics.
* Add more ECUs and vehicle parameters.
* Improve the dashboard interface.
* Add data logging for vehicle parameters.


B.E. Electronics and Communication Engineering
