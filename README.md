# Emotion Recognition with Optical Flow and Face Detection

## Overview

This project is a Jupyter Notebook developed in an IDE (VS Code) that implements a real-time emotion recognition system using optical flow, face detection, and emotion analysis. The system uses a webcam feed to capture video, detects faces with MTCNN, analyzes facial emotions with DeepFace, and visualizes motion using optical flow with OpenCV.

## Prerequisites

Before running the code, ensure this Python version is installed:

- Python 3.9 (this works properly with both Tensorflow and MTCNN)

## Setup Instructions

Follow these steps to set up and run the project:

### 1. Create a Virtual Environment

Create a virtual environment for the project:

```bash
python -m venv <environment_name>
```

Activate the virtual environment:

- **On Windows:**
  ```bash
  source <environment_name>/Scripts/activate
  ```
- **On macOS/Linux:**
  ```bash
  source <environment_name>/bin/activate
  ```

### 2. Install Required Libraries

Install the necessary dependencies listed in `requisites.txt`:

```bash
pip install -r requisites.txt
```

### 3. Select the Kernel and Run the Code

Before running the notebook, ensure that the Python kernel used in Jupyter Notebook is set to the virtual environment you just created.
Then run the cells sequentially in the IDE to execute the code.



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

