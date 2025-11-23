# Cursor-Control
Project Title

Gesture-Controlled Cursor Using Python


---

Motivation

The purpose of this project is to explore touchless human–computer interaction using computer vision. Modern applications increasingly focus on gesture control, automation, and accessibility.
This project demonstrates how a webcam can track hand movements and convert them into mouse actions such as cursor movement and clicking.
The goal is to create a simple, low-cost, contact-free alternative to a physical mouse.


---

Data Description

This project does not use traditional datasets. Instead, it uses real-time webcam input as the data source.

Data Sources & Format:

Input Data: Live video frames captured using the system’s webcam (cv2.VideoCapture(0)).

Data Processing:

Frames are converted to RGB format.

Mediapipe extracts 21 hand landmarks from each frame.

Coordinates of specific landmarks (index finger tip ID 8, thumb tip ID 4) are used to calculate cursor movement and click gestures.


Output Data:

Cursor movement on the computer screen.

Mouse click events detected from gesture distance.



How Data Is Created:

Data is created dynamically from the user's real-time hand movement.

No external files, CSV, images, or datasets are used.



---

How to Use

1. Install Required Libraries

Run the following commands in terminal/cmd:

pip install opencv-python mediapipe pyautogui

2. Run the Code

Save the script as gesture_cursor.py and run:

python gesture_cursor.py

3. Controls

Move Cursor: Move your index finger (tip ID 8).

Click: Bring your thumb (ID 4) close to the index finger (ID 8).

Exit Program: Press ESC.


4. Requirements

Python 3.7+

Webcam

Stable lighting

Windows/Mac/Linux



---

Contact Information

For questions or collaboration, contact:

Name: [Your Name]
Email: [Your Email]
GitHub (optional): [Your GitHub Profile]


---

License

This project is licensed under the MIT License, meaning:

You are free to use, modify, and distribute the code.

You must include credit to the original author.

The project is provided “as-is” without warranty.



---

Notes

Ensure proper lighting for better hand tracking.

Avoid busy or cluttered backgrounds to improve detection accuracy.

Works best when the hand is 30–60 cm away from the camera.

For smoother control, you may adjust sensitivity and smoothing values in the code.