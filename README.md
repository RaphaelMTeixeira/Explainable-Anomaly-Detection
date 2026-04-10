# 🎥 Explainable Anomaly Detection in Surveillance Videos (Computer Vision + XAI)

## 📌 Overview
This project presents an **Explainable Artificial Intelligence (XAI) approach** for anomaly detection in surveillance videos.

Unlike traditional methods that only detect anomalies, this system:
- Detects anomalous events
- Generates **human-readable explanations**
- Describes actions using natural language

The approach is based on **atomic action recognition combined with object detection and tracking**.

---

## 🎯 Business Problem
Monitoring surveillance video streams is:
- Labor-intensive
- Error-prone
- Difficult to scale

Traditional anomaly detection systems:
- Provide only binary outputs (normal vs anomaly)
- Lack interpretability

This project aims to:
- Detect anomalies in real time
- Provide **clear explanations of what happened**
- Reduce false alarms and improve decision-making

---

## 📊 Dataset
- Custom dataset: **UTFPR-AASD (Airport Anomaly Surveillance Dataset)**
- Source: YouTube surveillance videos
- Total duration: ~33.5 minutes
- Total videos: 70
  - 45 anomalous
  - 25 normal

### Anomaly Types:
- Suspicious actions (running, jumping)
- Unusual actions (dancing, kicking)
- Violent actions (fighting, shooting)
- Fainting
- Driving/riding (bike, skateboard, etc.)

---

## 🧠 Methodology

### 1. Person Detection & Tracking
- **YOLOv3 / YOLOv4**
- **Deep SORT** for multi-object tracking

---

### 2. Action Recognition
- **SlowFast Network (ResNet-101)**
- **AIA (Asynchronous Interaction Aggregation)** model
- Pre-trained on AVA dataset

---

### 3. Soft Biometrics Extraction
- Gender detection using:
  - Face detection (YOLO-based)
  - EfficientNet model (IMDB-Wiki dataset)

---

### 4. Natural Language Description
- Template-based description system
- Example:
  > "A man is riding a bike"

- Combines:
  - Detected action
  - Object interaction
  - Person attributes

---

### 5. Anomaly Detection Logic
- Rule-based semantic analysis
- Detects anomalies based on:
  - Action type
  - Context (e.g., airport environment)

---

## 📈 Results
- **F1-Score:** ~87%
- Strong performance across anomaly classes
- Effective detection of human-object interactions

The system was able to detect ~84% of anomalies in the dataset.

---

## 🔍 Key Innovation
The main contribution of this project is:

> 🔥 **Explainable anomaly detection using natural language descriptions**

Instead of only detecting anomalies, the system explains:
- What happened
- Who performed the action
- Which objects were involved

---

## 🛠 Tools & Technologies
- Python
- TensorFlow / Keras
- OpenCV
- YOLO (object detection)
- Deep SORT (tracking)
- SlowFast + AIA (action recognition)

---

## 📍 Key Insights
- Explainability significantly improves anomaly validation
- Context-aware anomaly detection is crucial
- Combining vision + language enhances interpretability
- Real-world video conditions (lighting, resolution) remain challenging

---

## 🚀 What This Project Demonstrates
- Advanced Computer Vision
- Deep Learning for video understanding
- Explainable AI (XAI)
- Multi-model pipeline integration
- Real-world application in security systems

---

## 📎 Files
- `Explainable Anomaly Detection.pdf` → Full research paper

---

## 📬 Contact
Open to opportunities in:
**Computer Vision | AI | Machine Learning | Data Science**
