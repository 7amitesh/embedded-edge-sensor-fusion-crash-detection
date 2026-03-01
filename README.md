
# 🚗 Embedded Edge Sensor Fusion Crash Detection System

A real-time **Embedded Edge Computing Crash Detection System** that uses **sensor fusion (accelerometer + GPS + camera)** to detect vehicle crashes and trigger emergency alerts.

This project demonstrates **embedded systems design, sensor interfacing, real-time firmware logic, and edge device computing**, similar to real automotive safety systems.

---

# 📌 Overview

This system runs on an **edge device (Raspberry Pi)** and continuously monitors:

* G-force using accelerometer
* GPS location
* Camera video stream

When a crash-level impact is detected, the system:

* Records video evidence
* Captures GPS coordinates
* Sends alert to server

---

# 🧠 Key Features

* Real-time crash detection using accelerometer
* Sensor fusion combining multiple hardware inputs
* Embedded firmware logic for event triggering
* Edge computing architecture
* Real-time data acquisition
* Emergency alert pipeline

---

# 🏗 System Architecture

## High-Level Architecture

```id="k7i7v7"
         ┌────────────────────────────┐
         │     Accelerometer Sensor   │
         │        (MPU6050)          │
         └─────────────┬─────────────┘
                       │ I2C
                       ▼
         ┌────────────────────────────┐
         │      Edge Device           │
         │      Raspberry Pi         │
         │ Embedded Detection Logic  │
         └───────┬────────┬──────────┘
                 │        │
                 │        │
                 ▼        ▼
            Camera     GPS Module
           Recording    Location

                 │
                 ▼

         ┌────────────────────────────┐
         │      Alert System          │
         └────────────────────────────┘
```

---

# ⚙ Hardware Components

* Raspberry Pi
* MPU6050 Accelerometer
* GPS Module
* Camera Module
* Power Supply

---

# 💻 Software Stack

Languages:

* Python
* Embedded Linux

Protocols:

* I2C
* UART

Platform:

* Raspberry Pi OS (Linux)

---

# 📂 Project Structure

```id="gux0nl"
embedded-edge-sensor-fusion-crash-detection/

├── sensors/
│   ├── accelerometer.py
│   ├── gps_module.py
│   └── camera_buffer.py
│
├── main.py
│
├── server/
│   └── alert_service.py
│
├── docs/
│   └── architecture.png
│
└── README.md
```

---

# 🚀 How to Run

## Step 1: Clone repository

```id="0y11w8"
git clone https://github.com/7amitesh/embedded-edge-sensor-fusion-crash-detection.git
```

---

## Step 2: Navigate

```id="hj8czr"
cd embedded-edge-sensor-fusion-crash-detection
```

---

## Step 3: Run system

```id="ffivrt"
python3 main.py
```

---

# 📊 Example Output

```id="63yrnl"
Monitoring sensors...

Impact detected: 8.5g

Recording video...

Sending alert with GPS location...
```

---

# 🧪 Embedded Concepts Demonstrated

This project demonstrates:

* Embedded systems programming
* Sensor interfacing
* Edge computing
* Hardware communication
* Firmware-style event detection
* Real-time systems

---

# 🚗 Real-World Applications

Automotive safety systems
Crash detection systems
Fleet monitoring
Smart vehicles

---

# 🚀 Future Improvements

* Implement firmware in Embedded C
* Add CAN bus support
* Add real-time dashboard
* Optimize for low power

---

# 👤 Author

Amitesh Kumar

GitHub:
[https://github.com/7amitesh](https://github.com/7amitesh)

Portfolio:
[https://amiteshportfolio.framer.website/](https://amiteshportfolio.framer.website/)

---

# ⭐ Why this project matters

This project demonstrates skills required for:

Embedded Software Engineer
Firmware Engineer
SoC Engineer



