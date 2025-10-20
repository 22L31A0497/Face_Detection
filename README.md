## 🧠 **Face Detection Using OpenCV**

### 📘 Overview

The **Face Detection** project uses **OpenCV** and **MediaPipe** to detect and mark faces in real-time using a webcam feed.
It leverages machine learning–based detection algorithms to identify facial regions efficiently, providing bounding boxes around each detected face.
This serves as a foundational step for applications like face recognition, emotion detection, or access control systems.

---

### ⚙️ Tech Stack

* **Python 3.x**
* **OpenCV** – for video capture and image processing
* **MediaPipe** – for advanced face landmark detection
* **NumPy** – for mathematical operations

---

### 🚀 Features

* Real-time face detection via webcam
* Detects multiple faces in a single frame
* Displays bounding boxes around detected faces
* Shows frame rate (FPS) for performance tracking
* Easy-to-integrate and extend for advanced use cases

---

### 🧩 Working Principle

1. The webcam captures continuous video frames.
2. Each frame is converted from **BGR → RGB** (as required by MediaPipe).
3. MediaPipe’s face detection model processes the RGB frame.
4. For each detected face, a bounding box is drawn using OpenCV’s rectangle method.
5. FPS (Frames Per Second) is calculated to display performance on the frame.

---

### 📦 Installation

```bash
pip install opencv-python mediapipe numpy
```

---

### ▶️ How to Run

```bash
python faceDetection.py
```

---

### 🖼️ Output Example

* The webcam window displays your live feed.
* Faces are marked with green rectangles.
* FPS count is shown on top-left of the screen.

---

### 🔍 Code Flow Summary

1. Initialize webcam (`cv2.VideoCapture(0)`)
2. Use a `FaceDetector` class to process each frame
3. Convert frame → RGB → detect → draw boxes
4. Display processed video output

---

### 💡 Future Enhancements

* Add face recognition (using Haar cascades or DeepFace)
* Integrate emotion or age-gender detection
* Create attendance systems or access control modules

---
