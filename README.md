# 🚮 Smart Dustbin using ESP32 + Ultrasonic + Servo + Blynk

An IoT-based smart dustbin that automatically opens when someone comes close. It sends real-time distance data to the Blynk app and can also be controlled manually via the app.

## 📦 Components Used

- ESP32
- Ultrasonic Sensor (HC-SR04)
- Servo Motor (SG90 or MG90)
- Blynk IoT App
- Jumper wires, breadboard
- Power source (Battery or USB)

## 🔌 Circuit Connections

| Component      | ESP32 Pin |
|----------------|-----------|
| Trig (HC-SR04) | D5        |
| Echo (HC-SR04) | D18       |
| Servo Signal   | D23       |
| Power & GND    | 3.3V & GND|

(Full `.fzz` circuit diagram will be added soon)

## 📲 Blynk Setup

- Create a new template in Blynk IoT Dashboard.
- Add a **Label (V0)** to show distance.
- Add a **Button (V1)** to manually open the bin.

## 🧠 Features

- Auto-opens lid when hand detected (<15 cm)
- Distance sent to Blynk app (every 2 seconds)
- Manual override via mobile app

## 🛠️ How to Use

1. Open the `.ino` file in Arduino IDE
2. Replace WiFi and Blynk credentials
3. Upload to ESP32
4. Power the circuit and open the Blynk app

## 📄 License

This project is open-source under the MIT License.
