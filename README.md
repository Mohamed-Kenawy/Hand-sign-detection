#  Hand Sign Keyboard  
<img width="845" height="879" alt="Screenshot 2025-09-07 182547" src="https://github.com/user-attachments/assets/f896e4e5-5986-431f-a483-c8868ea8d102" />

# ✋ Hand Sign Recognition

A real-time Hand Sign Recognition system built using **Python, PyTorch, MediaPipe, and OpenCV**.

The project uses computer vision and deep learning to recognize hand gestures through a webcam. It extracts hand landmarks, trains a neural network to classify gestures, and performs real-time predictions.

## 🚀 Features

- **Real-Time Hand Tracking:** Detects and tracks hand landmarks using MediaPipe.
- **Hand Landmark Extraction:** Extracts 21 hand landmarks (63 coordinate values).
- **Deep Learning Model:** Uses a PyTorch Multi-Layer Perceptron (MLP) for gesture classification.
- **Custom Dataset Collection:** Collects and saves hand gesture samples using a webcam.
- **Model Training:** Trains a custom model using the collected dataset.
- **Live Recognition:** Predicts hand gestures in real time using OpenCV.
- **Customizable Gestures:** Supports training with your own collected hand gesture samples.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| PyTorch | Deep learning and model training |
| MediaPipe | Hand detection and landmark extraction |
| OpenCV | Webcam access and image processing |
| NumPy | Numerical operations and data handling |
| Jupyter Notebook | Development and experimentation |

## 📂 Project Structure

```text
Hand-sign-detection/
│
├── data/
│   └── raw/                  # Collected hand gesture datasets
│
├── models/
│   └── best_model.pt         # Trained model weights
│
├── collect_data.ipynb        # Collect hand gesture samples
├── train.ipynb               # Train the recognition model
├── realtime.ipynb            # Real-time gesture recognition
│
├── requirements.txt          # Project dependencies
└── README.md
```

## ⚡ Installation

Follow these steps to install and run the project on **Windows**.

### 1. Clone the Repository

Open PowerShell or Command Prompt:

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

If PowerShell blocks script execution, run:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy RemoteSigned
```

Then activate the environment again.

### 3. Install Dependencies & Requirements

Upgrade pip:

```powershell
python -m pip install --upgrade pip
```

Install the required packages:

```powershell
pip install -r requirements.txt
```

### Requirements

- Windows 10 or Windows 11
- Python 3.11
- Webcam
- Internet connection for initial dependency installation
- The Python libraries listed in `requirements.txt`

## 📖 Usage

The project workflow consists of three main steps.

### 1. Collect Hand Gesture Data

Open `collect_data.ipynb` in Jupyter Notebook.

Run the notebook cells to:

- Initialize the webcam.
- Detect the hand using MediaPipe.
- Extract hand landmarks.
- Collect gesture samples.
- Save the collected data inside `data/raw/`.

Make sure your hand is clearly visible to the webcam while collecting samples.

### 2. Train the Model

Open `train.ipynb` and execute the cells.

The training process:

- Loads the collected dataset.
- Prepares the landmark features and labels.
- Trains the PyTorch neural network.
- Evaluates the model.
- Saves the trained model weights in the `models/` directory.

### 3. Real-Time Hand Sign Recognition

Open `realtime.ipynb` and execute the cells.

The system will:

- Access your webcam.
- Detect your hand using MediaPipe.
- Extract the hand landmarks.
- Pass the extracted features to the trained PyTorch model.
- Display the predicted hand sign in real time.




