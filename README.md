# Face Recognition Attendance System

A Python-based face recognition attendance system that detects and recognizes registered faces and records attendance automatically.

## 📌 Project Overview

This project uses **Python, OpenCV, Haar Cascade, NumPy, and Keras** to build a face recognition-based attendance system.

The system can:

* Detect faces using Haar Cascade
* Recognize registered users using a trained deep learning model
* Display the recognized person's name
* Record entry and exit information
* Save attendance information in CSV format

## 🛠️ Technologies Used

* Python
* OpenCV
* NumPy
* Keras / TensorFlow
* Haar Cascade
* CSV
* Git & GitHub

## 📂 Project Files

| File                                      | Description                                          |
| ----------------------------------------- | ---------------------------------------------------- |
| `collect_data (1).py`                     | Captures face images for registered users            |
| `consolidated_data (1).py`                | Prepares collected images and labels                 |
| `recognize (2).py`                        | Performs real-time face recognition                  |
| `attendance system (1).py`                | Runs the attendance system                           |
| `haarcascade_frontalface_default (1).xml` | Haar Cascade face detection classifier               |
| `.gitignore`                              | Prevents private/generated files from being uploaded |

## 🔄 How It Works

```text
Face Image
     ↓
Face Detection
     ↓
Image Preprocessing
     ↓
Trained ML Model
     ↓
Face Recognition
     ↓
Person Name
     ↓
Attendance Recording
```

## 🧠 Face Recognition Process

### 1. Face Detection

The system uses OpenCV's Haar Cascade classifier to detect faces from the camera.

### 2. Preprocessing

The detected face is:

* Converted to grayscale
* Resized to `100 × 100`
* Histogram equalized
* Normalized

### 3. Recognition

The processed face is passed to the trained Keras model.

The model predicts the corresponding class, and `argmax()` selects the class with the highest prediction value.

### 4. Attendance

After recognition, the person's name and attendance information are recorded.

## ▶️ How to Run

### Step 1 — Install Python

Python 3.12 is recommended for this project.

### Step 2 — Install dependencies

```bash
pip install opencv-python==4.10.0.84
pip install numpy
pip install tensorflow
pip install keras
```

### Step 3 — Collect face data

Run:

```bash
python "collect_data (1).py"
```

### Step 4 — Prepare the data

Run:

```bash
python "consolidated_data (1).py"
```

### Step 5 — Run face recognition

Run:

```bash
python "recognize (2).py"
```

### Step 6 — Run attendance system

Run:

```bash
python "attendance system (1).py"
```

## ⚠️ Important Note

This repository does not include collected face images, attendance records, or the trained model file because these files may contain sensitive or generated data.

## 🚀 Future Improvements

* Add a web-based interface
* Add a database instead of CSV storage
* Add admin login
* Add student registration through the interface
* Add attendance dashboard
* Add email notifications
* Improve recognition accuracy
* Deploy the system as a web application

## 👩‍💻 Author

**Dharitree Devi**

GitHub: `dharitree-devi`
