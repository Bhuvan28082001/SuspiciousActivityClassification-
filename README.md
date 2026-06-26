# 🚨 Suspicious Activity Classification Using Deep Learning

A Machine Learning and Computer Vision project that automatically classifies surveillance images into **Violence** and **Non-Violence** categories using Deep Learning models. This project compares a Custom CNN, ResNet50, and MobileNetV2 to identify the best model for real-time surveillance applications.

---

## 📌 Project Overview

Public surveillance systems generate massive amounts of visual data every day. Continuous manual monitoring is inefficient and often results in missed incidents due to human fatigue.

This project proposes an AI-based solution that automatically detects suspicious violent activities from surveillance images, enabling faster incident detection and improved public safety.

---

## 🎯 Objectives

- Develop an automated violence detection system using Deep Learning.
- Compare the performance of:
  - Custom CNN
  - ResNet50 (Transfer Learning)
  - MobileNetV2 (Transfer Learning)
- Evaluate models using multiple performance metrics.
- Identify the best model for real-time deployment.

---

## 📂 Dataset

**Dataset:** Real Life Violence Situations Dataset

- Total Images: **11,073**
- Violence Images: **5,842**
- Non-Violence Images: **5,231**

Dataset contains real-world surveillance scenes with different lighting conditions, backgrounds, and camera angles.

---

## 🛠️ Data Preprocessing

The following preprocessing techniques were applied:

- Image resizing (224 × 224)
- RGB image processing
- Pixel normalization (0–1)
- Data augmentation
  - Rotation (20°)
  - Zoom (0.2)
  - Horizontal Flip
- Train/Validation Split (80:20)

---

## 🧠 Models Implemented

### 1. Custom CNN
- Three Convolutional Layers
- Max Pooling
- Dense Layer
- Dropout
- Sigmoid Output

---

### 2. ResNet50 (Transfer Learning)

- ImageNet Pretrained
- Frozen Base Layers
- Global Average Pooling
- Dense Layer
- Dropout

---

### 3. MobileNetV2 (Transfer Learning)

- ImageNet Pretrained
- Lightweight Architecture
- Depthwise Separable Convolutions
- Global Average Pooling
- Dense Layer
- Dropout

---

# 📊 Model Performance

| Model | Validation Accuracy | Validation Loss |
|--------|--------------------:|----------------:|
| Custom CNN | 73.49% | 0.556 |
| ResNet50 | 54.07% | 0.671 |
| **MobileNetV2** | **88.03%** | **0.269** |

### 🏆 Best Model

**MobileNetV2**

- Validation Accuracy: **88.03%**
- Model Size: **9.24 MB**
- Trainable Parameters: **164K**

Suitable for deployment on edge devices.

---

# 📈 Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Training Loss
- Validation Loss

---

# 📸 Sample Prediction

The trained MobileNetV2 model successfully classifies unseen surveillance images as:

- Violence
- Non-Violence

with high confidence.

Example Output:

```
Prediction : Violence
Confidence : 94%
```

---

# 💻 Technologies Used

- Python
- TensorFlow 2.x
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-Learn
- Kaggle Notebook
- Google Colab

---

# 📁 Repository Structure

```
SuspiciousActivityClassification/

│── README.md
│── requirements.txt
│── notebook.ipynb
│
├── models/
│     mobilenet_violence_model.h5
│
├── results/
│     accuracy_curve.png
│     loss_curve.png
│     confusion_matrix.png
│
├── presentation/
│     ML_Phase_III_Presentation.pptx
│
├── report/
│     Final_Report.pdf
│
└── demo/
      Demo_Video.mp4
```

---

# 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/Bhuvan28082001/SuspiciousActivityClassification-.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

Open

```
notebook.ipynb
```

using

- Kaggle
- Google Colab
- Jupyter Notebook

Train the models and execute the prediction cell.

---

# 🌍 Applications

- Smart City Surveillance
- Airport Security
- Railway Stations
- Shopping Malls
- Schools & Universities
- Public Safety Monitoring
- Traffic Surveillance

---

# ⚠️ Limitations

- Image-based classification only
- Single dataset used
- No temporal video analysis
- No Explainable AI (Grad-CAM)

---

# 🔮 Future Work

- Video-based Violence Detection
- LSTM / Transformer Integration
- Explainable AI (Grad-CAM)
- Raspberry Pi Deployment
- Jetson Nano Deployment
- Model Quantization
- Real-time CCTV Integration

---

# 👨‍💻 Author

**Bhuvan Chandra**

Master's in Data Science

University of Europe for Applied Sciences

Berlin, Germany

GitHub:
https://github.com/Bhuvan28082001

---

# ⭐ Acknowledgements

- University of Europe for Applied Sciences
- Kaggle
- TensorFlow
- Keras
- OpenCV

---

## ⭐ If you found this project useful, please consider giving it a Star.
