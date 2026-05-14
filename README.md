# Implementation-of-Erosion-and-Dilation
## Reg no: 212224230073
## Name: GAYATHRI S
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
#### Step1:<br>
Import the necessary pacakages

#### Step2:<br>
Create the text using cv2.putText

#### Step3:<br>
Create the structuring element

#### Step4:<br>
Erode the image

#### Step5: <br>
Dilate the Image
 
## Program:
 
 Name: GIRITHICK ROHAN

 Reg.No:  212223230063
 
 Python
 Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((300, 600, 3), dtype="uint8")
```
 Create the Text using cv2.putText
```
text = "GAYATHRI"
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, text, (50, 150), font, 2, (255, 255, 255), 3)
```
 Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
plt.figure(figsize=(10, 5))
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```
 Erode the image
```
eroded_image = cv2.erode(image, kernel, iterations=1)
plt.imshow(eroded_image_rgb)
plt.title("Eroded Image")
plt.axis("off")
```
 Dilate the image
```
dilated_image = cv2.dilate(image, kernel, iterations=1)
plt.imshow(dilated_image_rgb)
plt.title("Dilated Image")
plt.axis("off")
```

## Output:

### Display the input Image
<img width="555" height="602" alt="image" src="https://github.com/user-attachments/assets/f7497459-016a-4267-a901-c8a714d04530" />


### Display the Eroded Image

<img width="622" height="605" alt="image" src="https://github.com/user-attachments/assets/8951bcb0-dd0e-46a0-a894-b50fb17a6853" />

### Display the Dilated Image

<img width="561" height="602" alt="image" src="https://github.com/user-attachments/assets/18280c19-ac69-4aab-a855-f2ce1d0c2dcf" />

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
