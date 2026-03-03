
# Automated LPG Safety System with Real-Time Alerts and Absorption Control

## Overview

The Automated LPG Safety System is an IoT-based solution designed to detect LPG gas leakage, provide real-time alerts, and automatically activate a gas absorption mechanism to reduce potential hazards.

The system integrates gas sensors, microcontroller-based processing, motor-driven absorption control, and wireless communication modules to ensure rapid detection and response in domestic and industrial environments.

---

## Problem Statement

Liquefied Petroleum Gas (LPG) leakage can lead to severe risks such as fire, explosion, and toxic exposure. Traditional systems primarily provide alarms without automated corrective action.

This project addresses the need for an intelligent safety system capable of detecting leakage, initiating absorption control, and notifying users instantly.

---

## Key Features

* Continuous LPG monitoring using MQ-6 or MQ-5 gas sensors
* Automatic activation of absorbent chamber upon leak detection
* Real-time alerts via Wi-Fi, GSM, or Bluetooth
* Absorbent material saturation monitoring using MQ-135 sensor
* Load cell monitoring with HX711 module for replacement alerts
* Manual reset and override functionality
* Cost-effective and scalable design

---

## System Architecture

The system consists of the following modules:

### 1. Sensing Layer

* MQ-6 / MQ-5 Gas Sensor for LPG detection
* MQ-135 Sensor for air quality monitoring
* HX711 Load Cell Module for absorbent weight measurement

### 2. Processing Layer

* Arduino Uno microcontroller for data processing and control logic

### 3. Actuation Layer

* Servo Motor / DC Motor / Solenoid for compartment control
* Buzzer and LED indicators for local alerts

### 4. Communication Layer

* ESP8266 / ESP32 for Wi-Fi notifications
* GSM Module (SIM800L / SIM900A) for SMS alerts
* Bluetooth Module (HC-05 / HC-06) for short-range control

---

## Working Principle

1. The gas sensor continuously monitors LPG concentration in PPM.
2. If the gas level exceeds the predefined threshold, the system detects leakage.
3. An alert is triggered through buzzer and wireless communication modules.
4. The motor-driven compartment opens to release activated charcoal and zeolite absorbent material.
5. The HX711 module monitors absorbent weight to determine saturation.
6. When the absorbent reaches capacity, a replacement notification is sent.
7. The system resets after user intervention.

---

## Hardware Requirements

* Arduino Uno
* MQ-6 or MQ-5 Gas Sensor
* MQ-135 Sensor
* HX711 Load Cell Module
* Servo Motor / DC Motor / Solenoid
* ESP8266 or ESP32
* GSM Module (Optional)
* Bluetooth Module (Optional)
* Buzzer and LEDs
* Power Supply (5V or 12V)

---

## Software Requirements

* Arduino IDE
* Embedded C/C++
* Optional IoT Platforms such as Blynk, Firebase, or Adafruit IO

---

## Experimental Results

The system successfully detected gas levels exceeding the threshold of 100 PPM. Upon detection:

* The alert mechanism was activated
* The absorbent chamber opened automatically
* The load cell tracked absorbent saturation

When the absorbent weight exceeded the defined capacity of 1000 grams, a replacement alert was generated.

These results validate the reliability and effectiveness of the proposed system.

---

## Applications

* Residential LPG safety
* Industrial gas monitoring
* Smart home integration
* Small-scale manufacturing units

---

## Future Enhancements

* Cloud-based data analytics dashboard
* Mobile application interface
* AI-based gas pattern recognition
* Integration with smart home ecosystems

---

## Conclusion

The Automated LPG Safety System provides a practical, cost-effective, and intelligent solution for gas leakage detection and control. By combining sensing, actuation, and IoT communication, the system enhances safety through timely alerts and automated corrective measures.


