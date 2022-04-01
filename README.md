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
### Developed By:
### Register Number: 
i) #To Read,display the image
```python
import cv2
bike=cv2.imread('f77.jpg',0)
cv2.imshow('Grayscale',bike)
cv2.waitKey(0)
```
ii) #To write the image
```python 
import cv2
bike=cv2.imread('f77.jpg',1)
cv2.imwrite('UltraViollete.jpg',bike)
```
iii) #Find the shape of the Image
```python3
import cv2
bike=cv2.imread('f77.jpg',1)
print(bike.shapeS)


```
iv) #To access rows and columns

```python3
import cv2
bike=cv2.imread('f77.jpg',1)
import random
for i in range(200):
    for j in range(bike.shape[1]):
        bike[i][j] = [random.randint(0,100),random.randint(0,100),random.randint(0,100)]
cv2.imshow('UltraViollete',bike )
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3
import cv2
bike=cv2.imread('f77.jpg',1)
img = bike[300:400:,300:400]
bike[50:150,50:150] = img
cv2.imshow('Cut Selection',bike)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image
![read and write image processing ](https://user-images.githubusercontent.com/93978702/161278239-425a59f0-eae2-42df-b2c4-682f28a02251.png)

<br>
<br>

### ii)Write the image
![written image](https://user-images.githubusercontent.com/93978702/161279061-34c377bb-5afa-4405-8720-4a49ffc2fc76.png)

<br>
<br>

### iii)Shape of the Image
![shape ](https://user-images.githubusercontent.com/93978702/161279335-d360e0d7-de41-4a2a-963c-dea2d017a21c.png)

<br>
<br>

### iv)Access rows and columns
![size ](https://user-images.githubusercontent.com/93978702/161279946-76def3bb-05c8-4131-8ef3-e86d09a46e92.png)

<br>
<br>

### v)Cut and paste portion of image
![Cut Selection](https://user-images.githubusercontent.com/93978702/161280249-7ea34567-c1f1-426e-8f70-a1d8adfdb7b7.png)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


