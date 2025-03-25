# EXAMEYE

## 📌 Overview
**EXAMEYE** is an AI-powered offline cheating detection system for exams using **YOLO-based object and behavior recognition**.

## 🚀 Features
- 🎥 **Real-Time Monitoring**: Detects cheating actions like **mobile usage**, **hand signals**, and **unauthorized movement**.
- 📹 **Video Analysis**: Processes recorded exam sessions to flag suspicious behavior.
- 🏆 **Custom Model Training**: Supports **YOLO-NAS** and **YOLOv8** for enhanced detection accuracy.

## ⚙️ Installation
```bash
pip install -r requirements.txt
```

## 🔹 Usage Guide

### 1️⃣ **Run Real-Time Exam Monitoring**
```bash
python main.py
```

### 2️⃣ **Analyze a Recorded Exam Video**
```bash
python detect_cheating.py --video input_video.mp4
```

### 3️⃣ **Train YOLO-NAS for Object Detection**
```bash
python train.py --model yolonas --dataset data/cheating_dataset
```

### 4️⃣ **Train YOLOv8 for Behavioral Analysis**
```bash
python train.py --model yolov8 --dataset data/behavior_dataset
```

### 5️⃣ **View Example Detections**
- **Cheating Detected (Mobile Usage)** 📷 `images/example_cheating.png`
- **Suspicious Behavior (Hand Movements)** 📷 `images/example_movement.png`

## 📜 License
This project is licensed under the **MIT License**.

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss.

---
🔗 **GitHub Repo**: [[https://github.com/VortexQuasarX)]
