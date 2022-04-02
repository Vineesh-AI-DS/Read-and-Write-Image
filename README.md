# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:

# Developed By:Vineesh M
# Register Number:212221230122
# To Read,display the image
```python
import cv2
a = cv2.imread('luffty.jpg',1)
cv2.imshow("ANIME",a)
cv2.waitKey(0)
```
# To write the image
```python
import cv2
colorImage = cv2.imread('luffty.jpg',1)
cv2.imwrite('written.jpg',colorImage)
writtenImage = cv2.imread('written.jpg',1)
cv2.imshow('WrittenImage',writtenImage)
cv2.waitKey(0)
```

# Find the shape of the Image
```python
import cv2 
colorImage = cv2.imread('luffty.jpg',1)
print(colorImage.shape)
```
# To access rows and columns
```python
import cv2
import random
colorImage = cv2.imread('luffty.jpg',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('to access rows and columns',colorImage)
cv2.waitKey(0)
```
# To cut and paste portion of image
```python
import cv2
color_img = cv2.imread('luffty.jpg',1)
tag = color_img[200:400,300:500]
color_img[300:500,200:400] = tag
cv2.imshow('Cut And Paste',color_img)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image
<img src=luffy.png>
<br>
<br>

### ii)Write the image
<img src=sanjii.png>
<br>
<br>

### iii)Shape of the Image
<img src=roger.png>
<br>
<br>

### iv)Access rows and columns
<img src=acee.png>
<br>
<br>

### v)Cut and paste portion of image
<img src=zoroo.png>
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


