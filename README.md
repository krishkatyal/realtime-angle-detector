# An Automated Angle Evaluation System for Geometric Analysis using Computer Vision Techniques
## Overview
- This project demonstrates how to measure angles in an image using OpenCV library in Python.
- The code allows the user to select three points in the image and calculates the angle between the two lines connecting these points. 
- The calculated angle is then displayed on the image.

## Required Libraries
- OpenCV
- math
## Code Explanation
- The code starts by importing the required libraries: OpenCV and math.
- The path to the image file is provided and the image is read using the cv2.imread() function.
- The pointsList variable is initialized to an empty list.
- A mouse event function called mousePoints() is defined. This function draws a circle at the clicked point and a line joining it to the previous circle. It also appends the clicked point to the pointsList variable.
- The gradient() function is defined, which takes two points as input and returns the gradient of the line connecting them.
- The getAngle() function is defined, which takes the last three points in pointsList as input and calculates the angle between the two lines connecting these points using the math.atan() and math.degrees() functions.
- A while loop is used to continuously display the image, detect mouse clicks and draw circles and lines using the mousePoints() function, and calculate and display angles using the getAngle() function.
- Pressing the 'q' key resets the pointsList variable and the image is re-read.
## How to Use
- Clone or download the project.
- Make sure you have the required libraries installed.
- Change the path variable to the path of your image file.
- Run the code and click on three points in the image to measure the angle between them.
- Press the 'q' key to reset the points and start over.
## Conclusion
This project showcases a simple but useful application of OpenCV library in measuring angles in images. The code can be modified and expanded to suit different use cases, such as measuring angles in real-time video streams or incorporating more advanced image processing techniques.
