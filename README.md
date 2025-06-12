# CV_hand_detection

✋ Orientation-Invariant Hand Detection using OpenCV & MediaPipe
This project uses OpenCV and MediaPipe to detect hands in real-time from a webcam feed, analyze hand landmarks, and determine whether each finger is extended, regardless of hand orientation. It includes enhanced finger analysis with 3D angle calculations for robust gesture detection.

📂 Features
Real-time hand detection and landmark tracking

Finger extension classification (thumb, index, middle, ring, pinky)

3D angle-based orientation-invariant logic

Visual overlay of detected landmarks and extended fingers

Count of extended fingers shown on screen

🛠️ Technologies Used
Python 3

OpenCV (cv2)

MediaPipe (mediapipe)

NumPy (numpy)

🚀 How to Run
Install dependencies:

bash
Copy
Edit
pip install opencv-python mediapipe numpy
Run the main script:

bash
Copy
Edit
python main.py
Controls:

The webcam will open automatically.

Press ESC to exit.

🧠 How It Works
MediaPipe detects hand landmarks in 3D.

Vectors and angles between joints are computed using NumPy.

Finger extension is decided based on:

Wrist to MCP (knuckle) angle

MCP to TIP alignment

Thresholds vary by finger (e.g., thumb is more flexible).

📸 Output Example
Extended fingers are marked with green circles and labels.

Total number of extended fingers is shown on the top-left.

📌 Notes
Works best in well-lit conditions.

Can detect up to two hands simultaneously.

🧩 Future Enhancements
Gesture classification (e.g., "peace", "fist", "OK" sign)

Multi-language finger counting voice assistant

Gesture-controlled UI interactions

