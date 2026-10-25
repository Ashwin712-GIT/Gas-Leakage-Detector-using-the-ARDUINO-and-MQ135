# Gas-Leakage-Detector-using-the-ARDUINO-and-MQ135
# MQ-135 Gas Detector Using Arduino UNO

## 📌 Project Description
This project is an **MQ-135 Gas Detection System using Arduino UNO** that monitors changes in air quality using the MQ-135 gas sensor. It provides visual and audible alerts when the analog sensor reading reaches a predefined threshold.

The system uses a red LED to indicate a high sensor reading, a green LED to indicate normal readings, and a buzzer to provide an audible warning. Sensor readings and status messages are displayed in the Arduino Serial Monitor.

## 🛠️ Components Required
- Arduino UNO
- MQ-135 Gas Sensor Module
- Red LED
- Green LED
- Buzzer
- 220–330 Ω resistors for LEDs
- Breadboard
- Jumper wires
- USB cable for programming and power

## 🔌 Pin Connections

| Component | Arduino UNO Pin |
|---|---|
| MQ-135 Analog Output (AO) | A0 |
| Red LED | Digital Pin 2 |
| Green LED | Digital Pin 3 |
| Buzzer | Digital Pin 4 |
| MQ-135 VCC | 5V, if supported by the module |
| MQ-135 GND | GND |

## ⚙️ Working Principle
1. The MQ-135 sensor provides an analog reading to the Arduino through pin A0.
2. The Arduino reads the sensor value, which ranges from 0 to 1023.
3. If the reading is **400 or higher**, the red LED and buzzer turn ON, the green LED turns OFF, and a warning is printed in the Serial Monitor.
4. If the reading is below 400, the green LED turns ON, while the red LED and buzzer remain OFF.
5. The sensor reading and status are updated every second.

## 💻 Software Requirements
- Arduino IDE
- Arduino UNO board support
- USB driver appropriate for your Arduino board

## 🚀 How to Run
1. Connect the MQ-135 sensor, LEDs, and buzzer according to the pin connections.
2. Connect the Arduino UNO to your computer using a USB cable.
3. Open the Arduino IDE and paste the project code into a new sketch.
4. Select **Arduino UNO** under Tools → Board.
5. Select the correct port under Tools → Port.
6. Upload the code to the Arduino.
7. Open the Serial Monitor and set the baud rate to **9600**.
8. Observe the sensor readings and LED/buzzer responses.

## ✨ Features
- Real-time analog sensor monitoring
- Visual alerts using red and green LEDs
- Audible warning using a buzzer
- Serial Monitor output
- Adjustable sensor threshold
- Simple and beginner-friendly Arduino project

## 🔮 Future Improvements
- Add a 16×2 I2C LCD to display sensor readings and status.
- Implement a moving average to reduce fluctuations in readings.
- Add a calibrated gas concentration estimation where appropriate.
- Integrate Wi-Fi notifications using a suitable microcontroller.
- Improve alarm logic with calibration and sensor warm-up handling.

## ⚠️ Important Note
The threshold value of 400 is a configurable example and does not represent a universal gas concentration limit. The MQ-135 responds to multiple gases and air-quality changes; this basic circuit is not a certified gas-leak alarm and should not be used as the sole means of protection against hazardous gas exposure.

## 👨‍💻 Author
**Scientist Beniel's Lab**

## 📜 License
This project can be shared and modified under the terms of a license you choose. Add a `LICENSE` file to your repository if you want to specify reuse permissions.
