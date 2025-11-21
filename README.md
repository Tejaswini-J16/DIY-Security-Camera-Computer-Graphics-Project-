# DIY-Security-Camera-Computer-Graphics-Project
🔐 Motion Detection Security Camera

This project is a simple yet effective motion detection security system built using Python and OpenCV. It continuously monitors webcam video feed and detects movement by comparing consecutive frames. When a significant motion is detected, the system triggers an audible alert using the system speaker.



🚀 Features

🖥 Real-time video capture using the system webcam.

🎯 Motion detection by comparing differences between consecutive frames.

⚠️ Automatic alarm sound when large movement is detected.

🎡 Contour detection to identify the moving objects.

📷 Live preview window showing processed video feed.

⏹ Can be stopped anytime by pressing the ESC key.



🧠 How It Works

The webcam captures two consecutive frames.

The system compares the frames using cv2.absdiff() to detect differences.

The result is converted to grayscale and thresholded.

Using findContours(), the program identifies areas with movement.

If a contour is large enough, it triggers a beep alert using winsound.

The processed frame is displayed in a window in real-time.




🛠️ Tech Stack

Python

OpenCV

Winsound (Windows beep library)




📂 Code Overview

Reads continuous frames from webcam

Computes frame difference for motion detection

Ignores small movements

Plays alarm sound for significant motion

Displays processed video feed

Releases resources on exit




🧰 Requirements

Install the required dependencies:

pip install opencv-python

winsound is built-in for Windows systems.



▶️ Running the Project

Run the script using:

python camera.py

Press ESC to exit the program.




📈 Possible Enhancements

Save recorded footage when motion is detected

Send email or mobile notification alerts

Add face recognition

Use OpenCV DNN for object detection

Deploy on Raspberry Pi for standalone CCTV

Store logs of detected movement with timestamps




📸 Applications

Home security,

Office surveillance,

Baby monitoring,

Door activity tracking,

Basic AI camera demonstration.

