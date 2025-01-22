# Emotion Recognition with Optical Flow and Face Detection

## Overview
This project implements a real-time emotion recognition system using optical flow, face detection, and emotion analysis. The system uses a webcam feed to capture video, detects faces with MTCNN, analyzes facial emotions with DeepFace, and visualizes motion using optical flow with OpenCV.

## Prerequisites
Before running the code, ensure the following tools and libraries are installed:

- Python 3.x
- `virtualenv` (for creating a virtual environment)

## Setup Instructions
Follow these steps to set up and run the project:

### 1. Install `virtualenv`
If `virtualenv` is not already installed, install it using pip:
```bash
pip install virtualenv
```

### 2. Create a Virtual Environment
Create a virtual environment for the project:
```bash
virtualenv env
```

Activate the virtual environment:
- **On Windows:**
  ```bash
  .\env\Scripts\activate
  ```
- **On macOS/Linux:**
  ```bash
  source env/bin/activate
  ```

### 3. Install Required Libraries
Install the necessary dependencies listed in `requisites.txt`:
```bash
pip install -r requisites.txt
```

### 4. Select the Kernel
Before running the script, ensure that the Python kernel used in your IDE (e.g., Jupyter Notebook or VSCode) is set to the virtual environment you just created.

## Running the Code
To execute the script, run the following command in your terminal:
```bash
python <script_name>.py
```
Replace `<script_name>.py` with the actual name of your Python script.

## Key Features
- **Real-Time Optical Flow Visualization:** Displays motion patterns in the video feed using dots and arrows.
- **Face Detection:** Detects faces in the video feed using the MTCNN library.
- **Emotion Recognition:** Analyzes emotions of detected faces using DeepFace.
- **Dynamic Visualization:** Visualizes detected emotions with bounding boxes, colored corners, and text.

## How It Works
1. The script captures video frames from the webcam.
2. Optical flow is calculated using OpenCV's Farneback method to identify motion patterns.
3. The MTCNN library detects faces in each frame.
4. The DeepFace library analyzes the detected faces to determine the dominant emotion.
5. The emotions are visualized on the frame with bounding boxes and color-coded indicators.
6. The processed video feed is displayed in real time.

## Controls
- Press `q` to quit the program.

## Notes
- Ensure the webcam is properly connected and accessible.
- The script is optimized for environments with a consistent lighting setup.
- Emotion analysis is performed every 10 frames to optimize performance.

## License
This project is open-source and available under the MIT License.

