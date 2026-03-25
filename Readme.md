# 🏠 Google Assistant-Based Home Automation System

---

## 👋 Introduction
Hello everyone!

I’m **Arun Suthar**, and in this project, I will guide you through building an **AI-powered home automation system** using Google Assistant. This project enables you to control electrical devices in your home using voice commands.

---

## 📌 Project Overview
This project demonstrates how to control an LED bulb (or any electrical appliance) remotely using:
- 📱 Mobile application
- 🎙️ Google Assistant voice commands

It integrates both **hardware** and **software** components to create a seamless smart home experience.

---

## 🧰 Components Required

### 🔌 Hardware
- ESP32 Microcontroller  
- Relay Module  
- LED Bulb (or any electrical device)  
- Jumper Wires  
- Power Supply  

### 💻 Software
- [Arduino IDE](https://www.arduino.cc/en/main/software)  
- [IFTTT](https://ifttt.com/)  
- [Blynk](https://blynk.io/)  

---

## 🔗 Circuit Connection
> Ensure proper and safe wiring while connecting components.

<p align="center">
  <img src="esp.jpg" alt="Circuit Diagram" width="500"/>
</p>

---

## ⚙️ Software Configuration

### 📱 Blynk Setup
1. Download the **Blynk App** from the Play Store or App Store.
2. Create a new account and start a **New Project**.
3. Select **ESP32** as the board.
4. Add a **Button Widget** and assign it to the GPIO pin connected to the relay.
5. You will receive an **Auth Token** via email — save it for later use.

<p align="center">
  <img src="b1.jpg" alt="Blynk Setup" width="300"/>
</p>

---

### 💡 Arduino Configuration
1. Open **Arduino IDE**.
2. Use the sample code from Blynk:
   - [ESP32 Blynk Example Code](https://examples.blynk.cc/?board=ESP32&shield=ESP32%20WiFi&example=GettingStarted%2FPushData)
3. Update the code with:
   - Your **Wi-Fi Name (SSID)**
   - **Wi-Fi Password**
   - **Blynk Auth Token**

4. Upload the code to your ESP32 board.

---

### 🌐 IFTTT Integration (Google Assistant)
1. Create an account on **IFTTT**.
2. Create a new **Applet**:
   - **If This (Trigger):** Google Assistant (voice command)
   - **Then That (Action):** Webhooks
3. Configure Webhooks to send a request to the **Blynk Server**.
4. Link the webhook URL with your Blynk project to trigger the relay.

---

## 🚀 Final Outcome
✅ Control your home appliances using your smartphone  
✅ Use **Google Assistant voice commands** to switch devices ON/OFF  
✅ Experience a simple and scalable IoT-based automation system  

---

## 📢 Conclusion
This project is a great starting point for anyone interested in:
- Internet of Things (IoT)
- Home Automation
- Voice-controlled systems  

Feel free to expand this project by adding more devices and automation features!

---

✨ *Happy Building!*  
