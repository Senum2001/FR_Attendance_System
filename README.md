# Face Recognition Attendance System

This project is a Face Recognition Attendance System built using OpenCV and scikit-learn. It captures faces using a webcam, processes them, and records attendance based on face recognition.

## Features

- Capture and store face data using a webcam.
- Train a K-Nearest Neighbors (KNN) classifier on the captured face data.
- Recognize faces in real-time and record attendance with a timestamp.
- Save attendance records in CSV format.
- Announce attendance confirmation using text-to-speech.

## Prerequisites

- Python 3.x
- OpenCV
- NumPy
- scikit-learn
- pywin32 (for text-to-speech on Windows)
- A webcam

## Installation

1. Clone the repository or download the code files.
2. Install the required Python libraries:
    ```bash
    pip install opencv-python numpy scikit-learn pywin32
    ```

3. Download the Haar Cascade XML file for face detection from [here](https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml) and place it in the project directory.

## Usage

### Step 1: Capture Face Data

1. Run the script to capture face data:
 ```bash
    Dataset.py
```  
3. Enter your name when prompted. The script will capture 100 face images and store them.

### Step 2: Train the Classifier and Recognize Faces

1. Run the attendance script:
    ```bash
    Attendance.py
    ```
2. The script will load the captured face data, train a KNN classifier, and start recognizing faces using the webcam.

### Step 3: Record Attendance

1. When a face is recognized, the name and timestamp will be recorded.
2. Press 'o' to confirm and save the attendance record.
3. Attendance records are saved in the `Attendance` directory with the filename format `Attendance_dd-mm-yyyy.csv`.
4. directory needs to be added manually.
5. press 'q' to exit.

### Additional Information

- The background image `background.png` should be placed in the project directory.
- Attendance records are stored in CSV format in the `Attendance` directory.

