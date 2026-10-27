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

## Preliminary Results
In the demonstration video, the system processed 846 frames and successfully generated knee-tracking annotations.

The exploratory analysis identified one candidate squat repetition, with the lowest position occurring at approximately 12.78 seconds.

The maximum measured projected knee deviation was approximately 11.63 degrees.

These findings are preliminary and have not been clinically validated.

## How to Run
1. Download the Jupyter Notebook from this repository.
2. Open it in Google Colab.
3. Install the required Python libraries.
4. Upload a single-leg squat video.
5. Run the notebook cells in order.
6. Launch the Gradio application to analyze the video.

## Limitations
- The prototype focuses on the anatomical left leg.
- Camera position and video mirroring affect measurements.
- Two-dimensional pose analysis cannot fully represent three-dimensional knee biomechanics.
- The current prototype uses pretrained pose estimation and geometric calculations, not a separately fine-tuned knee-valgus classifier.
- The system is intended for educational and research demonstration, not medical diagnosis.

## Future Improvements
- Collect expert-labeled single-leg squat datasets.
- Train and evaluate a valgus-versus-normal classifier.
- Improve repetition detection and angle validation.
- Incorporate real-time webcam feedback.
