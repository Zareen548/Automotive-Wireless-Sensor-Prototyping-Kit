# Automotive Wireless Sensor Prototyping Kit

> **Master's Thesis Project**  
> **University of Bremen**  
> **Developed in collaboration with HELLA (FORVIA)**

---

## Overview

This repository presents an overview of my Master's thesis carried out in collaboration with **HELLA (FORVIA)**. The project focused on developing an **ESP32-based automotive wireless sensor prototyping platform** for rapid firmware development, sensor integration, CAN communication, wireless monitoring, and data logging.

The repository showcases the engineering workflow, firmware design methodology, testing process, and MATLAB-based data analysis while intentionally excluding proprietary source code and confidential implementation details.

---

# Project Objectives

The main objectives were to:

- Develop embedded firmware for an ESP32-based automotive prototype
- Integrate multiple automotive sensors
- Acquire and process real-time sensor data
- Implement CAN communication
- Develop an embedded Wi-Fi dashboard
- Log measurements to an SD card
- Validate firmware through systematic testing
- Analyze recorded sensor data using MATLAB

---

# Technical Stack

## Programming Languages

- C
- C++
- MATLAB

## Embedded Platform

- ESP32
- Arduino Framework

## Communication

- CAN Bus
- Wi-Fi
- HTTP Web Server

## Storage

- SD Card

## Sensors

- Pressure Sensor
- Environmental Sensor
- 6-Axis IMU

## Development Tools

- Arduino IDE
- MATLAB
- Git
- Serial Monitor
- CAN Analyzer

---

# Key Features

- Real-time sensor acquisition
- Multi-sensor integration
- CAN communication
- Embedded HTTP web server
- Wireless dashboard
- SD card logging
- Sensor calibration
- Firmware validation
- MATLAB data analysis
- Embedded system testing

---

# System Workflow

<p align="center">
<img src="docs/sanitized_system_overview.png" width="750">
</p>

The firmware continuously acquires sensor measurements, validates incoming data, communicates through the CAN interface, updates an embedded web dashboard, and stores measurements for offline analysis.

---

# Embedded Web Dashboard

The ESP32 hosts a lightweight HTTP server that allows users to monitor sensor measurements wirelessly from any device connected to the same network.

### Dashboard Features

- Live pressure monitoring
- Temperature display
- Humidity monitoring
- IMU measurements
- Connection status
- Automatic dashboard refresh
- Embedded HTTP server

<p align="center">
<img src="web_dashboard/dashboard_mockup.png" width="750">
</p>

For confidentiality reasons, the actual HTML/CSS and firmware implementation are not included. A simplified workflow is available in the **web_dashboard/** directory.

---

# Firmware Validation

The firmware was tested using multiple functional validation scenarios.

Validated modules include:

- Pressure sensor
- Environmental sensor
- IMU
- CAN communication
- SD card logging
- Wi-Fi communication
- Embedded web server
- Error handling

<p align="center">
<img src="docs/firmware_test_summary.png" width="700">
</p>

---

# MATLAB Data Analysis

After data acquisition, recorded measurements were analyzed using MATLAB to evaluate system performance.

The analysis included:

- Pressure stability
- Temperature variation
- Motion characteristics
- Sensor consistency
- Basic statistical analysis
- Data visualization

### Pressure Analysis

<p align="center">
<img src="docs/pressure_analysis.png" width="700">
</p>

---

### Temperature Analysis

<p align="center">
<img src="docs/temperature_analysis.png" width="700">
</p>

---

### Acceleration Analysis

<p align="center">
<img src="docs/acceleration_analysis.png" width="700">
</p>

---

# Repository Structure

```
automotive-wireless-sensor-prototyping-kit/
│
├── README.md
│
├── docs/
│   ├── sanitized_system_overview.png
│   ├── firmware_test_summary.png
│   ├── pressure_analysis.png
│   ├── temperature_analysis.png
│   └── acceleration_analysis.png
│
├── web_dashboard/
│   ├── README.md
│   ├── dashboard_workflow.md
│   ├── webserver_pseudocode.md
│   └── dashboard_mockup.png
│
├── pseudocode/
│   ├── pressure_monitoring_logic.md
│   ├── acceleration_event_detection.md
│   └── data_logging_workflow.md
│
├── matlab/
│   ├── sensor_data_analysis_pseudocode.m
│   └── plot_static_sensor_results_pseudocode.m
│
├── results/
│   └── test_summary.md
│
└── LICENSE
```

---

# Firmware Design (Simplified)

```text
Initialize Hardware

Initialize Sensors

Initialize CAN Interface

Initialize Wi-Fi

Initialize SD Card

Start HTTP Server

while(system_running)

    Read Sensor Measurements

    Validate Data

    Update CAN Messages

    Save Measurements

    Update Dashboard

    Check System Status

end
```

Additional pseudocode describing individual firmware modules is available in the **pseudocode/** directory.

---

# Engineering Skills Demonstrated

- Embedded Firmware Development
- C/C++ Programming
- ESP32 Development
- Automotive Sensor Integration
- CAN Communication
- Embedded HTTP Server
- Wireless Communication
- Real-Time Data Acquisition
- Data Logging
- Firmware Validation
- MATLAB Data Analysis
- Embedded System Testing
- Technical Documentation
- Git Version Control

---

# Results

The developed prototype successfully demonstrated:

- Reliable acquisition of multiple sensor signals
- Stable CAN communication
- Embedded wireless monitoring
- Real-time sensor visualization
- Reliable SD card logging
- Modular firmware architecture
- MATLAB-based offline data analysis

The project provides a flexible embedded platform for evaluating automotive sensing concepts during the prototyping phase.

---

# Confidentiality Notice

This repository has been intentionally sanitized to comply with the confidentiality agreement established during my Master's thesis collaboration with **HELLA (FORVIA)**.

The following items are **not included**:

- Production firmware
- Complete source code
- Proprietary communication protocols
- PCB designs
- Hardware schematics
- Internal software architecture
- Calibration algorithms
- Confidential datasets

Only project documentation, simplified workflows, pseudocode, and representative analysis are provided to demonstrate the engineering process and technical competencies.

---

# Acknowledgements

This work was completed as part of my Master's thesis at the **University of Bremen** in collaboration with **HELLA (FORVIA)**.

---

# Author

**Syeda Tajkia Zareen**

M.Sc. Communication and Information Technology  
University of Bremen

**Areas of Interest**

- Embedded Systems
- Automotive Electronics
- Firmware Development
- Sensor Integration
- Hardware Validation
- Embedded Networking
- MATLAB Data Analysis
