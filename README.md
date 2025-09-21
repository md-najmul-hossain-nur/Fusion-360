# Smart Waste Management System

## 📌 Overview
The **Smart Waste Management System** is an IoT-based project designed to automate and optimize the process of waste collection.  
It uses **sensors, motors, and wireless communication** to monitor waste levels, detect obstacles, and control robotic movement for efficient collection and disposal.

This system reduces manual labor, saves time, and promotes cleaner environments by ensuring timely waste collection.

---

## 🚀 Features
- **Smart Dustbin Monitoring**  
  - Ultrasonic sensor detects the waste level inside the bin.  
  - LCD display shows the fill percentage.  

- **Bluetooth/Remote Control Car**  
  - Motor driver and Bluetooth module allow the car to move **forward, backward, left, and right**.  
  - Controlled wirelessly using a smartphone.  

- **Robotic Arm with Servo Motors**  
  - Six DOF robotic arm to pick and drop waste items.  
  - Controlled via Bluetooth commands.  

- **Real-Time Distance Measurement**  
  - Ultrasonic sensor ensures the vehicle avoids obstacles.  

- **Automation & Alerts**  
  - LCD provides real-time feedback.  
  - Can be extended with GSM/IoT modules for notifications.  

---

## 🛠️ Hardware Components
- Arduino UNO / Mega
- L293D Motor Driver (or equivalent)
- DC Motors & Wheels
- Servo Motors (x6 for robotic arm)
- Ultrasonic Sensor (HC-SR04)
- Bluetooth Module (HC-05/HC-06)
- LCD Display (16x2 with I2C)
- Power Supply / Battery Pack
- Chassis for vehicle and robotic arm

---

## 💻 Software Requirements
- Arduino IDE
- C/C++ (Arduino language)
- Required Libraries:
  - `Servo.h`
  - `NewPing.h`
  - `Wire.h`
  - `LiquidCrystal_I2C.h`

---

## ⚙️ Working Principle
1. **Monitoring Waste Bin**  
   - The ultrasonic sensor checks the waste level and sends data to the Arduino.  

2. **Vehicle Navigation**  
   - User controls the car wirelessly via Bluetooth commands.  
   - The car moves to the waste bin location.  

3. **Robotic Arm Operation**  
   - Servo motors control the robotic arm to pick and dispose of waste.  
   - Commands like *open gripper, close gripper, lift arm* are mapped to Bluetooth inputs.  

4. **Obstacle Detection**  
   - If the car encounters an obstacle, ultrasonic sensor detects it.  
   - Car movement is adjusted to avoid collision.  

5. **Display Output**  
   - LCD continuously displays distance/waste level.  

---

## 📲 Bluetooth Command Mapping
| Command | Action |
|---------|--------|
| `F` | Move Forward
