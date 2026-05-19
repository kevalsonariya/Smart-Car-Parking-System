## 🅿️ Smart Car Parking System using Arduino

A **smart car parking system** built using Arduino UNO, IR sensors, LCD I2C display, and a servo motor. This system monitors slot availability and controls a gate barrier automatically when a vehicle enters or exits.

---

### 📽️ Demo Video

Watch the working project in action:
👉 [📂 Google Drive Link](https://drive.google.com/folderview?id=1hKYeNZJ9Guod9xetxR8_E2grsbQVN-cf)

---

### 🔧 Components Used

| Component          | Quantity | Purpose                          |
| ------------------ | -------- | -------------------------------- |
| Arduino Uno        | 1        | Main microcontroller             |
| IR Sensors         | 8        | 6 for slots, 1 for entry, 1 exit |
| Servo Motor        | 1        | Controls gate barrier            |
| 16x2 LCD with I2C  | 1        | Displays parking status          |
| Breadboard + Wires | -        | Connections                      |
| 5V 2A Adapter      | 1        | Power Supply                     |

---

### 🖥️ Features

* 🚘 Detects filled and empty parking slots in real time
* 🪪 Displays status of 6 slots on LCD (S1–S6)
* 🧠 Automatically opens/closes gate via servo motor
* 🔄 Entry only when a slot is available
* 🧾 Simulation available in Proteus

---

### 🧠 How It Works

1. Each parking slot is monitored by an IR sensor.
2. Entry and exit IR sensors track incoming/outgoing cars.
3. LCD displays:

   * Total available slots
   * Status of each individual slot
4. If a car approaches and space is available:

   * Servo opens the gate
   * Slot count decreases
5. When a car exits:

   * Servo opens again
   * Slot count increases

---

### 🔌 Circuit Diagram

![Car Parking Circuit]
<img width="1920" height="1020" alt="How to make Car Parking System using Arduino and lcd display" src="https://github.com/user-attachments/assets/1e831d74-756e-49aa-a079-26d3214c5edf" />


---

### 📁 Required Arduino Libraries

1. **Servo**

   * Already included in Arduino IDE
   * Used to control the gate motor

2. **LiquidCrystal\_I2C**

   * For I2C 16x2 LCD display
   * Install via Library Manager → Search `LiquidCrystal I2C` by Frank de Brabander or similar

---

### ⚙️ Setup Instructions

1. Connect IR sensors, servo motor, and LCD I2C module as per circuit diagram.
2. Upload `Car_Parking_System_LCD.ino` to Arduino UNO.
3. Select correct board and port in Arduino IDE:

   ```
   Tools → Board → Arduino UNO  
   Tools → Port → [Your Port]
   ```
4. Click `Upload`
5. Power the Arduino via adapter for real-time use.

---

### 📷 Proteus Simulation

You can simulate the project using **Proteus** with the file:
📄 `Proteus Simulation.pdsprj`

> Works with Proteus 8 or later.

---

### 📂 Project Folder Structure

```
📁 Smart Car Parking System
├── Car_Parking_System_LCD.ino         ← Main Arduino code
├── Proteus Simulation.pdsprj          ← Simulation file (optional)
├── How_to_make_Car_Parking_System.png ← Circuit diagram
└── README.md                          ← This file
```

---

### 🚀 Skills You Gain

* Real-time sensor-based system design
* Servo motor control logic
* I2C LCD communication
* Hands-on Proteus simulation
* Embedded system integration

---

### 💡 Future Scope

* Add IoT functionality for mobile app monitoring
* Replace IR with ultrasonic sensors for accuracy
* Add number plate recognition using camera module

---

### 🙋‍♂️ Author

**Keval Sonariya**
🔗 [LinkedIn Profile](https://www.linkedin.com/in/sonariya-keval-5b10392a5)

---

### 📬 Contact

For doubts or improvements, feel free to reach out or fork this project!

---
