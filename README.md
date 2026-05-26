# Pose Estimation Assignment – Computer Vision

## Project Overview

This project demonstrates a **human pose estimation and activity recognition system** using **Computer Vision** and **MediaPipe Pose**. The system detects human body landmarks from a video, calculates joint angles, and identifies human activities such as standing based on body posture.

The project processes a raw input video, extracts body keypoints, computes important joint angles (knee, elbow, hip), and generates an annotated output video with a visual skeleton overlay and activity labels.

---

## Features

* Human pose detection using **MediaPipe**
* Real-time body landmark tracking
* Joint angle calculation:

  * Knee angle
  * Elbow angle
  * Hip angle
* Activity recognition based on body posture
* Annotated output video generation
* Skeleton visualization
* Angle plotting and performance analysis

---

## Technologies Used

* Python
* OpenCV
* MediaPipe
* NumPy
* Matplotlib
* Jupyter Notebook

---

## Project Structure

```bash
Pose-Estimation-Assignment-CV/
│
├── pose_activity_FIXED.ipynb      # Main notebook
├── output_raw.mp4                 # Original input video
├── output_annotated (2).mp4       # Annotated output video
├── pose_landmarker_lite.task      # MediaPipe pose model
├── accuracy_report.png            # Accuracy visualization
├── angle_plots (2).png            # Joint angle graphs
├── skeleton_samples.png           # Skeleton detection samples
└── README.md                      # Project documentation
```

---

## How It Works

### 1. Pose Detection

The system uses MediaPipe Pose to detect body landmarks from each frame of the video.

### 2. Landmark Extraction

Important body points are extracted, including:

* Shoulders
* Elbows
* Hips
* Knees
* Ankles

### 3. Angle Calculation

Using geometric calculations, the system computes:

* Elbow angle
* Knee angle
* Hip angle

### 4. Activity Recognition

The activity is classified based on predefined angle thresholds.

Example:

```python
if knee_angle > 160 and hip_angle > 160:
    activity = "Standing"
```

### 5. Video Annotation

The final output video displays:

* Skeleton overlay
* Joint points
* Calculated angles
* Predicted activity

---

## Sample Output

### Activity Detection

* Standing

### Example Angles

* Knee Angle: 172°
* Elbow Angle: 102°
* Hip Angle: 173°

---

## Installation

### Clone Repository

```bash
git clone https://github.com/javeria843/Pose-Estimation-Assignment-CV.git
cd Pose-Estimation-Assignment-CV
```

### Install Dependencies

```bash
pip install opencv-python mediapipe numpy matplotlib
```

---

## Run the Project

Open the notebook:

```bash
jupyter notebook
```

Then run:

```bash
pose_activity_FIXED.ipynb
```

---

## Results

The system successfully:

* Detects body posture
* Calculates accurate joint angles
* Recognizes standing activity
* Generates annotated visual outputs

---

## Future Improvements

* Add more activity classes:

  * Walking
  * Sitting
  * Running
  * Jumping
* Real-time webcam support
* Deep learning–based activity classification
* Improved accuracy using custom-trained models

---

## Applications

* Fitness tracking
* Sports analytics
* Healthcare monitoring
* Physical therapy
* Human-computer interaction
* Surveillance systems

---

## Author

**Javeria**
Computer Vision & AI Project

