# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
Jupyter lab
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
```python
# Developed By:S.MEENA
# Register Number;212221240028
```
# To Read,display the image
```
import cv2
color_img=cv2.imread('img.jpg',1)
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)
```

```
# To write the image
```
import cv2
color_img=cv2.imread('img.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)
```


```
# Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('img.jpg',1)
print(color_img.shape)
```

```
# To access rows and columns
```
import cv2
import random
color_img=cv2.imread('img.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)
```


```
# To cut and paste portion of image
```
import cv2
color_img=cv2.imread('img.jpg',-1)
tag=color_img[300:400,300:400]
color_img[50:150,50:150]=tag
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)
```









## Output:

### i) Read and display the image

![output](./ss5.png)

### ii)Write the image
![output](./ss3.png)

### iii)Shape of the Image

![output](./ss1.png)
### iv)Access rows and columns
![output](./ss4.png)
### v)Cut and paste portion of image
![output](./ss2.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


