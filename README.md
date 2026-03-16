## Project Overview

This project develops an **AI-based hand gesture recognition system** that allows users to control a drone using hand gestures detected by a camera. The system uses computer vision and deep learning to recognize gestures and convert them into drone control commands such as takeoff, landing, and directional movement.

The goal of this project is to create a **natural and contactless human–machine interaction system** where drones can be controlled without traditional remote controllers.

---

## Dataset

The gesture recognition model in this project is trained using the **Hand Gesture Recognition Dataset** from Kaggle.

Dataset link:  
[Hand Gesture Recognition Dataset](https://www.kaggle.com/datasets/aryarishabh/hand-gesture-recognition-dataset)

### Dataset Information

- Total images: **24,000**
- Total gesture classes: **20**
- Training images per class: **900**
- Testing images per class: **300**

The dataset contains images of different hand gestures captured under various lighting conditions and backgrounds, making it suitable for training deep learning models for gesture classification tasks.

The dataset includes multiple hand gesture categories such as **thumbs up, thumbs down, stop, directional pointing gestures, and peace signs**, which are commonly used for gesture-based interaction systems.

---

## Development Approach

The system follows the workflow below:

1. Collect and prepare the gesture dataset.
2. Train a gesture recognition model using deep learning.
3. Convert the trained model to a lightweight format for real-time inference.
4. Detect gestures from live camera input.
5. Map recognized gestures to drone control commands.

---

## System Pipeline
```
Camera Input
↓
Hand Gesture Recognition Model
↓
Gesture Classification
↓
Command Mapping
↓
Drone Control
```

Example gesture commands:

| Gesture | Drone Command |
|-------|---------------|
| 👍 | Takeoff |
| 👎 | Land |
| ✋ | Stop |
| 👉 | Move Right |
| 👈 | Move Left |

---

## Technologies Used

- Python
- OpenCV
- TensorFlow / TensorFlow Lite
- Computer Vision
- Edge AI / TinyML
- Drone SDK (e.g., DJI Tello)

---

## Future Improvements

- Improve gesture recognition accuracy
- Implement real-time tracking using MediaPipe
- Deploy the model on embedded edge devices
- Integrate autonomous drone navigation
