# Touch Screen Controlled Wheelchair

## Bachelor of Technology Capstone Project

### Electronics and Communication Engineering

**Project:** Touch Screen Controlled Wheelchair

**Institution:** Sam Higginbottom Institute of Agriculture, Technology and Sciences (SHIATS), Allahabad, India

**Batch:** 2010–2014

**Project type:** Undergraduate engineering capstone project

---

## 1. Project Overview

This project involved the design and development of a microcontroller-based wheelchair control system using a resistive touchscreen interface.

The objective was to provide an alternative method of controlling wheelchair movement through a touchscreen rather than conventional manual wheel operation.

The system combines embedded control, electronic hardware, motor control, touchscreen interfacing and PCB design.

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
