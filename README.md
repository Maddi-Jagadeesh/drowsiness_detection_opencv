Drowsiness Detection using OpenCV and dlib

This project detects drowsiness by monitoring eye blinks using a webcam in real-time.

Prerequisites

Python 3.7+

Libraries: OpenCV, dlib, imutils, numpy

Webcam connected and accessible by your system

Installation

Clone this repository or copy the script files.

Install the required Python packages:
pip install opencv-python dlib imutils numpy

Download the Facial Landmark Predictor model file

This project requires the shape_predictor_68_face_landmarks.dat file, which is a pre-trained model used by dlib to detect facial landmarks.

You must download this file manually from the official dlib source:
http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

After downloading, extract the .bz2 archive to get the .dat file.


Place the extracted file shape_predictor_68_face_landmarks.dat in the same directory as your Python script or provide the full path to it in your code:
predictor = dlib.shape_predictor("shape_predictor_68_face_landmarks.dat")

Usage
Run the Python script after confirming the .dat file is accessible.
The script will open your webcam and start the drowsiness detection.

Press ESC to stop the program.

Notes

Make sure your webcam permissions are enabled.

The .dat model file is large (~100 MB) and not included in this repository.

References

dlib official site for model: http://dlib.net

Shape predictor model trained on iBUG 300-W dataset.

