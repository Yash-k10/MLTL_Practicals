# 🧍 Pose Detection using PoseNet (TensorFlow.js)

## 👤 Author

**Yash Kapse**

---

## 📌 Project Overview

This project demonstrates real-time human pose detection using the PoseNet model in TensorFlow.js. It uses a webcam feed to identify human body keypoints, draw skeleton structures, classify posture, count exercise repetitions (squats), and compare single-pose vs multi-pose detection.

---

## 🎯 Objectives

* Detect human body keypoints using a pre-trained PoseNet model
* Visualize keypoints and skeleton structure on live webcam feed
* Classify posture (Standing / Sitting)
* Count repetitions of a simple exercise (Squats) using joint angles
* Compare performance between single-pose and multi-pose detection

---

## ⚙️ Technologies Used

* HTML, CSS, JavaScript
* TensorFlow.js
* PoseNet (Pre-trained model)
* jsDelivr CDN

---

## 📷 Features

### 1️⃣ Pose Detection

* Detects 17 body keypoints (nose, shoulders, hips, knees, etc.)
* Displays keypoints (red dots) and skeleton (green lines)

### 2️⃣ Posture Detection

* Classifies posture based on relative positions of nose and hips
* Outputs: **Standing / Sitting**

### 3️⃣ Squat Counter

* Uses joint angle calculation (hip, knee, ankle)
* Detects squat movement and counts repetitions
* Real-time counter display

### 4️⃣ Single vs Multi Pose Detection

* Single Pose → detects one person (faster)
* Multi Pose → detects multiple people (slower but more flexible)
* Console logs show confidence and number of detected persons

---

## 🧠 Methodology

### Step 1: Webcam Setup

* Access webcam using `getUserMedia()`
* Stream video to HTML `<video>` element

### Step 2: Model Loading

* Load PoseNet model using TensorFlow.js CDN

### Step 3: Pose Estimation

* Use:

  * `estimateSinglePose()` for single person
  * `estimateMultiplePoses()` for multiple people

### Step 4: Visualization

* Draw keypoints using canvas
* Connect keypoints to form skeleton

### Step 5: Angle Calculation (Squat Detection)

* Compute angle using three points:
  Hip → Knee → Ankle
* Apply threshold logic to detect squat

### Step 6: Output

* Display posture on screen
* Log results in console
* Count repetitions dynamically

---

## 📊 Results

* Successfully detected body keypoints in real-time
* Skeleton structure accurately mapped to human body
* Posture classification worked with good accuracy
* Squat counter correctly counted repetitions
* Multi-pose detection identified multiple people

---

## ⚖️ Comparison

| Feature          | Single Pose   | Multi Pose       |
| ---------------- | ------------- | ---------------- |
| Speed            | Fast ⚡        | Slower 🐢        |
| Persons Detected | One           | Multiple         |
| Accuracy         | High (single) | Better in groups |

---

## 🚀 How to Run

### Step 1: Save File

Save the HTML code as:

```
index.html
```

### Step 2: Run on Local Server

Use one of the following:

**Option 1 (VS Code Live Server)**

* Right click → Open with Live Server

**Option 2 (Python Server)**

```
python -m http.server
```

### Step 3: Open in Browser

```
http://localhost:8000
```

---

## ⚠️ Important Notes

* Webcam permission must be allowed
* Do not run using `file://` (camera will not work)
* Good lighting improves accuracy

---

## 🔮 Future Improvements

* Angle-based posture correction system
* Exercise detection (push-ups, jumping jacks)
* AI fitness trainer
* Data logging and analytics dashboard

---

## ✅ Conclusion

This project successfully demonstrates the use of PoseNet for real-time human pose detection. It highlights how machine learning models can be applied in browser-based applications for posture analysis, fitness tracking, and multi-person detection.

---

## 📚 References

* TensorFlow.js Documentation
* PoseNet Model by Google
* jsDelivr CDN

---
