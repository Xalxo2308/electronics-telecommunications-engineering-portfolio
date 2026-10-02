# Touch Screen Controlled Wheelchair

## Bachelor of Technology Capstone Project

**Discipline:** Electronics and Communication Engineering  
**Project:** Touch Screen Controlled Wheelchair  
**Project Type:** Undergraduate Engineering Capstone  
**Period:** 2010–2014

## Overview

A microcontroller-based wheelchair control system using a resistive touchscreen as the user input interface.

The project integrated embedded control, electronic hardware, motor control, LCD interfacing and PCB design.

## Main Components

- ATmega168 microcontroller
- Resistive touchscreen
- L293D motor-driver IC
- Two 12 V DC motors
- 16×2 LCD
- 16 MHz crystal oscillator
- 7805 voltage regulator
- Resistors, capacitors and diodes

## Technical Work

- ATmega168 microcontroller configuration
- Embedded C programming
- GPIO and digital I/O
- ADC-based touchscreen interfacing
- Touch coordinate detection
- L293D motor-driver interfacing
- DC motor direction control
- LCD interfacing
- Ultrasonic sensor interfacing
- Circuit and schematic design
- PCB layout using Express PCB
- PCB fabrication

## Motor Control

The documented program implements:

- Forward movement
- Reverse movement
- Individual motor control
- Direction changes
- Stop
- Parking
- Unparking

Example:

```c
P0 = 0x05;   // Move forward
P0 = 0x0A;   // Move backward
P0 = 0x00;   // Stop
---

## 2. System Architecture

The major functional blocks of the system are:

```text
             ┌─────────────────┐
             │   Touchscreen   │
             └────────┬────────┘
                      │
                      │ User Input
                      ▼
             ┌─────────────────┐
             │    ATmega168    │
             │  Microcontroller│
             └───────┬─────────┘
                     │
                     │ Motor Control
                     ▼
             ┌─────────────────┐
             │     L293D       │
             │  Motor Driver   │
             └───────┬─────────┘
                     │
              ┌──────┴──────┐
              ▼             ▼
          ┌───────┐     ┌───────┐
          │Motor 1│     │Motor 2│
          └───────┘     └───────┘

             ┌─────────────────┐
             │     16×2 LCD    │
             └─────────────────┘
