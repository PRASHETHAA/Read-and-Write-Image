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
```

import cv2
image_1=cv2.imread("pic_1.PNG")
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)

```
ii) #To write the image
```

cv2.imwrite("pic_1.jpg",image_1)

```
iii) #Find the shape of the Image
```python3

print(image_1.shape)

```
iv) #To access rows and columns

```python3

for i in range(110,140):
    for j in range(115,140):
        image_1[i][j]=[0,0,0]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3

image_1[110:140,115:140]=image_1[150:180,115:140]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

![Screenshot (20)](https://user-images.githubusercontent.com/75234942/161495510-d00e977c-8bdb-4155-8344-a64de35573d5.png)

### ii)Write the image

![Screenshot (19)](https://user-images.githubusercontent.com/75234942/161495534-351f8a33-cc1b-4ea3-8342-0cc6c43e2375.png)

### iii)Shape of the Image

![Screenshot (21)](https://user-images.githubusercontent.com/75234942/161495599-0c0244b2-957b-4e03-9f3c-92c4a420ddc9.png)

### iv)Access rows and columns

![Screenshot (22)](https://user-images.githubusercontent.com/75234942/161495625-8dd163fe-272e-436d-8ab8-c997e4f4b942.png)

### v)Cut and paste portion of image

![Screenshot (23)](https://user-images.githubusercontent.com/75234942/161495682-aca7221e-f1a5-4b81-a98a-389501f541fd.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


