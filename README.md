# Waste Segregation Monitoring System
### Smart India Hackathon 2025 — Hardware Domain | PS #14 | Clean & Green Technology
**Team:** Ai-migos (Team ID: 88246) | **Role:** Team Leader | **Status:** SIH 2025 Finalist

---

## Problem Statement
Urban Local Bodies (ULBs) struggle with manual waste segregation — a process that is slow, inaccurate, and exposes sanitation workers to hazardous material. There was no automated, affordable system to classify and sort waste at the source in real time.

## Our Solution
An AI-powered automated waste segregation system that uses **Computer Vision** and a **custom-trained Machine Learning model** to classify waste in real time and physically sort it using a hardware conveyor-servo system — all controlled via a companion Android app.

---

## How It Works

```
Waste placed on conveyor belt
        ↓
USB Camera captures image
        ↓
ML Model classifies waste category
(E-waste / Plastic / Metal / Glass / Organic)
        ↓
ESP32 receives classification signal via Bluetooth
        ↓
Servo motor rotates to correct bin
        ↓
DC motor advances conveyor belt for next item
```

---

## Tech Stack

### Software
| Component | Technology |
|-----------|-----------|
| ML Model | Python, Custom-trained image classifier |
| Computer Vision | OpenCV |
| Android App | MIT App Inventor |
| App-Hardware Interface | Bluetooth (via MIT App Inventor WebViewer) |
| Model Training | Python, image dataset (manually collected & labelled) |

### Hardware
| Component | Purpose |
|-----------|---------|
| ESP32 Microcontroller | Brain of the hardware system; receives classification and controls actuators |
| Servo Motor | Rotates diverter gate to route waste into correct bin |
| DC Motor | Drives the conveyor belt |
| USB Camera | Captures real-time images of waste items for classification |
| Battery Module | Powers the full hardware stack |
| Conveyor Belt (custom) | Transports waste items past the camera and to sorting bins |

---

## Waste Categories Supported
- E-waste (batteries, circuit boards)
- Plastic
- Metal
- Glass
- Organic

---

## Key Features
- **Real-time classification** — waste is identified and sorted in seconds
- **Custom-trained ML model** — trained on a self-collected and labelled image dataset
- **Android app control** — start/stop conveyor, view live classification via Bluetooth
- **Low-cost hardware** — built entirely with accessible, off-the-shelf components
- **Scalable** — additional servo motors can extend support to more waste categories

---

## Impact
- Reduces human exposure to hazardous waste
- Enables accurate waste segregation at source
- Supports municipal recycling and sustainability goals
- Lowers long-term operational costs for Urban Local Bodies

---

## Project Gallery
> *Demo video and hardware photos available on request.*

---

## Team — Ai-migos
| Name | Role |
|------|------|
| Apoorva Prashant Kulkarni | Team Leader, Hardware Integration, ESP32 Programming |
| *(Team members)* | ML Model, Android App, Mechanical Assembly |

**Institution:** Modern College of Engineering, PES — Pune
**Event:** Smart India Hackathon 2025 | Result: **National Finalist**

---

## Note on Code
This was a hardware-first project developed and deployed directly onto embedded devices (ESP32) and Android (MIT App Inventor APK) during the SIH hackathon. The full source was developed collaboratively on-site. This repository serves as the official project documentation.

---

> *Built with curiosity, caffeine, and a conveyor belt.*
