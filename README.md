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
```python
# Developed By:S.MEENA
# Register Number;212221240028
# To Read,display the image
import cv2
color_img=cv2.imread('img.jpg',1)
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)



# To write the image
import cv2
color_img=cv2.imread('img.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221240028,S.MEENA',color_img)
cv2.waitKey(0)




# Find the shape of the Image
import cv2
import random
color_img=cv2.imread('img.jpg',1)
print(color_img.shape)



# To access rows and columns
import cv2
import random
color_img=cv2.imread('img.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('cimg',color_img)
cv2.waitKey(0)




# To cut and paste portion of image
import cv2
color_img=cv2.imread('img.jpg',-1)
tag=color_img[300:400,300:400]
color_img[50:150,50:150]=tag
cv2.imshow('cimg',color_img)
cv2.waitKey(0)









```
## Output:

### i) Read and display the image

<br>
![Screenshot (9)](https://user-images.githubusercontent.com/94677128/160786173-a929c539-79fa-47b1-82fe-5a0de56a62c5.png)

<br>

### ii)Write the image

<br>
![Screenshot (13)](https://user-images.githubusercontent.com/94677128/160787251-6cdfddd6-d369-4a7e-a18b-37c641cc6d1f.png)

<br>

### iii)Shape of the Image

<br>
![Screenshot (10)](https://user-images.githubusercontent.com/94677128/160787345-04e26a36-7fc8-45f4-91e2-32b3ebb41cd6.png)

<br>

### iv)Access rows and columns
<br>
![Screenshot (12)](https://user-images.githubusercontent.com/94677128/160787480-97479314-aabd-4016-bbd3-ec133602f13f.png)

<br>

### v)Cut and paste portion of image
<br>
![Screenshot (11)](https://user-images.githubusercontent.com/94677128/160787585-57e6e10a-dc58-4a20-9ff6-9aeac8601608.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


