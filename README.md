🎨 Virtual Paint App – Hand Gesture Drawing using OpenCV & MediaPipe

This project is a virtual painting application that allows users to draw on the screen using hand gestures detected from a webcam. It uses OpenCV for image processing and MediaPipe for hand-tracking.
You can draw lines, rectangles, circles, free-hand sketches, and also erase your drawings — all using simple finger movements.

🚀 Features

✔️ Hand Tracking using MediaPipe

✔️ Gesture-based Tool Selection

Line

Rectangle

Circle

Free Draw

Eraser

✔️ Smooth Drawing with Index Finger

✔️ Real-time Video Processing

✔️ Toolbar Overlay for Tool Selection

📁 Project Structure
virtual_paint_app/
│
├── virtual_paint_app.py     # Main application code
├── tools.png                # Toolbar image (required)
└── README.md                # Project documentation

🧰 Requirements

Install the required Python packages before running the project:

pip install opencv-python mediapipe numpy

▶️ How to Run

Clone or download the project folder.

Place tools.png in the same directory as virtual_paint_app.py.

Run the script:

python virtual_paint_app.py


The webcam will open automatically.

🖐️ Gesture Controls
🎛 Tool Selection

Move your index finger into the toolbar area at the top-left and hold for ~1 second.

Toolbar layout (left → right):

Line

Rectangle

Draw

Circle

Erase

✏️ Drawing

Raise your index finger → start drawing

Lower your finger → stop drawing

🧽 Erasing

Use the erase tool and hover your finger over drawn areas.

🧠 How It Works

MediaPipe detects 21 hand landmarks in real time.

The app tracks the position of:

Index Finger Tip (landmark 8)

Middle Finger Tip (landmark 12)

Finger Fold Landmarks (landmark 9)

Gestures are identified by comparing finger positions.

Mask-based drawing is applied and merged with the webcam feed.

🛠 Technologies Used

Python

OpenCV

MediaPipe

NumPy

📷 Screenshots (optional)

You can add images here:

![Demo Screenshot](demo.png)

📌 Future Improvements (optional)

Add undo/redo features

Save drawings

Add colors to the drawing tools

Better UI for toolbar

📄 License

This project is for educational and demo purposes only.