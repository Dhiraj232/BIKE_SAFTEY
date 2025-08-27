# Smart Helmet using Arduino  

[![Arduino](https://img.shields.io/badge/Board-Arduino-blue?logo=arduino)](https://www.arduino.cc/)  [![Language](https://img.shields.io/badge/Language-Arduino%20C++-orange?logo=c%2B%2B)](https://www.arduino.cc/reference/en/)  [![Project](https://img.shields.io/badge/Project-CircuitDigest-green)](https://circuitdigest.com/)  

---

## 📖 Tutorial  
👉 [Smart Helmet using Arduino](https://circuitdigest.com/microcontroller-projects/smart-helmet-using-arduino)  

## 📂 Project Type  
👉 [Arduino Project](https://circuitdigest.com/arduino-projects)  

---

## 🖼️ Main Project Image  
![Smart Helmet using Arduino](https://circuitdigest.com/sites/default/files/projectimage_mic/Smart-Helmet-using-Arduino.jpg)  

---

## 🚀 Features  
- Ensures rider safety by detecting helmet usage.  
- Prevents bike ignition if the rider is not wearing a helmet.  
- Detects alcohol consumption using **MQ-3 Sensor**.  
- Wireless communication between helmet (transmitter) and bike (receiver).  
- Uses **IR Sensor** to detect helmet wearing status.  

---

## 🛠️ Hardware Requirements  

| Component                  | Quantity | Description |
|-----------------------------|----------|-------------|
| Arduino Uno                 | 2        | One for transmitter (helmet) and one for receiver (bike). |
| RF Transmitter & Receiver   | 1 pair   | Wireless communication between helmet and bike. |
| IR Sensor Module            | 1        | Detects whether helmet is being worn. |
| MQ-3 Alcohol Sensor         | 1        | Detects alcohol in the rider's breath. |
| 5V Relay Module             | 1        | Controls ignition system. |
| Connecting Wires            | As req.  | For circuit connections. |
| Power Supply (Battery)      | 2        | For transmitter and receiver sides. |

---

## ⚙️ How It Works  
1. The **IR sensor** in the helmet detects whether the rider is wearing it.  
2. The **MQ-3 sensor** checks for alcohol consumption.  
3. Both signals are sent to the **Arduino Uno (helmet side)**.  
4. If conditions are met (helmet worn, no alcohol), Arduino transmits an "OK" signal via the **RF Transmitter**.  
5. The **RF Receiver (bike side)** receives this signal.  
6. The **Arduino Uno (receiver side)** processes the signal and activates the **relay**, allowing ignition.  
7. If conditions are not met, ignition remains off.  

---

## 🔌 Circuit Connection  

### Transmitter Side  
![Smart Helmet Transmitter Circuit](https://circuitdigest.com/sites/default/files/circuitdiagram_mic/Circuit-Diagram-of-Smart-Helmet-Transmitter.png)  

| Component          | Arduino Pin |
|--------------------|-------------|
| IR Sensor Output   | D2          |
| MQ-3 Sensor Output | A0          |
| RF Transmitter     | D12         |

### Receiver Side  
![Smart Helmet Receiver Circuit](https://circuitdigest.com/sites/default/files/inlineimages/u5/Circuit-Diagram-of-Smart-Helmet-Receiver-Side.png)  

| Component        | Arduino Pin |
|------------------|-------------|
| RF Receiver Data | D11         |
| Relay IN         | D10         |

---

## 🧠 Troubleshooting  

| Issue                          | Possible Cause                | Solution |
|--------------------------------|--------------------------------|----------|
| Bike not starting even with helmet | Loose RF connection or low power | Check battery and RF modules. |
| False alcohol detection        | MQ-3 not calibrated properly   | Allow warm-up time before use. |
| IR sensor not detecting helmet | Misalignment or weak signal    | Adjust helmet placement or replace sensor. |

---

## 📱 Applications  
- Two-wheeler rider safety systems.  
- Prevents drunk driving.  
- Can be extended for smart vehicle access control.  

---

## 🔮 Future Enhancements  
- GSM/GPS integration for accident alert systems.  
- More reliable wireless communication (e.g., Bluetooth/LoRa).  
- Helmet-mounted display for alerts.  

---

## 🧪 Technical Specifications  

| Parameter                | Value |
|---------------------------|-------|
| Operating Voltage (Arduino) | 5V    |
| RF Module Frequency       | 433 MHz |
| MQ-3 Sensor Type          | Semiconductor Gas Sensor |
| Relay Voltage             | 5V    |

---

## 🔗 Links  
- Tutorial: [Smart Helmet using Arduino](https://circuitdigest.com/microcontroller-projects/smart-helmet-using-arduino)  
- IDE: [Arduino IDE](https://www.arduino.cc/en/software)  
- Datasheet: [MQ-3 Sensor Datasheet](https://www.sparkfun.com/datasheets/Sensors/MQ-3.pdf)  
- Interfacing Guides:  
  - [Arduino IR Sensor Interfacing](https://circuitdigest.com/microcontroller-projects/interfacing-ir-sensor-module-with-arduino)  
  - [Arduino MQ3 Alcohol Sensor](https://circuitdigest.com/microcontroller-projects/interfacing-mq3-alcohol-sensor-with-arduino)  

---

## ⭐ Support  
This project is published on **[CircuitDigest](https://circuitdigest.com/)**. Visit us for more DIY electronics projects, tutorials, and circuit ideas.  

---

## 🔖 Keywords  
`Smart Helmet using Arduino` `Arduino Safety Projects` `Arduino Alcohol Detection` `Helmet Ignition Lock System` `MQ3 Arduino Project` `IR Sensor Arduino Project`  
