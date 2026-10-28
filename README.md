# Knee Valgus Detection
analyze the movement of a person's knee during a single-leg squat

## Project Demonstration
20-minute video presentation: https://drive.google.com/file/d/1kvC9462UkzBF1HFN7Q2AieC7OrBVsS4Y/view?usp=drivesdk

Brief written summary:

## Project Overview
This project demonstrates a computer-vision prototype for analyzing knee movement during a single-leg squat using a front-facing video.

The system uses MediaPipe Pose Landmarker to identify the patient's left hip, knee, and ankle, calculates 2D projected knee alignment, and generates an annotated video displaying movement direction.

An interactive Gradio interface allows users to upload a squat video and view the processed results.

## Project Objectives
1. Detect human pose landmarks using MediaPipe.
2. Calculate projected knee alignment during a single-leg squat.
3. Identify squat movement phases and candidate repetitions.
4. Visualize knee movement using graphs and annotated videos.
5. Build an interactive Gradio application.

## Technologies Used
- Python
- Google Colab
- MediaPipe
- OpenCV
- NumPy
- Matplotlib
- Pandas
- SciPy
- Gradio

## Methodology
1. Upload a front-facing single-leg squat video.
2. Extract anatomical left-leg landmarks using MediaPipe.
3. Calculate 2D projected knee angles and normalized knee displacement.
4. Analyze squat movement throughout the video.
5. Generate an annotated output video.
6. Display results using Gradio.
