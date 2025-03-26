# 🚦 RoadSafe: AI-Powered Smart Traffic Monitoring and Control  

## 📌 Overview  
**RoadSafe** is an intelligent traffic monitoring system designed to enhance **road safety** by integrating **AI, IoT, and smart traffic control**. The system uses **AI-powered traffic cameras** and **smart traffic lights** to detect **red-light violations, accidents, and real-time traffic conditions**, ensuring safer and more efficient roads.  

## 🎯 Features  

✅ **AI-Based Traffic Monitoring**  
   - Detects red-light violations and captures license plates using **OCR (Optical Character Recognition)**.  
   - Automatically issues alerts for traffic infractions.  

✅ **Real-Time Accident Detection**  
   - Identifies collisions at intersections.  
   - Sends **instant alerts** to traffic authorities for emergency response.  

✅ **Smart Traffic Light System (Arduino Mega + ESP8266)**  
   - **Four traffic lights** following a structured cycle:  
     - 🔴 Red: **9 seconds**  
     - 🟡 Yellow: **3 seconds**  
     - 🟢 Green: **9 seconds**  
   - **LDR Sensor-Based LED Brightness Control**  
     - Uses **PWM** to dynamically adjust brightness based on ambient light conditions.  
   - **Manual Override via Web Interface**  
     - Allows emergency personnel to **remotely change signals** in critical situations.  

## 🛠️ Hardware & Software Components  

### **Hardware**  
- 🔹 **ESP8266** (WiFi Module)  
- 🔹 **Arduino Mega** (Main Controller)  
- 🔹 **LDR Sensor** (For ambient light detection)  
- 🔹 **Seven-Segment Displays** (For countdown timers)  
- 🔹 **Traffic Light LEDs**  

### **Software & Technologies**  
- 💻 **C++ (Arduino IDE)**
- 🌐 **ESPAsyncWebServer** (Web-based traffic control)
- 🧠 **OpenCV & OCR (AI-based detection)**
- 🔗 **WiFi Communication (ESP8266 & Arduino Mega)**  

## 🎬 How It Works  

1️⃣ **Traffic Light Automation**: The system follows a structured sequence while adapting to ambient light conditions.  
2️⃣ **Manual Override**: Pressing `T1` forces the corresponding light to **turn green immediately** if it was red.  
3️⃣ **Adaptive Transition**: Pressing `T4` shifts from green → yellow (3s) → red → next light turns green.  
4️⃣ **AI Monitoring**: A webcam detects red-light violations and captures **license plate information** for enforcement.  
5️⃣ **Accident Alerts**: AI detects accidents and **notifies traffic authorities** for faster emergency response.  

## 🔗 Web Interface Demonstration  

Since **WiFi restrictions** prevent port forwarding, the app currently **cannot access the ESP8266 remotely**.  
However, a **backup web interface** allows local real-time control, demonstrating the system’s feasibility.  


## 🚀 Installation & Setup  

### **1️⃣ Setting Up the Arduino & ESP8266**  
1. Install **Arduino IDE** and the required ESP8266 libraries (`ESPAsyncWebServer`, `Ticker`, `WiFi`).  
2. Flash the **ESP8266 firmware** with the provided `.ino` file.  
3. Upload the **Arduino Mega code** for traffic light control.  

### **2️⃣ Running the AI-Based Monitoring System**  
1. Install **Python 3.x** and required packages:  
   ```sh
   pip install opencv-python pytesseract flask
