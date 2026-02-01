# Adaptive Automatic Headlight Intensity Controller for Vehicles
An ESP8266-based adaptive automatic headlight intensity controller that adjusts brightness in real time using LDR and ultrasonic sensors to reduce glare and improve night-time driving safety.

## Overview
Night-time driving is often dangerous due to glare from oncoming vehicle headlights, which can temporarily blind drivers and increase the risk of accidents. Most existing solutions are manual or expensive and limited to luxury vehicles.

This project presents a low-cost, automatic, and IoT-ready adaptive headlight intensity controller using **ESP8266 NodeMCU**, **LDR**, and **Ultrasonic sensors**.  
The system intelligently adjusts headlight brightness in real time based on ambient light conditions and the distance of approaching vehicles — **without any driver intervention**.

---

## Objectives
- Reduce glare caused by oncoming vehicle headlights
- Improve night-time driving safety and comfort
- Eliminate the need for manual headlight adjustment
- Design a low-cost and energy-efficient solution
- Enable future IoT and smart vehicle integration

---

## Working Principle
The system works based on two real-time inputs:
1. **Ambient Light Intensity** (via LDR sensor)
2. **Distance of Approaching Vehicles** (via Ultrasonic sensor)

### Logic:
- In **dark environments**, the headlight intensity increases.
- When an **approaching vehicle is detected nearby**, brightness is reduced to prevent glare.
- In **bright conditions**, the headlight remains dim.
- Brightness is controlled using **PWM (Pulse Width Modulation)**.

All operations are **fully automatic**, ensuring driver safety and convenience.

---

## Components Used
- ESP8266 NodeMCU
- LDR (Light Dependent Resistor)
- Ultrasonic Sensor (HC-SR04)
- LED (Headlight Prototype)
- Resistors
- Breadboard
- Jumper Wires
- USB / 5V Power Supply

---

## Circuit Connections

| Component            | NodeMCU Pin |
|---------------------|-------------|
| LDR Sensor          | A0          |
| Ultrasonic Trigger  | D6          |
| Ultrasonic Echo     | D5          |
| LED (PWM Control)   | D1          |
| Power Supply        | USB / 5V    |
<img width="324" height="257" alt="Image" src="https://github.com/user-attachments/assets/b1a66a42-b5c9-4974-a01d-9cfa861f035c" />
---

## Software & Tools
- Arduino IDE
- ESP8266 Board Package
- Embedded C / Arduino Programming
- Breadboard Prototyping

---

## Results and Observations

| Ambient Condition | Distance (cm) | LED Brightness |
|------------------|--------------|---------------|
| Dark             | 200 cm       | 255 (Full)    |
| Dark             | 20 cm        | 127 (Dim)     |
| Bright           | 200 cm       | 90 (Dim)      |
| Bright           | 20 cm        | 50 (Low)      |

 The system successfully adapts headlight intensity based on both **light and distance**, validating the effectiveness of the design.

---

## Advantages
- Prevents glare and enhances road safety
- Fully automatic and driver-friendly
- Low-cost and energy-efficient
- Simple hardware design
- IoT-ready and scalable



## Applications
- Adaptive automotive headlight systems
- Smart street lighting
- IoT-based vehicle safety systems
- Autonomous and semi-autonomous vehicles
- Smart city infrastructure

---

## Future Scope
- Integration with **solar power** for energy independence
- **Deep Sleep mode** for power optimization
- **Cloud connectivity** for real-time monitoring
- **AI-based glare detection** for intelligent decision-making
- Mobile app dashboard for control and analytics

---

## 📂Project Structure
Adaptive-Automatic-Headlight-Controller/
│
├── code/
│ └── main.ino
├── circuit/
│ └── circuit_diagram.png
├── docs/
│ ├── Project_Report.pdf
│ └── Presentation.pptx
├── images/
│ └── hardware_setup.jpg
└── README.md
---

## 👨‍💻 Authors
- **Bobbireddi Pranathi**
- **Bollabathini KavyaPriya**
---

## License
This project is licensed under the **MIT License** — feel free to use, modify, and distribute with proper attribution.
---
