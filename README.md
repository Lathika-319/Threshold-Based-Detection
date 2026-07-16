# 🚨 Threshold-Based Detection for Chain Snatching

A deep learning project developed during the UpToSkills Internship that identifies potential chain snatching events from CCTV videos using a CNN-based threshold detection approach, YOLO object detection, and motion analysis.

---

## 📖 Project Overview

This project implements a threshold-based detection pipeline for identifying chain snatching events in surveillance videos. Video frames are processed using OpenCV, classified with a Convolutional Neural Network (CNN), and verified using a confidence threshold. YOLO is used to detect people in each frame, while speed estimation and CSV logging provide additional event analysis.

The complete implementation was developed and tested using Kaggle Notebook.

---

## 🎯 Objectives

- Detect possible chain snatching events from CCTV footage.
- Classify video frames using a CNN model.
- Apply a confidence threshold to reduce false detections.
- Detect people using YOLO object detection.
- Record predictions for further analysis.

---

## 📂 Dataset

The project uses CCTV video frames collected for chain snatching detection experiments.
The dataset used for this project is publicly available on Kaggle.

Dataset Link: (https://www.kaggle.com/code/lathika04/chain-snaching-project?select=Chain_Snatching_Videos),https://www.kaggle.com/code/lathika04/chain-snaching-project,https://www.kaggle.com/code/lathika04/chain-snaching-project,https://www.kaggle.com/code/lathika04/chain-snaching-project,https://www.kaggle.com/code/lathika04/chain-snaching-project,https://www.kaggle.com/code/lathika04/chain-snaching-project,https://www.kaggle.com/code/lathika04/chain-snaching-project


> Due to the dataset size, it is not included in this repository.

---

## 🧹 Methodology

### 1️⃣ Frame Extraction
- Read CCTV videos frame by frame using OpenCV.
- Resize each frame to **128 × 128 pixels**.
- Normalize pixel values before prediction.

### 2️⃣ CNN Model Training
- Build a 3-layer Convolutional Neural Network.
- Train using TensorFlow/Keras.
- Optimize using the Adam optimizer.

### 3️⃣ Threshold-Based Detection
- Predict the confidence score for every frame.
- If the confidence is **0.65 or above**, classify the frame as a chain snatching event.

### 4️⃣ YOLO Object Detection
- Detect people in every frame.
- Draw bounding boxes around detected persons.

### 5️⃣ CSV Event Logging
- Store frame number, prediction, confidence score, and timestamp.

### 6️⃣ Speed Verification
- Calculate centroid movement between consecutive frames.
- Use motion speed as an additional verification step.

---

## 💻 Features

- 🎥 CCTV Video Processing
- 🖼️ Frame Extraction
- 🧠 CNN-Based Classification
- 📊 Threshold Decision Making
- 👤 YOLO Person Detection
- 📈 Confidence Score Prediction
- 🚶 Motion Speed Analysis
- 📄 CSV Event Logging
- 🎬 Annotated Output Video

---

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- YOLO
- NumPy
- Pandas
- Matplotlib
- Kaggle Notebook

---

## 📁 Repository Structure

```
Threshold-Based-Detection/
│
├── README.md
├── LICENSE
├── chain-snaching-project.ipynb
├── Image.png
└── output_video.mp4 (Demo)
```

---

## ▶️ How to Run

1. Clone the repository

```bash
git clone https://github.com/Lathika-319/Threshold-Based-Detection.git
```

2. Install the required libraries

```bash
pip install -r requirements.txt
```

3. Open the notebook in Kaggle or Jupyter Notebook.

4. Run all notebook cells.

---


## 🔗 Kaggle Notebook

The complete implementation is available on Kaggle:

https://www.kaggle.com/code/lathika04/chain-snaching-project

---

## 🚀 Future Enhancements

- Improve CNN accuracy using a larger dataset.
- Integrate real-time CCTV monitoring.
- Support multi-camera surveillance.
- Reduce false positives using temporal analysis.
- Deploy as a web application.

---

## 👩‍💻 Author

**Lathika S**

B.E. Computer Science and Engineering

UpToSkills Internship Project
