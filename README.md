# AI-Based Driver Drowsiness and Distraction Monitoring System for Road Safety

An AI-powered real-time driver monitoring system designed to improve road safety by detecting **drowsiness, yawning, gaze distraction, and head pose deviations** using computer vision techniques.
The system continuously analyzes the driver’s facial cues through a camera feed and generates alerts when unsafe driving behavior is detected.

---

## Overview

This project focuses on **real-time driver state monitoring** to reduce accident risks caused by fatigue and distraction. It uses facial landmark analysis, gaze monitoring, and alert generation to identify unsafe conditions such as prolonged eye closure, yawning, and looking away from the road.

The system is designed as a **road safety support application** and demonstrates how AI and computer vision can be applied in **automotive safety systems**.

---

## Key Features

* Real-time **driver drowsiness detection**
* **Distraction monitoring** using gaze and head movement analysis
* **Eye closure detection** using Eye Aspect Ratio (EAR)
* **Yawning detection** using Mouth Aspect Ratio (MAR)
* **Head pose / attention monitoring**
* Real-time **alert generation** for unsafe driver behavior
* Video-based analysis through webcam or input video
* Performance-oriented visual monitoring interface

---

## Technologies Used

* **Python**
* **OpenCV**
* **MediaPipe**
* **PyQt6**
* **NumPy**
* **Computer Vision**
* **Facial Landmark Detection**
* **Gaze / Driver Attention Analysis**

---

## System Workflow

1. Capture real-time video from webcam / camera
2. Detect face and extract facial landmarks
3. Compute driver monitoring metrics such as:

   * **EAR (Eye Aspect Ratio)** for eye closure detection
   * **MAR (Mouth Aspect Ratio)** for yawning detection
   * **Gaze / head orientation** for distraction monitoring
4. Evaluate fatigue and distraction conditions
5. Trigger alert if unsafe behavior is detected
6. Display real-time monitoring output

---

## Driver Monitoring Metrics

### 1. Eye Aspect Ratio (EAR)

Used to detect **eye closure and blinking behavior**.

* Helps identify prolonged eye closure associated with fatigue
* Useful for drowsiness detection in real-time monitoring

### 2. Mouth Aspect Ratio (MAR)

Used to detect **yawning activity**.

* Higher MAR values indicate frequent or prolonged yawning
* Supports fatigue assessment

### 3. Gaze / Attention Monitoring

Used to detect **driver distraction**.

* Monitors if the driver is looking away from the road
* Tracks head orientation and gaze direction for attention analysis

### 4. PERCLOS

Percentage of eye closure over a fixed time interval.

* Used as an additional fatigue indicator
* Helps assess sustained drowsiness

---

## Project Structure

```bash
AI-Based-Driver-Drowsiness-and-Distraction-Monitoring-System/
│── src/
│   ├── detection/          # Drowsiness, distraction, gaze, EAR/MAR logic
│   ├── gui/                # PyQt6 interface components
│   ├── utils/              # Helper functions and processing utilities
│   ├── models/             # Model loading / gaze estimation models
│   └── images/             # README images, screenshots, diagrams
│
│── scripts/                # Utility scripts / testing / calibration
│── examples/               # Example video analysis scripts
│── tests/                  # Test files
│── requirements.txt
│── run.py
│── README.md
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AI-Based-Driver-Drowsiness-and-Distraction-Monitoring-System.git
cd AI-Based-Driver-Drowsiness-and-Distraction-Monitoring-System
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

**Windows**

```bash
venv\Scripts\activate
```

**macOS / Linux**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Launch the real-time monitoring application

```bash
python run.py
```

### Basic usage flow

1. Connect the camera / webcam
2. Start the application
3. Position the driver’s face within the camera frame
4. Monitor real-time fatigue and distraction status
5. Stop analysis when required

---

## Video Analysis

You can also analyze recorded driver videos.

```bash
python examples/analyze_video.py --input video.mp4 --output results/
```

---

## Example Output

The system can detect and monitor:

* eye closure
* yawning
* inattentive gaze direction
* head movement / driver distraction
* fatigue alerts in real time

You can include screenshots such as:

* face landmark detection output
* gaze zone visualization
* drowsiness alert frame
* GUI monitoring screen
* performance charts / evaluation visuals

---

## Applications

This project is relevant for:

* **Automotive safety systems**
* **Driver monitoring systems (DMS)**
* **Road safety applications**
* **Smart vehicle assistance**
* **Human-machine interaction in vehicles**
* **AI-based safety monitoring solutions**

---

## Future Enhancements

* Driver identity / profile-based fatigue personalization
* Low-light / night driving optimization
* Mobile or embedded deployment
* In-vehicle audio warning system
* Cloud logging for trip-wise fatigue reports
* Integration with ADAS / smart vehicle safety systems

---

## Conclusion

The **AI-Based Driver Drowsiness and Distraction Monitoring System for Road Safety** demonstrates how computer vision can be applied to improve vehicle safety by monitoring driver alertness in real time. By combining facial landmark analysis, fatigue metrics, and distraction detection, the system acts as a practical prototype for AI-driven driver safety support in automotive environments.

---

## Author

**Durga Lalitha Sri Varshitha**
**Role:** AI Infrastructure Engineer
