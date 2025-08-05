# 🚗 Smart Vehicle Detector — YOLO + VLM-Powered Vehicle Analysis

This project combines real-time **vehicle detection** using YOLOv12 with intelligent analysis powered by a **Vision Language Model (VLM)** such as gemini-2.5-flash-lite. The system not only detects vehicles in a video stream but also identifies their **type**, **color**, and **manufacturer**, with improved accuracy by automatically estimating the **country context**.

---

## 🎥 Project Demo

> Below is a quick demo of the system in action:

![Demo](smart_vehicle_detector-demo.gif)
---

## 🚀 Features

- Real-time detection of cars, trucks, buses, motorcycles, and bicycles using YOLO.
- Persistent object tracking via unique track IDs.
- Automatic vehicle cropping from the original (clean) frame.
- VLM-based analysis to extract:
  - Vehicle type (e.g., car, bus, truck)
  - Dominant color (e.g., red, black, white)
  - Manufacturer (e.g., Toyota, BMW, Ford)
- Initial country detection from the first frame to adapt vehicle analysis based on geographical context.
- Clean and structured JSON output of all results.

---

## 📦 Requirements

- Python 3.8+
- OpenRouter or OpenAI-compatible API key
- CUDA-enabled GPU recommended for YOLO acceleration

---

## ⚙️ Installation

1. **Clone the repository:**

```bash
git https://github.com/Y1D1R/smart-vehicle-detector.git
cd smart-vehicle-detector
