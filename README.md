# Opencv-Background-Subtraction-Without-AI

# [YouTube link](https://www.youtube.com/watch?v=wtYW42sRU1Y)

 Algorithm
 
  1- Save the reference frame(in gray scale and saturation scale) at the beginning of the video
  2- Convert other coming frames to gray scale and also hsv channels
  3- Compare each new frame with the reference frame in saturation and gray scale
  4- If absolute value differences bigger than 25 than mark the pixel and save in a new Mat
  5- Then erode + dilate to this frame (2 times)
  6- Check non-zero pixels in gray channel domain and mark them for result image
  7- Remained zero pixels in Step-6 check in saturation domain and mark them in result image
  8- If still remained zero pixels which means they belong to background, you can make replace them with the desired background
 
  Requirements:
 
  1- At the beginning camera should take a reference frame so you shouldnt be in front of camera
  2- Camera should be constant
