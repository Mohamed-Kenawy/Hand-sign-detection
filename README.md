# ✋ Hand Sign Keyboard  
<img width="845" height="879" alt="Screenshot 2025-09-07 182547" src="https://github.com/user-attachments/assets/f896e4e5-5986-431f-a483-c8868ea8d102" />

A real-time hand sign recognition system using **PyTorch**, **Mediapipe**, and **OpenCV**.  
This project lets you **train models to recognize custom gestures** and map them to letters or words, enabling gesture-based typing and accessibility tools for deaf and hard-of-hearing communities.  

---

## 🚀 Features  
- Real-time hand tracking with Mediapipe  
- Trainable PyTorch model for sign recognition  
- Map gestures to letters, words, or actions  
- Build inclusive tools for accessibility and communication  

---

## 🛠️ Tech Stack  
- [PyTorch](https://pytorch.org/) – Deep Learning framework  
- [Mediapipe](https://developers.google.com/mediapipe) – Hand landmark detection  
- [OpenCV](https://opencv.org/) – Visualization & camera handling  

---

## 📂 Project Structure  
Hand-sign-Keyboard/
│── collect_data.py # Collect hand gesture samples
│── train.py # Train PyTorch model on collected data
│── infer_realtime.py # Real-time gesture recognition & visualization
│── data/raw/ # Saved hand sign datasets (.npy files)
│── models/ # Trained models (best_model.pt)

yaml
Copy code

---

## ⚡ Installation

Follow these steps to install and run the project on Windows.

### 1. Clone the Repository

```powershell
git clone https://github.com/Mohamed-Kenawy/Hand-sign-detection.git
cd Hand-sign-detection
```

### 2. Create a Virtual Environment

```powershell
python -m venv .venv
```

Activate the environment:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install Dependencies & Requirements

Upgrade pip and install all required libraries:

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run the Application

Launch the Streamlit application:

```powershell
streamlit run app.py
```

