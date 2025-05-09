
# 🚗 Honda Civic RPM Gauge

An ESP32-based real-time RPM gauge display for a Honda Civic-themed project, featuring a TFT screen and a web-based animated dashboard. Created with ❤️ by Javier Siliacay.

![RPM Gauge Preview](https://github.com/javiersiliacay/honda-civic-rpm-gauge/raw/main/preview.gif)

## 🔧 Features

- **Real-Time RPM Simulation** using PWM values
- **TFT Display Output** using `Adafruit_ILI9341` and `Adafruit_GFX` libraries
- **Carbon Fiber Background** aesthetic on the screen
- **WiFi-Enabled Web Dashboard** served via ESP32's built-in web server
- **Fully Custom RPM Gauge** with CSS animations and redline warnings
- **DC Motor Speed Control** to simulate RPM changes

## 📱 Web Dashboard

The ESP32 serves a web-based RPM dashboard that auto-refreshes and displays:

- Current RPM
- Animated needle rotation
- Visual redline warning
- Honda Civic theme UI

## 🧰 Hardware Requirements

- ESP32 Dev Board  
- ILI9341 TFT Display (SPI)
- 1x DC Motor + Driver (PWM Control)
- Power supply (5V or USB)
- Optional: Motor for physical simulation

## 🧪 Libraries Used

- [`WiFi.h`](https://www.arduino.cc/en/Reference/WiFi)
- [`WebServer.h`](https://github.com/espressif/arduino-esp32/tree/master/libraries/WebServer)
- [`Adafruit_GFX`](https://github.com/adafruit/Adafruit-GFX-Library)
- [`Adafruit_ILI9341`](https://github.com/adafruit/Adafruit_ILI9341)

## 📶 WiFi Settings

Update these lines in the code to match your network:

```cpp
const char* ssid = "HONDA_CIVIC";
const char* password = "shesssh123";
````

## 🖥️ Setup Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/javiersiliacay/honda-civic-rpm-gauge.git
   cd honda-civic-rpm-gauge
   ```
2. Open the `.ino` file in Arduino IDE.
3. Select your **ESP32 board** and port.
4. Install all required libraries (listed above).
5. Upload and open the serial monitor.
6. Connect to the ESP32’s IP via browser to see the RPM gauge.

## 👨‍💻 Author

**Javier Siliacay**
Autotronics Student at USTP
GitHub: [@javiersiliacay](https://github.com/javiersiliacay)

---

Made with coffee, solder, and Civic dreams. 🚘🔥

```
SHAAATTTTTTTT ERRS

