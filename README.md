# Virtual-Painting


I have created this Virtual Paint Program to paint(draw) on your screen using hand gestures.

## Gestures
- Index Finger - for drawing
- Index+Middle Finger - for changing position and objects
- Middle+Fourth Finger - for clearing whole screen
- Thumb+Index Finger - for shape sizes
- Except Thumb all Fingers - storing images dynamically
- Thumb+Little Finger - for exit



## Requirements
- Python 3.10.9 64 bit
- Visual Studio Code



## Installation
To run this file you need to install some PYTHON modules, open your CMD and type following commands-

- pip install mediapipe
- pip install opencv-python
- pip install numpy



## Code
Firstly I have created a Module "HandTrackingModule.py", this file contains the code which detects our hand, in this file I have created functions for specific tasks in a class "handDetector()".

Short description of functions are -

- findHands() - This function detect hands and show landmarks of your hand and it return image in RGB.
- findPosition() - This function finds the position of particular landmark of your hand and it returns a list containing id_of_that_landmark, x_position_of_that_landmark, y_position_of_that_landmark.
- fingersUp() - This function check wheather your particular finger is up or not and it return a list containing values 0 (if finger is down) ans 1 (if finger is up). i.e. [0,0,0,0,0] if all the 5 fingers are down and [1,1,1,1,1] if all the fingers are up.

Then another file is "VirtualPaint.py", this file uses that HandTrackingModule and contains the code which draw on the screen and provide various features (3 Colors + Eraser), and there is a folder "Paint" which contains the UI for this program.


