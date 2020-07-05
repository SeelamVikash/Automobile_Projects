# Automobile_Projects
# **Finding Lane Lines on the Road** 

# My Pipeline for side lane lines detection
1. I have read the image.
2. I have converted it into grayscale for easy processing.
3. I have used gaussian blur to reduce noise.
4. I have detected the edges using the canny edge detection algorithm.
5. I have selected the region of interest.
6. Using the Hough Tranformation I have detected the coordinates of the lines.
I have modified draw_lines function as follows
1. Segregated the points according to the slope there by seperating the left and right lane lines.
2. Built a regression fit and found coefficients for extrapolation.
3. Built a line equation.
4. Drawn lines using the line equation by giving the coordinates with in my limit.
### initial image
<img src="https://github.com/SeelamVikash/Automobile_Projects/blob/master/CarND-LaneLines-P1-master/test_images/solidWhiteCurve.jpg" alt="Output" width="300" height="200">

### Output image
<img src="https://github.com/SeelamVikash/Automobile_Projects/blob/master/CarND-LaneLines-P1-master/test_images_output/output_of_solidWhiteCurve.jpg.png" alt="Output" width="300" height="200">

# Pipeline for side lane lines detection in a video
1. Used VideoFileClip for reading the video.
2. Used fl_image to read and process the data Frame by Frame using process_image function.

<a href="https://youtu.be/eB6Nlvnuago">Click this to see the result on video</a>


### 2. potential shortcomings with my current pipeline


One potential shortcoming would be what would happen when there is a curvey lane lines it became hard to detect lane lines.

Another shortcoming could be what if there are white cars present inside the region of interest.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to improve the lane detection during turnings

Another potential improvement could be to avoid the other objects with in the region  of interest.
