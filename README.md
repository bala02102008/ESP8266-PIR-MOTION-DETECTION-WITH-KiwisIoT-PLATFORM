# Building a PIR Motion Detection System Using ESP8266 and KiwisIoT Platform

## 🚀 Introduction

Have you ever wanted to monitor movement in a room using IoT technology?

In this project, I built a simple **PIR Motion Detection System** using an ESP8266 NodeMCU and a PIR sensor.

The system detects human movement and sends the sensor information to the **KiwisIoT Platform** through Wi-Fi.

The KiwisIoT dashboard displays the result in real time:

- True – Motion Detected
- False – No Motion Detected

This project is a simple example of how sensors and IoT technology can work together.

## 🧰 Components Required

To build this project, I used the following components:

| Component | Quantity |
|---|---|
| ESP8266 NodeMCU | 1 |
| PIR Sensor | 1 |
| Jumper Wires | As required |
| USB Cable | 1 |
| Computer | 1 |

## 💻 Software and Tools

- Arduino IDE
- ESP8266 Board Package
- KiwisIoT Arduino Library
- KiwisIoT Platform
- Wi-Fi Connection

## 🔌 Circuit Connections

The PIR sensor is connected to the ESP8266 NodeMCU using jumper wires.

| PIR Sensor | ESP8266 NodeMCU |
|---|---|
| VCC | 3.3V |
| GND | GND |
| OUT | D7 |

The OUT pin sends the sensor signal to the ESP8266.

## ⚙️ How Does It Work?

The working process is very simple:

1. The PIR sensor checks for human movement.
2. When someone moves in front of the sensor, it detects the movement.
3. The ESP8266 receives the sensor signal.
4. If movement is detected, the status becomes True.
5. If no movement is detected, the status becomes False.
6. The ESP8266 sends this information to the KiwisIoT Platform through Wi-Fi.
7. The dashboard displays the motion status.

## 🔄 Project Workflow

```text
PIR Sensor
    ↓
ESP8266 NodeMCU
    ↓
Motion Detection
    ↓
True / False
    ↓
Wi-Fi Connection
    ↓
KiwisIoT Platform
    ↓
Live Dashboard
```

## 📊 KiwisIoT Platform Integration

One of the important parts of this project is connecting the ESP8266 to the KiwisIoT Platform.

The ESP8266 sends the motion status to Channel 0.

The dashboard displays the received information using a Label Widget.

**Dashboard Configuration:**

- Widget Name: Motion Detection
- Channel ID: 0

This makes it easy to check the motion status through the dashboard.

## 🧪 Testing and Results

I tested the project in two conditions.

### 1. Motion Detected

When someone moves in front of the PIR sensor, the output is:

```text
PIR Sensor Value: 1
Motion Status: True
Motion: DETECTED
```

Dashboard Result: **True**

### 2. No Motion Detected

When there is no movement in front of the sensor, the output is:

```text
PIR Sensor Value: 0
Motion Status: False
Motion: NOT DETECTED
```

Dashboard Result: **False**

The project successfully detects movement and sends the status to the KiwisIoT Platform.

## ✨ Project Features

- Real-time motion detection
- ESP8266 Wi-Fi connectivity
- PIR sensor integration
- Live dashboard monitoring
- True / False status display
- Simple and beginner-friendly design

## 🌍 Real-World Applications

This project can be used in different areas, such as:

- Smart Home Monitoring
- Room Movement Detection
- Smart Lighting Systems
- Entry Monitoring
- IoT-Based Monitoring

## 🔮 Future Improvements

In the future, I would like to improve this project by adding:

- LED indicators
- Buzzer alerts
- Mobile notifications
- Automatic light control
- Additional sensors

## 🎓 What I Learned

While building this project, I learned:

- How to connect a PIR sensor with ESP8266.
- How to detect movement using a sensor.
- How to connect ESP8266 to Wi-Fi.
- How to send sensor information to the KiwisIoT Platform.
- How to monitor sensor data through an IoT dashboard.

This project helped me understand how hardware components and IoT platforms work together.

## 📌 Conclusion

This project demonstrates a simple way to detect human movement and monitor it remotely using IoT technology.

By combining a PIR sensor, ESP8266 NodeMCU, and KiwisIoT Platform, we can build a simple real-time motion monitoring system.

It was a great learning experience for understanding sensor interfacing, Wi-Fi connectivity, and IoT dashboard integration.

**Thanks for reading!**

I hope this project helps other beginners who are interested in learning IoT.

**Built With:** ESP8266 NodeMCU | PIR Sensor | Arduino IDE | KiwisIoT Platform
