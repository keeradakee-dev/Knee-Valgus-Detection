# Knee Valgus Detection
analyze the movement of a person's knee during a single-leg squat

## Project Demonstration
20-minute video presentation: https://drive.google.com/file/d/1kvC9462UkzBF1HFN7Q2AieC7OrBVsS4Y/view?usp=drivesdk

Brief written summary:

## Project Overview
The main goal of this project is to develop a simple AI-based system that can analyze knee movement from a video.

The project aims to estimate how many degrees of knee deviation inward or outward during a single-leg squat. 

This project uses MediaPipe for human pose detection, 

Python for calculating knee angles, and 

Gradio for creating an interactive web application.

## Methodology
1. Upload a front-facing single-leg squat video.
2. Extract anatomical left-leg landmarks using MediaPipe.
3. Calculate 2D projected knee angles and normalized knee displacement.
4. Analyze squat movement throughout the video.
5. Generate an annotated output video.
6. Display results using Gradio.
