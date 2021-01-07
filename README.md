# LaneRecognition
Simple computer vision project for hackaton, created in 1 day. Based on OpenCV.

## How it works
For given input like this:
![source image](https://github.com/wiertek/LaneRecognition/blob/master/photos/samples/source.jpg "Wrong Lane")

The image is converted into grayscale, histogram is equalized and subtle gaussian blur is applied:
![source image](https://github.com/wiertek/LaneRecognition/blob/master/photos/samples/gaussGrey.jpg "Wrong Lane")

Then Canny edge detection algorithm is used and image is cropped to get this:
![source image](https://github.com/wiertek/LaneRecognition/blob/master/photos/samples/cannyEdges.jpg "Wrong Lane")

Finially, Hough transform is performed, to detect the lines:
![source image](https://github.com/wiertek/LaneRecognition/blob/master/photos/samples/houghTransform.jpg "Wrong Lane")

Algorithm evaluates mainly on the angles, look at the source code for more details.
