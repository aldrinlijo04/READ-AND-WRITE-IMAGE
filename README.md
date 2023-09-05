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

### Developed By:Aldrin Lijo J E
### Register Number: 212222240007

i) #To Read,display the image
```
import cv2
img = cv2.imread('dog.jpeg',1)
cv2.imshow('212222240007',img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```
img=cv2.imread('dog.jpeg',1)
cv2.imwrite('canine.png',img)

```
iii) #Find the shape of the Image
```

img=cv2.imread('dog.jpeg',0)
print(img.shape)

```
iv) #To access rows and columns

```
import random
img = cv2.imread('dog.jpeg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```
import cv2
import numpy as np
image = cv2.imread('dog.jpeg')
roi = image[50:100, 100:200]
image[50:100, 100:200]= roi
cv2.imwrite('part.jpeg', roi)
cv2.imshow('part.jpeg', roi)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

![dog](https://github.com/aldrinlijo04/READ-AND-WRITE-IMAGE/assets/118544279/5dd4d515-33b5-443c-8d46-5b355766e466)


<br>
<br>

### ii)Write the image
![canine](https://github.com/aldrinlijo04/READ-AND-WRITE-IMAGE/assets/118544279/c27241aa-dac0-47c7-88db-aaaf22b18127)


<br>
<br>

### iii)Shape of the Image
![Screenshot 2023-09-05 091741](https://github.com/aldrinlijo04/READ-AND-WRITE-IMAGE/assets/118544279/947bcdac-0030-4a22-a54d-f0d021d48b62)

<br>
<br>

### iv)Access rows and columns
![img2](https://github.com/aldrinlijo04/READ-AND-WRITE-IMAGE/assets/118544279/bffba0fa-6687-4367-9671-6087eb144c9a)

<br>
<br>

### v)Cut and paste portion of image

![img3](https://github.com/aldrinlijo04/READ-AND-WRITE-IMAGE/assets/118544279/c78f3ce6-b2f5-499f-9f7e-3caf397cd4b6)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
