# 车位识别中的计算机视觉
以车位识别为例介绍CV中经典算法

## 架构
架构设计图
主要分为图像预处理，边沿检测，直线检测，角点识别，及车位拟合

## kernel(核函数)
核函数的作用相当于一个filter。可以作提取特征用。通过计算核心函数与原图的卷积，提取图像的某些特征。
![fiter](./img/ADAS/pointcloud.png)

## 低通滤波
图片模糊处理
gausissan kernel
![gaus]

## 高通滤波
边沿检测
Gradients
Gradients are a measure of intensity change in an image, and they generally mark object boundaries and changing area of light and dark. If we think back to treating images as functions, F(x, y), we can think of the gradient as a derivative operation F ’ (x, y). Where the derivative is a measurement of intensity change.

Sobel filters
The Sobel filter is very commonly used in edge detection and in finding patterns in intensity in an image. Applying a Sobel filter to an image is a way of taking (an approximation) of the derivative of the image in the xx or yy direction. The operators for Sobel_xSobel 
x
​	
  and Sobel_ySobel 
y
​	
 , respectively, look like this:
sobel high pass，
sobel x, y 
![sobel]
 
### 边沿检测canny
调参的含义
canny double thresholding, eliminate weak edges and nosie 
isolates edges that are part of an object boundary
![canny]

## 直线检测
6 hough
线段检测
![sobel]


## 角点检测
9 hog+svm
![sobel]

## 车位拟合
1.在直角坐标系下通过最小二乘法拟合
2.在Hough空间拟合
![sobel]
![sobel]
1calcualtes the magnitude and direction of the gradient at each pixel
2groups these pixel into square cells
3. counts how many gradients in each cell fall in a certain range of the orientations
histogram of oriented gradient