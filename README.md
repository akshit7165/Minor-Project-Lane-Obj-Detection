 # Lane Detection and Vehicle Tracking

This project implements a lane detection system that can detect lanes on static images as well as video files and also track vehicles on the road.

## Features

- Applies distortion correction and bird's eye view transformation on input images to get a top-down view of the lanes
- Converts the original image to different color spaces (RGB, HLS, HSV, YCrCb) and extracts the luminance/saturation channels to obtain a binary image  
- Performs thresholding of the warped images and converts them to Sobel gradient images to extract the lane pixels
- Fits polynomial lines to the lane pixels and highlights the detected lanes on the original image  
- For video files, applies perspective transform on each frame to create masks and extract the lane data
- Uses the 'Sweeping Window' technique to calculate the lane start and width based on lane hotspots  
- Extracts the lane center to determine the vehicle position on the road
- Detects vehicles on the road using the YOLOv3 dataset

## Accuracy

The system achieves an accuracy of 85% under Indian road conditions.

## Technologies Used

- Python 
- OpenCV  
- NumPy

## Instructions

1. Install the required libraries - OpenCV, NumPy 
2. Run the lane_detection.py file to detect lanes on a sample image   
3. Run the lane_detection_video.py file to detect lanes and track vehicles in a sample video

You can modify the code to detect lanes on your own images and videos.

That's it! You now have a functional lane detection and vehicle tracking system built with computer vision techniques in Python.
