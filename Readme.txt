I will explain blobk by block in this file:
1-In first block i import libraries
2-In 2nd block i import input image and resize it to 150 width by 150 height.
3-In 3rd block i plot image
4-In 4th block i convert RGB image into HSV.
5-In 5th block i apply Gaussian blur on image.
6-In 6th block i convert RGB image to Gray sclae image.
7-In 7th block i set Upper and lower white values according to HSV and apply on HSV image.You can see it is generating white color of image.
8-In 8th block i set upper and lower yellow values according to HSV and apply on HSV image. you can see it is generating yellow color of image.
9-In 9th block i combine both white and yellow mask and apply on image. you can see generated filter image. 
10-In 10th block i use grey scale image and apply canny edge detector on image to check edges of image.
11-In 11th block i set region according to road lines you can see i set shape in tri-shape and apply on canny edge generated image.
12-In 12th block i make function of Hough transform Lines function to detect lines.In this step i set roh from maximum possible distance
sqrt(width*width+height*height) and for theta i use range from -180,180.
13- In last step i use hough line result and draw lines on input image.