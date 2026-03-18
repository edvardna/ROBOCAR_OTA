# 🚗 Robocar IoT System

A cloud-connected mecanum wheel robot with real-time control, sensor feedback, and OTA update capability.

---

## 🚀 Overview
Robocar is a fully integrated **IoT-enabled robotic system** designed for remote control, autonomous navigation, and real-time monitoring.

The system combines embedded hardware, cloud communication, and a custom web interface to create a responsive and scalable robotics platform.

It features mecanum wheels for omnidirectional movement, multiple sensors for environment awareness, and a cloud-based architecture for control and data exchange.

---

## 🧠 Features
- 🌐 **Remote control via web interface (D-pad)**
- ☁️ **MQTT communication (HiveMQ Cloud)**
- 🔄 **OTA firmware updates via GitHub**
- 📡 **Real-time sensor data streaming**
- 🧭 **Maze solving mode**
- ⚡ **Safety watchdog (auto-stop on signal loss)**
- 🔁 **Accurate 90° rotation calibration**
- 📺 **OLED display for system status**

---

## 🛠 Technologies Used
- **ESP32-C5** → WiFi, MQTT, OTA  
- **Arduino Uno** → sensor processing  
- **C / C++** → embedded programming  
- **MQTT (HiveMQ Cloud)** → communication  
- **HTML / JavaScript** → web controller  
- **SSD1306 OLED display**  
- **HC-SR04 ultrasonic sensors (x4)**  
- **L298N motor drivers**  
- **Mecanum wheel drive system**  

---

## ⚙️ System Architecture

### 🔌 Hardware Layer
- 4WD mecanum chassis for omnidirectional movement  
- Ultrasonic sensors for obstacle detection  
- Dual microcontroller setup:
  - Arduino Uno → sensor acquisition  
  - ESP32 → networking and control  

---

### 🔄 Communication Layer
- UART (JSON) between Arduino and ESP32  
- MQTT for cloud communication  
  - Sensor data → published  
  - Control commands → subscribed  

---

### 🌐 Cloud & Interface Layer
- HiveMQ Cloud broker  
- Web-based control interface (hosted online)  
- Real-time control + monitoring  

---

### 🔋 Control Flow
1. User sends command via web UI  
2. MQTT → ESP32 receives command  
3. ESP32 drives motors  
4. Arduino sends sensor data → ESP32  
5. ESP32 publishes data back to cloud  

---

## 🎯 Purpose
The goal of this project was to:
- Build a **complete IoT robotic system**
- Combine **embedded systems + cloud communication**
- Implement **real-time control and feedback loops**
- Explore **autonomous navigation strategies**
- Gain experience in **system-level engineering**

---

## 📸 Preview

![WhatsApp Image 2026-03-01 at 16 58 11](https://github.com/user-attachments/assets/36618001-9c93-45f3-be6d-4169fa05fc22)
<img width="321" height="371" alt="image" src="https://github.com/user-attachments/assets/4bad5683-5439-43e7-b45d-09daf857a43e" />



---

## 📈 Outcome
- Built a fully functional **cloud-controlled robot**
- Implemented **real-time distributed communication system**
- Integrated multiple subsystems (sensors, motors, UI, cloud)
- Demonstrated ability to design **complex engineering systems**
- Created a scalable platform for further robotics development  

---

## 🔗 Future Improvements
- Advanced autonomous navigation (SLAM / mapping)  
- Camera integration (computer vision)   
- Improved motor control (PID tuning)  
- Custom PCB design  
- Battery optimization and power monitoring  

---

## 👤 Author
Edvárd Nagy  
Kevin Kolervo
