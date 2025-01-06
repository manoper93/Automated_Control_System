9# Automated Control System with PWM and Sensor Integration

This project implements an automated control system using a microcontroller, featuring PWM modulation, EEPROM data storage, and various sensor integrations. The system is designed to manage motor control, safety mechanisms, and dynamic adjustments based on real-time sensor readings.

## Features

- **PWM Control:** Dynamically adjusts motor power based on system states and sensor feedback.

- **EEPROM Storage:** Saves and retrieves operational data to ensure continuity across power cycles.

- ### Sensor Integration:

  - Hall effect sensor for positional feedback.

  - Photoresistor for light-based system interruption.

  - Emergency stop sensor for safety.

  - Voltage sensor for power monitoring.


- ### Automatic and Manual Modes:

  - Supports automatic operation based on pre-configured parameters.

  - Manual override for user intervention.


- ### Real-Time Monitoring: 
  - Outputs system status and operational logs via serial communication.


## Hardware Pin Mapping

| **Pin** | **Function**            |
|---------|-------------------------|
| D2      | Execute Button          |
| D4      | Status LED              |
| D5      | Photoresistor Switch    |
| D6      | PWM Output              |
| D7      | PWM Switch              |
| D8      | Save Settings Switch    |
| D9      | Motor 2 Control         |
| D10     | Motor 1 Control         |
| D11     | Hall Sensor             |
| D12     | 24V Power Control       |
| A1      | Stop Sensor             |
| A2      | Photoresistor           |
| A3      | Receiver ch2            |
| A4      | Receiver ch1            |
| A5      | Voltage Sensor          |


## Code Overview

- **Setup Phase:** Initializes pins, reads EEPROM data, and sets default states.

- ### Loop Functions:

  - **PWM Control:** Manages motor speed and direction based on sensor data.

  - **Emergency Handling:** Stops the system when safety conditions are met.

  - **Data Logging:** Provides real-time feedback via serial communication.

  - **EEPROM Updates:** Ensures operational data persistence.



## How to Use

1. **Initial Setup:** Connect components according to the hardware pin mapping.


2. **Calibration:** Use the manual mode to configure and save system parameters.


3. **Operation:** Choose between automatic or manual modes to control the system.


4. **Monitoring:** View real-time logs via the serial monitor for debugging and system insights.



## Applications

This code can be adapted for various applications, including automated gates, conveyor systems, or other motorized setups requiring precise control and safety mechanisms.

## Photos

![20201229_190907](https://github.com/user-attachments/assets/34eb36d3-d4e2-4830-8478-0801c2f72f7b)
![20201229_191403](https://github.com/user-attachments/assets/3ce568cd-cd64-4ef8-afa7-02ad9b83d453)
