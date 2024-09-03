**Description**
This code creates an "Air Canvas" where hand movements tracked via a webcam are used to draw on a virtual canvas.
It utilizes Python with OpenCV for image processing, Mediapipe for hand tracking, and NumPy for managing points and colors.


**Algorithm**
Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)
Prepare the canvas frame and put the respective ink buttons on it.
Adjust the values of teh mediapipe intilization to detect one hand only.
Detect teh landmarks by passing the RGB frame to the mediapipe hand detector
Detect the landmarks, find the forefinger coordinates and keep storing them in the array for successive frames .(Arrays for drawing points on canvas)
Finally draw the points stored in array on the frames and canvas.
