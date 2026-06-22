# 🏠 ESP32 Based Smart Home Automation System using Blynk IoT

## 🚀 Project Overview

The **ESP32 Smart Home Automation System** is an IoT-based solution that enables users to remotely monitor and control household appliances using a smartphone. Powered by the ESP32 microcontroller and integrated with the **Blynk IoT Platform**, this project provides a seamless, real-time home automation experience from anywhere in the world.

By leveraging Wi-Fi connectivity and cloud-based communication, users can switch appliances ON/OFF, monitor device status, and enhance convenience, energy efficiency, and smart living.

---

## ✨ Key Features

🔹 Remote control of Lights and Fans through a mobile application

🔹 Real-time monitoring of appliance status

🔹 Wi-Fi enabled communication using ESP32

🔹 Manual switch override for local control

🔹 User-friendly Blynk IoT dashboard

🔹 Low-cost and scalable smart home solution

🔹 Supports multiple appliances simultaneously

---

## 🛠 Components Required

| Component               | Quantity    |
| ----------------------- | ----------- |
| ESP32 Development Board | 1           |
| 4-Channel Relay Module  | 1           |
| LED Bulbs / Appliances  | 2-4         |
| Push Buttons            | 2-4         |
| Jumper Wires            | As Required |
| Breadboard              | 1           |
| Wi-Fi Network           | 1           |

---

## ⚙️ Working Principle

1️⃣ ESP32 connects to the local Wi-Fi network.

2️⃣ The device establishes communication with the Blynk Cloud Server.

3️⃣ User sends control commands using the Blynk mobile application.

4️⃣ ESP32 receives the commands in real time.

5️⃣ Relay module activates or deactivates connected appliances.

6️⃣ Device status is instantly reflected on the mobile dashboard.

---

## 📡 System Architecture

```text
📱 Blynk Mobile App
          │
          ▼
       🌐 Internet
          │
          ▼
      ⚡ ESP32 Board
          │
          ▼
    🔌 Relay Module
          │
          ▼
🏠 Home Appliances
```

## 🔗 Circuit Connections

### Relay Connections

| Relay Channel | ESP32 GPIO |
| ------------- | ---------- |
| IN1           | GPIO 23    |
| IN2           | GPIO 22    |
| IN3           | GPIO 21    |
| IN4           | GPIO 19    |

### Push Button Connections

| Button | ESP32 GPIO |
| ------ | ---------- |
| SW1    | GPIO 13    |
| SW2    | GPIO 12    |
| SW3    | GPIO 14    |
| SW4    | GPIO 27    |

---

## 💻 Software & Tools Used

* Arduino IDE
* ESP32 Board Package
* Blynk IoT Platform

### Libraries

```cpp
#include <WiFi.h>
#include <BlynkSimpleEsp32.h>
```

---

## 📄 Sample Firmware Structure

```cpp
#define BLYNK_TEMPLATE_ID "XXXX"
#define BLYNK_AUTH_TOKEN "XXXX"

char ssid[] = "WiFi_Name";
char pass[] = "WiFi_Password";

BLYNK_WRITE(V0)
{
    int state = param.asInt();
    digitalWrite(RELAY1, state);
}
```

---

## 🎯 Applications

🏠 Smart Home Automation

🏢 Smart Office Automation

🏫 Hostel & Classroom Automation

⚡ Energy Efficient Appliance Control

📱 Remote Monitoring & Control Systems

🌐 IoT-Based Smart Infrastructure

---

## 🔮 Future Enhancements

✅ Voice Control using Google Assistant

✅ Amazon Alexa Integration

✅ Energy Consumption Monitoring

✅ Mobile Notifications & Alerts

✅ Smart Scheduling Features

✅ Security & Intrusion Detection





## 👨‍💻 Developed By

**Mrityunjay Patel**

Embedded Systems | IoT | ESP32 | STM32 | Arduino | Smart Electronics

GitHub: https://github.com/Mrityunjay-Patel
