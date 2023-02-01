# Circle Overlap Detection in Animation Video
A project that plays an animation video and pauses the video where the center of a green circle and a blue circle exactly overlap (or very close to each other).

## Requirements
- OpenCV
- Numpy

## Usage
1. Clone or download the repository to your local machine
2. Run the code using a Python environment with the above dependencies installed.
3. The program will automatically load the animation video.
4. The program will display each frame of the video and pause the video when the center of the green circle and the blue circle overlap (or are very close to each other).
5. If the centers of both circles do not overlap, the program will continue to play the video until the end.

## Algorithm
1. Load the video using OpenCV's VideoCapture function.
2. Convert the video frames to grayscale using cvtColor function.
3. Use the Hough Circle Transformation technique to detect the circles in each frame.
4. Track the centers of the green and blue circles in each frame.
5. Check the distance between the centers of the green and blue circles in each frame.
6. If the distance is below a certain threshold, pause the video and display the frame.
7. If the distance is above the threshold, continue to play the video and display the next frame.

## Note
- The code has been tested on the provided animation video with green and blue circles. The accuracy may vary on videos with different shapes, colors, and movements of the objects.
- The threshold for the distance between the centers of the circles can be adjusted in the code to control the sensitivity of the overlap detection.
