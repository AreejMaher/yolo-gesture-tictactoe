# Gesture-Controlled Tic-Tac-Toe using YOLOv5

This project presents a real-time, interactive Tic-Tac-Toe game where players use hand gestures as input. The system is powered by a custom-trained YOLOv5 object detection model that recognizes specific gestures for the "X" and "O" moves.

![Tic-Tac-Toe Demo](tictactoe-demo.gif)

## ✨ Key Features

* **Real-Time Gesture Recognition:** Utilizes a YOLOv5 model to detect hand gestures from a live webcam feed with minimal latency.
* **Custom-Trained Model:** The model was trained on a custom dataset of 500 images, augmented to 3700, to recognize two specific gestures:
    * **Crossed Fingers:** Represents the 'X' player.
    * **OK Sign:** Represents the 'O' player.
* **Interactive Gameplay:** An OpenCV-based interface draws the 3x3 grid and places the 'X' and 'O' symbols based on the detected gesture's location.
* **Complete Game Logic:** Implements a turn-based system and standard Tic-Tac-Toe rules to detect win, draw, and loss conditions.

## 📈 Model Development Pipeline

The core of this project was the end-to-end development of the gesture recognition model:

1.  **Dataset Collection:** Captured 500 images of hand gestures under various lighting conditions, angles, and backgrounds.
2.  **Annotation:** Used Roboflow to precisely label the "X" (crossed fingers) and "O" (OK sign) gestures.
3.  **Data Augmentation:** Applied techniques like flipping, rotation, and scaling to increase dataset size and model robustness.
4.  **Training:** Trained a YOLOv5 model on the custom dataset, achieving **92% accuracy** on the test set.

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:**
    * PyTorch (for YOLOv5)
    * OpenCV (for image processing and the game interface)
    * NumPy
* **Tools:** Roboflow (for annotation)


