# Facial Expression Recognition 🎭

This project implements a **real-time facial expression recognition system** using deep learning. Built with **TensorFlow, Keras, and OpenCV**, the system detects human faces from a webcam feed and classifies them into one of **seven basic emotions**.

---

## 🔍 Overview

- **Input:** Live webcam feed or FER-2013 dataset images  
- **Output:** Detected face annotated with one of the following emotions:
  - Angry
  - Disgusted
  - Fearful
  - Happy
  - Neutral
  - Sad
  - Surprised
- **Model Architecture:** Custom CNN (similar to VGG-like structure)  
- **Frameworks:** TensorFlow, Keras, OpenCV

---

## 📁 Project Structure
Download data/ folder from FER-13 Dataset to your project folder

Facial_Expression_Recognition/

├── data/ # Dataset directory (FER-2013 format)

  │ ├── train/ # Training images (by emotion)

  │ └── test/ # Validation images (by emotion)

├── haarcascade_frontalface_default.xml # Face detector XML (OpenCV)

├── kerasmodel.py                       # Main script (training/display modes)

├── model.h5                            # Trained model weights (generated after training)

├── graphs.png                          # Accuracy/Loss plot (generated after training)

├── README.md                           # This file

├── requirements.txt                    # Modules required for this project with versions



---

## 🚀 Getting Started

### 1. Clone the repository
bash

git clone https://github.com/itzme-deekshith/Facial-Expression-Recognition.

cd Facial-Expression-Recognition.

---
### 2. Create and activate a virtual environment
- python -m venv tfenv
#### On Windows
- tfenv\Scripts\activate
#### On macOS/Linux
- source tfenv/bin/activate
---
### 3. Install dependencies
- pip install -r requirements.txt
---
### 4. Train the model
- python kerasmodel.py --mode train

---
### 5. Run real-time emotion detection
- python kerasmodel.py --mode display
