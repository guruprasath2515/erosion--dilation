# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import necessary packages

### Step2:
Create an empty window and add text to it
### Step3:
create a structuring element

### Step4:
Do the operation

### Step5:
Show the output image

 
## Program:
## DEVELOPED BY : GURU PRASATH R
## REG.NO : 212223040053
``` Python
# Import the necessary packages
import cv2
import numpy as np


# Create the Text using cv2.putText

img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'THALAPATHY',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element



# Erode the image

erode1= np.ones((5,5),np.uint8)
erode2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_erode1 = cv2.erode(img,erode1)
cv2.imshow('Eroded_image_1',image_erode1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_erode2 = cv2.erode(img,erode2)
cv2.imshow('Eroded_image_2',image_erode2)
cv2.waitKey(0)
cv2.destroyAllWindows()


# Dilate the image


dilate1= np.ones((5,5),np.uint8)
dilate2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_dilate1 = cv2.dilate(img,dilate1)
cv2.imshow('Dilated_image_1',image_dilate1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_dilated2 = cv2.dilate(img,dilate2)
cv2.imshow('Dilated_image_2',image_dilated2)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
## Output:

### Display the input Image


<img width="1736" height="418" alt="Screenshot 2025-11-12 220347" src="https://github.com/user-attachments/assets/c6c2ec20-a56b-400d-be5d-a55e013df9fa" />





### Display the Eroded Image

<img width="1754" height="432" alt="Screenshot 2025-11-12 220408" src="https://github.com/user-attachments/assets/9ecbc55c-9566-4361-847f-16a58e1cbdd6" />


<img width="1722" height="438" alt="Screenshot 2025-11-12 220431" src="https://github.com/user-attachments/assets/591477b8-f33f-4222-8153-49ff4ab56929" />


### Display the Dilated Image

<img width="1718" height="420" alt="Screenshot 2025-11-12 220446" src="https://github.com/user-attachments/assets/570d5af7-132c-413a-8497-d5200edb1d0c" />

<img width="1436" height="429" alt="Screenshot 2025-11-12 220459" src="https://github.com/user-attachments/assets/bdbb1b6e-8be5-4f70-b8f8-411f5b5e7726" />

## Result
Thus the generated text image is eroded and dilated using Python and OpenCV.
