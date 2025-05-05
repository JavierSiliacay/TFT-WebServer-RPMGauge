# 🏎️ Honda Civic RPM Gauge (ESP32 + ILI9341 + Ultrasonic)

A **real-time RPM gauge** simulation styled like a Honda Civic tachometer, displayed on a 2.4" or 3.5" TFT screen (ILI9341), using **ESP32**, **Ultrasonic Sensor**, and **Web Interface**.  

Created by **Javier Siliacay**, an Autotronics student at **USTP (Philippines)**.

![screenshot](https://github.com/javiersiliacay/honda-civic-rpm-gauge/assets/sample.png)

---

## 🚀 Features

- Live **RPM needle animation** on TFT using ultrasonic readings (0–200cm = 1000–8000 RPM)
- **Carbon fiber dashboard design** on TFT
- Built-in **WiFi AP mode** (SSID: `HONDA_CIVIC`)
- **Stylish HTML RPM web UI** (auto-refreshes every 1 second)
- Responsive design with **neon-style needle and redline effects**
- Fully **self-contained** (no internet required)

---

## ⚙️ Hardware Requirements

| Component              | Description                         |
|------------------------|-------------------------------------|
| ESP32 Dev Module       | Main controller                     |
| ILI9341 TFT (SPI)      | 2.4" or 3.5" TFT Display             |
| HC-SR04 Ultrasonic     | Distance sensor (for fake RPM data) |
| Breadboard & Jumpers   | For wiring                          |
| Power Supply           | USB / 5V                            |

---

## 🧠 Concept

- Ultrasonic sensor reads distance from 0 to 200 cm.
- This value is linearly mapped to RPM range **1000 to 8000**.
- The RPM needle moves accordingly and updates on:
  - The **TFT Display** via `Adafruit_ILI9341`
  - The **Web Interface** via ESP32's `WebServer`

---

## 📡 WiFi Configuration

- **WiFi Mode:** Access Point (AP)
- **SSID:** `HONDA_CIVIC`
- **Password:** `shesssh123`
- Access via browser at `http://192.168.4.1`

---

## 🔌 Pinout

| Module            | ESP32 Pin |
|------------------|-----------|
| TFT_CS           | 22        |
| TFT_DC           | 21        |
| TFT_RST          | 18        |
| TFT_MOSI         | 23        |
| TFT_SCK          | 19        |
| TFT_MISO         | 25        |
| TFT_LED          | 5         |
| Ultrasonic Trigger | 12      |
| Ultrasonic Echo    | 13      |

---

## 🛠️ Libraries Required

Install these in the Arduino IDE:
- `Adafruit_GFX`
- `Adafruit_ILI9341`
- `NewPing`
- `WiFi`
- `WebServer` (built-in with ESP32 board)

---

## 🧾 Installation

1. Open Arduino IDE
2. Select your **ESP32 board** (e.g., ESP32 Dev Module)
3. Install all required libraries (see above)
4. Connect your hardware as per the pinout
5. Upload the code
6. Connect to `HONDA_CIVIC` WiFi → open browser at `http://192.168.4.1`

---

## 🖥️ TFT Display Preview

TFT will show:
- RPM needle
- Background styled like a carbon dashboard
- Needle moves based on ultrasonic distance

---

## 🌐 Web UI Preview

The web interface includes:
- Circular RPM meter
- Animated needle synced to sensor
- Neon-style visual effects
- "Redline" effect when RPM > 6400

---

## 📷 Screenshots

![494813059_700998532395659_74537618773182952_n](https://github.com/user-attachments/assets/7bdd3860-975f-417b-95a9-5af698a757e7)


---


