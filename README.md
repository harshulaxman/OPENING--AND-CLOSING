# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.

### Step2:
Create the Text using cv2.putText.

### Step3:

Create the structuring element.
### Step4:
Use Opening operation.

### Step5:
Use Closing Operation.

 
## Program:
### DEVELOPED BY: Harsshitha lakshmanan
### REGISTER NO: 212223230075

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```


# Create the Text using cv2.putText
```
img = np.zeros((100, 550), dtype = 'uint8')
font = cv2.FONT_ITALIC
cv2.putText(img, 'MOUNIKA', (5,70), font, 2, (255), 5, cv2.LINE_AA)
n_img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
plt.imshow(n_img)
plt.axis("off")
```


# Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS, (11,11)
```
# Use Opening operation
```
image_open = cv2.morphologyEx(n_img, cv2.MORPH_OPEN, kernel)
plt.imshow(image_open)
plt.axis("off")

```
# Use Closing Operation
```
image_close = cv2.morphologyEx(n_img, cv2.MORPH_CLOSE, kernel)
plt.imshow(image_close)
plt.axis("off")



```
## Output:

### Display the input Image
<img width="579" height="122" alt="image" src="https://github.com/user-attachments/assets/8f6ce695-12ed-4a86-8243-37cd1b9e141b" />


### Display the result of Opening

<img width="575" height="116" alt="image" src="https://github.com/user-attachments/assets/0fe5ea29-9015-482a-a25d-4a60c17e0f3e" />



### Display the result of Closing

<img width="577" height="122" alt="image" src="https://github.com/user-attachments/assets/f6c8cee1-83dd-47ed-b6e3-3ead61f05414" />

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
