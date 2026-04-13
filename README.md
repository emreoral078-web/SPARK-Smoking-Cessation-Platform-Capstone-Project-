# SparkBox: Smart Electronic Ashtray & Cessation App

This repository contains the documentation and project details for **SparkBox**, a comprehensive hardware-software ecosystem developed as the final project for the **GE 402: Innovative Design and Entrepreneurship II** course at Bilkent University. 

The initiative aims to address long-term smoking addiction by leveraging user-friendly technology and data-driven behavioral strategies.

##  Team Neocline
* **Emre Oral** (Hardware Product)
* **Ömer Koyuncu** (Hardware Product)
* **Ahmet Feyzican Güloğlu** (Hardware Product)
* **Ahmet Aybars Pektaş** (Software Product)
* **Azmi Eren Acar** (Business Development)
* **Hasan Murat Talan** (Industrial Methodologies)
* **Selin Uğur** (Corporate Identity)

##  Project Overview
SparkBox replaces manual habit tracking with an automated, discreet, and reliable system. The ecosystem consists of two main components:

1. **SparkBox (Hardware):** A compact, portable, and odor-proof electronic ashtray embedded with a laser sensor and BLE (Bluetooth Low Energy) connectivity. It automatically records the exact time and date of each cigarette disposal event.
2. **SPARK (Mobile App):** A cross-platform companion application built with React Native. It syncs with the SparkBox via BLE to help users visualize their smoking patterns, track their progress, and receive motivational support.

##  Hardware Architecture (SparkBox)
The physical device was iteratively designed for real-life usage scenarios, prioritizing battery longevity and portability:
* **Microcontroller:** ESP32 (Wi-Fi + BLE Dual-Mode)
* **Sensor:** 5mW Laser Sensor Module for disposal detection
* **Power Management:** TPS63030 Buck-Boost Converter & TP4056 Type-C Charging Module
* **Battery:** 3.7V LiPo Battery (1050 mAh) - Achieved $\ge7$ days of operation per charge.
* **Enclosure:** Custom-designed, pocket-sized ($85mm \times 60mm \times 25mm$), and odor-proof casing.

##  Software Architecture (SPARK App)
Initially prototyped in Flutter, the application was rebuilt using a more robust framework to ensure seamless cross-platform performance:
* **Framework:** React Native + Expo (TypeScript)
* **Navigation:** Expo Router + React Navigation
* **Data Security:** Expo Secure Store for encrypted local storage (GDPR/KVKK compliant)
* **Key Features:** BLE device pairing, onboarding & motivational tracking, smoking pattern visualization, and community support forums.

##  Key Accomplishments
* **Successful BLE Integration:** Established reliable data transmission between the ESP32 hardware and the React Native application.
* **Accuracy:** Reached a timestamp accuracy with only a $\pm5$ seconds deviation.
* **Design Pivot:** Successfully removed the initially planned on-device screen to offload all visual elements to the mobile app, significantly enhancing the hardware's battery life and reducing manufacturing complexity.
* **Business Ready:** Developed a comprehensive business plan, configuration control process, and branding strategy under the "Neocline" corporate identity.

##  Repository Structure
* `Team3_GE402_FinalReport.pdf`: The complete final report detailing the engineering process, business plan, organizational structure, and test results.
* *(Note: This repository serves as the public documentation for the project. Source code and CAD files are maintained internally.)*

## 🔮 Future Roadmap
* Implement full BLE data parsing and real-time history tracking in the app.
* Integrate Machine Learning to classify user smoking behavior and recommend personalized quitting strategies.
* Consolidate hardware modules into a custom-designed PCB for mass manufacturing.
