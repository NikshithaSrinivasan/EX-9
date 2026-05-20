# EX-9
# EXP-9 Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import required libraries (OpenCV, NumPy) and load the image in grayscale.
### Step2:
Define a structuring element (kernel) for morphological operations.
### Step3:
Apply erosion using cv2.erode() on the image with the defined kernel.
### Step4:
Apply dilation using cv2.dilate() on the image with the same kernel.
### Step5:
Display and compare the original, eroded, and dilated images
## Program:
# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Input Image with Text
```
#NAME: NIKSHITHA S
#REG NO: 212224040220
import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'MONISH', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB for displaying
plt.title("Input Image with Text")
plt.axis('off')
```
# Erode the image
```
#NAME: NIKSHITHA S
#REG NO: 212224040220
kernel = np.ones((3, 3), np.uint8)
eroded_image = cv2.erode(image, kernel, iterations=1)

plt.imshow(cv2.cvtColor(eroded_image, cv2.COLOR_BGR2RGB))
plt.title("Eroded Image")
plt.axis('off')
```
# Dilate the image
```
#NAME: POOJA P
#REG NO: 212224230195
dilated_image = cv2.dilate(image, kernel, iterations=1)


plt.imshow(cv2.cvtColor(dilated_image, cv2.COLOR_BGR2RGB)) 
plt.title("Dilated Image")
plt.axis('off')

```
## Output:

### Display the input Image
<img width="274" height="285" alt="image" src="https://github.com/user-attachments/assets/439225d3-e47f-4695-8d76-4ef26c8920d7" />



### Display the Eroded Image
<img width="269" height="292" alt="image" src="https://github.com/user-attachments/assets/aa352edb-53c9-46c4-a22c-847dbb64c5ad" />



### Display the Dilated Image
<img width="270" height="285" alt="image" src="https://github.com/user-attachments/assets/8a5f7c88-dd10-4fb0-b3ac-5f00792442a4" />


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
