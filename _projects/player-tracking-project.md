---
layout: default
title: "AI Player Tracking with YOLOv8 & DeepSORT"
category: "Personal"
tech-stack: "Python, YOLOv8, DeepSORT, PyTorch, OpenCV"
github-link: "https://github.com/githubabhay2003/Player-Tracking"
---

# Project: AI Player Tracking with YOLOv8 & DeepSORT

This project is a sophisticated computer vision pipeline that performs real-time player detection and tracking in football match footage using a custom-trained AI model.

[Back to Home](./index.md)

---

### 1. The Goal
The primary objective was to build and implement a robust system for player detection and tracking in sports footage. The solution leverages a custom-trained YOLOv8 model to identify players in each frame and the DeepSORT algorithm to assign and maintain unique tracking IDs for each player, even amidst occlusion and rapid movement.

---

### 2. My Role & Contributions
As the engineer for this project, I was responsible for integrating the entire computer vision pipeline from model inference to final output.

* **Model Integration:** I utilized a custom-trained YOLOv8 model specifically fine-tuned for player detection, ensuring high accuracy in identifying subjects within the video frames.
* **Tracking Algorithm Implementation:** I implemented the DeepSORT algorithm, a state-of-the-art multi-object tracking system, to process the YOLOv8 detections. This involved managing object states, handling re-identification, and assigning persistent IDs to each player.
* **Pipeline Development:** I wrote the core Python script that orchestrates the entire process: loading the video, passing frames to the YOLOv8 model, feeding detections to DeepSORT, and rendering the final output video with tracking boxes and IDs using OpenCV.
* **Environment & Dependency Management:** I managed all project dependencies, including specific versions of PyTorch and Ultralytics, and handled large model files using Git LFS for proper version control.

---

### 3. Technologies Used
* **Object Detection:** YOLOv8 (custom-trained model)
* **Object Tracking:** DeepSORT
* **ML Framework:** PyTorch
* **Core Language:** Python
* **Computer Vision Library:** OpenCV
* **Version Control:** Git, Git LFS

---

### 4. Project Links
* **<a href="https://github.com/githubabhay2003/Player-Tracking" target="_blank" rel="noopener noreferrer">View Code & Models on GitHub</a>**

---