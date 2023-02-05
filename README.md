# Lane Detection System using OpenCV

This is a lane detection system implemented using OpenCV and Python. The system detects lane lines in a video stream and highlights them in green color.

## Dependencies

OpenCV

NumPy

Matplotlib

Steps to run the code

## Clone the repository

git clone https://github.com/<username>/LaneDetectionSystem.git

## Install the dependencies

pip install opencv-python

pip install numpy

pip install matplotlib

## Run the code

python lane_detection.py

The video stream with highlighted lane lines will be displayed in a window. Press q to exit the video stream.

## Code explanation

The code contains the following functions:

region_of_interest - This function masks the region outside the region of interest (ROI). The ROI is defined using vertices and passed as an argument to this function. The function returns the masked image.

draw_the_lines - This function draws the lane lines on the original image. The input is an image and the lines detected in the previous step. The function returns the image with the highlighted lane lines.

process - This function is the main pipeline of the system. It takes an image as input and returns the image with highlighted lane lines. The function performs the following steps:

--> Convert the image to grayscale.

--> Apply Canny edge detection to the grayscale image.

--> Mask the region outside the ROI.

--> Use Hough Line Probabilistic Transform to detect lane lines in the cropped image.

--> Draw the detected lane lines on the original image.

The video stream is captured using OpenCV's VideoCapture class and processed frame by frame. The processed frame is displayed in a window until the user presses q.





