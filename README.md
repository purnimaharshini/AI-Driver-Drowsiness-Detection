# Driver-Drowsiness-Detection 🚗💤

The **Driver Drowsiness Detection System** is a computer vision–based safety application designed to detect driver fatigue in real time using a webcam. It leverages facial landmark detection and eye tracking to compute the **Eye Aspect Ratio (EAR)**, which helps identify prolonged eye closure — a key indicator of drowsiness.

This system alerts the driver using sound alarms and optional SMS notifications, thereby reducing the risk of road accidents caused by fatigue.

---

## 📌 Features

- Real-time face and eye detection using a webcam
- Eye Aspect Ratio (EAR)–based drowsiness detection
- Visual alerts on the screen
- Audio alarm to wake the driver
- SMS alert support (Twilio integration)
- Fullscreen monitoring interface

---

## 🧠 How It Works

- **dlib** detects facial landmarks
- **imutils** simplifies video frame processing
- **scipy** calculates Euclidean distances between eye landmarks
- **OpenCV** handles image and video processing
- **EAR (Eye Aspect Ratio)** determines eye closure duration
- Alerts are triggered when EAR falls below a threshold for consecutive frames

---

## 🛠 Prerequisites

### 1️⃣ Python Version
- Python **3.x** is required

### 2️⃣ Facial Landmarks File
Download the facial landmark predictor file:

**Dataset Download Link:**  
https://sourceforge.net/projects/dclib/files/dlib/v18.10/shape_predictor_68_face_landmarks.dat.bz2/download

➡ Extract the file and place it in your project directory.

### 3️⃣ Required Libraries
The project uses the following Python libraries:

- `dlib`
- `imutils`
- `scipy`
- `opencv-python`
- `numpy`
- `pygame`
- `twilio`

All dependencies are listed in the `requirements.txt` file.

---

## ⚙️ Installation

Install the required libraries using:

```bash
python -m pip install -r requirements.txt

 ▶️ Execution

Run the main Python script:
python Driver_Drowsiness_Detection.py
```
## 📷 The system will:

- Access your webcam

- Detect facial landmarks

- Monitor eye movements

- Trigger alerts when drowsiness is detected

Press q to exit the application.
## 🚨 Alerts

**Initial Alerts**: Siren sound when drowsiness is detected

**Repeated Alerts**: Continuous music to keep the driver awake

**Critical Alert**: SMS notification sent after multiple detections

## 🧪 Troubleshooting
- Webcam Issues

- Ensure your webcam is properly connected

- Check if OpenCV can access the camera

- dlib Installation Issues

- Make sure C++ build tools are installed

- Refer to official dlib installation documentation

## 📝 Notes

- The shape_predictor_68_face_landmarks.dat file is essential for accurate detection

- Ensure the file path is correctly set in the Python script

- For SMS alerts, configure valid Twilio credentials

## 📌 Future Enhancements

- Mobile app integration

- Head pose and yawning detection

- Cloud-based alert monitoring

- Driver behavior analytics

## 👨‍💻 Author

Developed as a Computer Vision & Safety Project to enhance road safety and reduce accidents caused by driver fatigue.
