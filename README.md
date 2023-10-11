# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1 :
Load the necessary packages requiured for the implemtation of erosion and dilation on an image.

### Step 2 :
Create the text image for the implemtation of erosion and dilation using cv2.putText function.

### Step 3 :
Create the structuring image for the implemtation of erosion and dilation on the text image.

### Step 4 :
Apply the erosion and dilation to the text image using cv2.erode and cv2.dilate.

### Step 5 :
Display the images of the erosion and dilation applied using the plt.imshow.

### Step 6 :
End the program.
 
## Program:
## Developed by : NIROSHA S
## Register Number: 212222230097
### Program to implement Erosion and Dilation using Python and OpenCV.
## Import the necessary packages :
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
## Create the Text using cv2.putText :
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'ABRIN NISHA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()
```
## Create the structuring element :
```
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
Erode the image :
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()
```
## Dilate the image :
```
mage_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```
## Output :
## Display the input Image :
![image](https://github.com/Niroshassithanathan/EROSION-AND-DILATION/assets/121418437/151efcf8-3df6-4084-bd3f-3705cac9a903)

## Display the Eroded Image :
![image](https://github.com/Niroshassithanathan/EROSION-AND-DILATION/assets/121418437/626eb0b1-d95a-4523-b86f-d5d07ffe0f9e)

## Display the Dilated Image :
![image](https://github.com/Niroshassithanathan/EROSION-AND-DILATION/assets/121418437/16b80e89-9658-4244-81a2-1d4dabfb9a04)

## Result :
Thus the generated text image is eroded and dilated using python and OpenCV.
