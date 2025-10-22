# 🔌 IoT-Based 5V Relay Control Module (ESP32 WiFi Controlled)

A compact, two-layer **Printed Circuit Board (PCB)** design for a 5-channel relay control module, powered by the **ESP32** for seamless **Internet of Things (IoT)** integration. This project enables remote control and automation of up to five independent AC loads via a WiFi network.

## ✨ Features

* **5-Channel Control:** Individually control up to five AC devices using **HK4100F-5V** relays.
* **ESP32 Integration:** Utilizes the powerful ESP32 module for WiFi connectivity and core logic.
* **Integrated Power Supply:** Incorporates the **HLK-PM05** power module to step down 220V AC to the required 5V and 3.3V DC supplies.
* **Two-Layer PCB:** Designed in **Altium Designer** for a compact **115.444 mm x 50.546 mm** footprint.
* **Safety and Isolation:** Features intentional layout for **AC-DC isolation** and optimized grounding to minimize electrical interference and enhance operational safety.
* **Transistor Switching:** Uses **2N3904/MMBT3904 NPN** transistors to drive the relay coils from the ESP32's 3.3V logic signals.

---

## 🏗️ Design and Architecture

### Key Components

| Component | Function | Notes |
| :--- | :--- | :--- |
| **ESP32 Module** | WiFi connectivity & Microcontroller | Core control logic. |
| **HLK-PM05** | Power Supply (AC-DC) | Converts 220V AC to 5V DC. |
| **HK4100F-5V** | 5V DC Relay | Switches the AC loads. |
| **2N3904/MMBT3904** | NPN Transistor | Drives the relay coil from the ESP32's 3.3V logic. |
| **Barrier Block Connector** | AC and Load Connections | Provides secure, high-current connection points. |

### PCB Layout Highlights

* **Compact Design:** Achieved efficient routing on a two-layer board, fitting all components within a limited space.
* **Isolation:** A clear, intentional separation is maintained between the high-voltage **AC LIVE** sections and the low-voltage **DC/Digital** control circuitry to prevent interference and ensure safety.
* **Grounding:** Separate nets for **AC GND** and **DC GND/Circuit GND** are used, connecting only at a single, appropriate point to prevent ground loops.

---

## ⚙️ Hardware Schematic and PCB Files

The full project repository includes:

* **`Schematic_Files/`:** Altium schematic source files.
* **`PCB_Layout/`:** Altium PCB source files, including the Gerber files for manufacturing.
* **`Bill_of_Materials.xlsx`:** A comprehensive list of all required components.

---

## 💻 Firmware (Coming Soon)

The firmware will be developed to:

* Establish a WiFi connection.
* Host a web server or connect to an MQTT broker for remote command reception.
* Map incoming commands to the appropriate ESP32 GPIO pins to toggle the relays.
* Provide status feedback (e.g., current relay state).

---

## 👨‍💻 Developed By

**Abad-ur-Rehman** (2021-EE-91)
* **Institution:** UET Lahore (Makers Lab)
