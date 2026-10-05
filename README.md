# 🗑️ SmartBin – Arduino-Based Automatic Touchless Dustbin

SmartBin is an **Arduino-based automatic touchless dustbin** that opens and closes its lid automatically when a person brings their hand or an object near the sensor. The system uses an **HC-SR04 ultrasonic sensor** to detect distance and an **SG90 servo motor** to control the dustbin lid.

## 📌 Project Overview

Traditional dustbins require users to touch the lid manually. SmartBin provides a simple and low-cost solution by automating the lid using an ultrasonic sensor and Arduino.

When an object is detected within the predefined **20 cm range**, the Arduino activates the servo motor and opens the lid. When the object moves away, the lid closes automatically.

## ✨ Key Features

* 🖐️ Touchless operation
* 📡 Ultrasonic object detection
* 📏 Distance-based control
* ⚙️ Automatic lid opening and closing
* 🔌 Arduino-based implementation
* 💰 Low-cost and beginner-friendly design
* 🧪 Can be simulated using Tinkercad

## 🛠️ Hardware Requirements

* Arduino Uno R3
* HC-SR04 Ultrasonic Sensor
* SG90 Servo Motor
* Dustbin with movable lid
* Breadboard
* Jumper Wires
* USB Cable
* 5V Power Supply

## 💻 Software Requirements

* Arduino IDE
* Arduino C/C++
* Servo Library
* Tinkercad Circuits *(optional)*

## 🔌 Circuit Connections

| Component    | Arduino Pin |
| ------------ | ----------- |
| HC-SR04 VCC  | 5V          |
| HC-SR04 GND  | GND         |
| HC-SR04 TRIG | D9          |
| HC-SR04 ECHO | D10         |
| Servo Signal | D11         |
| Servo VCC    | 5V          |
| Servo GND    | GND         |

## ⚙️ Working Principle

The SmartBin works through the following process:

```text
Hand/Object Detected
        ↓
HC-SR04 Measures Distance
        ↓
Arduino Processes Distance
        ↓
Is Distance ≤ 20 cm?
      /       \
    YES        NO
     ↓          ↓
 Open Lid    Close Lid
     ↓          ↓
    Servo Motor
```

### Working Steps

1. The HC-SR04 sensor sends an ultrasonic signal.
2. The signal reflects from a nearby object.
3. The Arduino calculates the distance using the echo duration.
4. If the distance is **20 cm or less**, the servo rotates to approximately **90°**.
5. The lid opens automatically.
6. When the object moves away, the servo returns to approximately **0°**.
7. The lid closes automatically.


## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/SmartBin.git
```

### 2. Open the Project

Open `SmartBin.ino` using the **Arduino IDE**.

### 3. Connect the Hardware

Connect the ultrasonic sensor and servo motor according to the circuit connection table.

### 4. Select Arduino Board

In Arduino IDE:

```text
Tools → Board → Arduino Uno
```

Select the appropriate COM port.

### 5. Upload the Code

Click **Upload** in Arduino IDE.

### 6. Test the System

Open the Serial Monitor at:

```text
9600 Baud
```

Bring your hand within 20 cm of the ultrasonic sensor and observe the automatic lid operation.

## 📸 Project Demonstration

<img width="1200" height="1600" alt="WhatsApp Image 2026-10-05 at 7 37 25 PM" src="https://github.com/user-attachments/assets/c85436b6-41b6-40ff-905c-f686729293b0" />

## 📊 Expected Result

| Condition               | Output                        |
| ----------------------- | ----------------------------- |
| Object within 20 cm     | Lid opens                     |
| Object beyond 20 cm     | Lid closes                    |
| No valid sensor reading | No unnecessary servo movement |

The system successfully demonstrates automatic, touchless opening and closing of the dustbin lid.

## 🔮 Future Scope

The project can be enhanced by adding:

* Waste-level detection
* IoT-based monitoring
* Mobile notifications
* Automatic lid timing
* Waste segregation
* Solar-powered operation
* Voice-controlled features

## 🎓 Learning Outcomes

Through this project, the following concepts were learned:

* Arduino programming
* Ultrasonic sensor interfacing
* Distance measurement
* Servo motor control
* Circuit assembly
* Embedded-system automation
* Hardware and software integration

## 👩‍💻 Author

**Jasleen Kaur**

Chandigarh University
University Institute of Computing
Academic Session: 2026–2027

## 📄 License

This project is created for **educational and academic purposes**.
