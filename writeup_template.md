# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"
[image2]: ./examples/gray.png "gray.png"
[image3]: ./examples/blur_gray.png "blur_gray.png"
[image4]: ./examples/edges.png "edges.png"
[image5]: ./examples/masked_edges.png "masked_edges.png"
[image6]: ./examples/line_image.png "line_image.png"
[image7]: ./examples/lines_edges.png "lines_edges.png"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 

First, I converted the images to grayscale, 

![alt text][image2]

Secondly I blur the gray image,

![alt text][image3]

then I find the edge of image,

![alt text][image4]

and make the region of interest,

![alt text][image5]

after that, I find the lane line of the image,

![alt text][image6]

finally, I weight the lane line to the raw image.

![alt text][image7]

In order to draw a single line on the left and right lanes, I create the new draw_lines_full() function by 
* Classify the line between the right lane and the left lane,
* Fit the single line with line segments.



### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
