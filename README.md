# Virtual-Pen
Computer Vision Project implemented with OpenCV.

In this we can draw anything on it just by capturing the motion of a colored marker with camera. Here the coloured object is a pen. Here I have used computer vision techniques of OpenCV to build this project. The language that I have used is Python but we can use any OpenCV preferrable language.

Here Color Detection and tracking is used in order to achieve the objective. The color marker is detected and a mask is produced. It includes morphological operations on the mask produced which are Erosion and Dilation. Erosion reduces the impurities present in the mask and dilation further restores the eroded main mask.

## Algorithm
<ol type="1">
  <li> Start reading the frames and convert the captured frames to HSV color space (Easy for Color detection). </li>
  <li> Prepare the canvas frame and put the respective ink buttons on it.</li>
  <li> Adjust the trackbar values for finding the mask of colored marker.</li>
  <li> Preprocess the mask with morphological operations (Erosion and dilation).</li>
  <li> Detect the contours, find the center coordinates of largest contour and keep storing them in the array for successive frames (Arrays for drawing points on canvas).</li>
  <li> Finally draw the points stored in array on the frames and canvas.</li>
</ol>
