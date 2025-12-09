# 🚗 Vehicle Classification using YOLOv8 and Flask

This project implements **real-time object detection and classification** (with a focus on vehicles) using **YOLOv8** and a **Flask web interface**. Users can either upload a video or use their webcam for real-time object detection powered by YOLOv8.

---

## 🔍 Features

- ⚡ Real-time object detection with YOLOv8 (Ultralytics)
- 📹 Supports video uploads for batch detection
- 🎥 Real-time webcam-based detection
- 🌐 Clean Flask web interface
- 📦 Modular code structure with live MJPEG stream

---

## 🧠 Model

We use the **YOLOv8n (nano)** model from [Ultralytics](https://github.com/ultralytics/ultralytics), ideal for fast inference with decent accuracy.

---

## 🖼️ Object Classes

The YOLOv8 model detects 80 COCO classes. Key vehicle-related classes:

- 🚗 Car
- 🚛 Truck
- 🚌 Bus
- 🏍️ Motorbike
- 🚲 Bicycle

---



---

## ⚙️ Installation
**Clone the Repository**
```bash
git clone https://github.com/Azzan/vehicle-classification-yolov8-flask.git
cd vehicle-classification-yolov8-flask
