# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.
## Program 
## Developed By : GANESH R
## Reg No : 212222240029
```p
import cv2
import matplotlib.pyplot as plt

img=cv2.imread("bird.jpeg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
## Sobel X axis
```p
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelx)
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
## Sobel Y axis
```p
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobely)
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
## Sobel XY axis
```p
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelxy)
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
## Laplacian Edge Detector
```p
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(lap)
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
## Canny Edge Detector
```p
canny=cv2.Canny(gray,120,150)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(canny)
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
## SOBEL EDGE DETECTOR
## Sobel X axis
![image](https://github.com/ganesha360/EDGE-DETECTION/assets/120884552/8859fbe0-3e79-4f5c-9c58-e97dfa143242)

## Sobel Y axis
![image](https://github.com/ganesha360/EDGE-DETECTION/assets/120884552/74af07e4-0ecd-49d9-8092-ff6e4c84aedc)

## Sobel XY axis
![image](https://github.com/ganesha360/EDGE-DETECTION/assets/120884552/2b831678-5e27-4e1d-9110-f36c6f25991e)

## LAPLACIAN EDGE DETECTOR
![image](https://github.com/ganesha360/EDGE-DETECTION/assets/120884552/d65feb97-790a-48b0-93ab-b67e1f463433)

## CANNY EDGE DETECTOR
![image](https://github.com/ganesha360/EDGE-DETECTION/assets/120884552/4ef104e0-818b-4550-ae92-521a81dd2fb1)


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
