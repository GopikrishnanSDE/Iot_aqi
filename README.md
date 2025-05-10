# 🌫️ Smart AQI Monitor & Prediction System

This project monitors the **Air Quality Index (AQI)** in real-time using an **MQ135 gas sensor** and a **DHT11 temperature sensor** connected to an Arduino. It also features a website that shows the current AQI, gives health suggestions, and uses **machine learning** to predict whether a future date is safe for walking based on air conditions.

---

## 🔧 Hardware Used

- Arduino UNO/Nano
- MQ135 Gas Sensor (for air quality)
- DHT11 Sensor (for temperature & humidity)
- Optional: ESP8266 for Wi-Fi data transfer

---

## 📟 Arduino Function

- Reads air quality (analog) from MQ135
- Reads temperature and humidity from DHT11
- Classifies air into basic categories:
  - Excellent, Good, Moderate, Poor, Hazardous
- Sends data to serial monitor or server

---

## 🌐 Website Features

- Shows current **AQI**, **temperature**, and **humidity**
- Gives simple health **suggestions** based on AQI
- Users can select a **future date** to check if it's safe for outdoor walking (using ML prediction)

---

## 🧠 ML Prediction (Optional)

- A basic model predicts whether a given day will be “Safe” or “Not Safe” for walking
- Trained on historical AQI + temperature data
- Exposed via a simple Flask API

---

## 🏥 Health Suggestions Table

| AQI Level      | Condition   | Suggestion           |
|----------------|-------------|----------------------|
| 0–50           | Excellent   | Perfect for walking  |
| 51–100         | Good        | Safe to go outside   |
| 101–150        | Moderate    | Mask recommended     |
| 151–200        | Poor        | Limit outdoor time   |
| 201+           | Hazardous   | Avoid going out      |

---

## 🚀 How to Run

1. Upload the Arduino sketch to your board
2. (Optional) Send data to your website using ESP8266 or USB serial
3. Open the website to view live AQI and health info
4. Use the ML feature to check future safety

---

## 📌 Future Ideas

- Wireless data logging with ESP32
- SMS alerts when AQI crosses threshold
- AI-based advanced prediction models

---

## 👥 Authors

Made by [Your Name / Team Name]  
Powered by Arduino + Web + Machine Learning

---

## 📜 License

Open-source project under MIT License
