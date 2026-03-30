# Exp-6

### Developed by: DINESH S
### Register Number: 212224230069
# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## Program:

```
import cv2
import numpy as np
import matplotlib.pyplot as plt

import cv2
import numpy as np
import matplotlib.pyplot as plt


image = cv2.imread('mk.jpeg')  # Replace with your image path
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
# Original Image
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title('Original Image')
plt.axis('off')

```

### SOBEL EDGE DETECTOR
```
sobel_x = cv2.Sobel(gray_image, cv2.CV_64F, 1, 0, ksize=5)  # Sobel in x direction
sobel_y = cv2.Sobel(gray_image, cv2.CV_64F, 0, 1, ksize=5)  # Sobel in y direction
sobel_combined = cv2.magnitude(sobel_x, sobel_y)  # Combine both directions
plt.imshow(sobel_combined, cmap='gray')
plt.title('Sobel Edge Detection')
plt.axis('off')
```
### LAPLACIAN EDGE DETECTOR
```
laplacian = cv2.Laplacian(gray_image, cv2.CV_64F)
plt.imshow(laplacian, cmap='gray')
plt.title('Laplacian Edge Detection')
plt.axis('off')
```
### CANNY EDGE DETECTOR
```
canny_edges = cv2.Canny(gray_image, 50, 150)
plt.imshow(canny_edges, cmap='gray')
plt.title('Canny Edge Detection')
plt.axis('off')  
```

## Output:

<img width="401" height="508" alt="image" src="https://github.com/user-attachments/assets/ba8c967d-7eb9-44eb-9e64-c81b695eb1b6" />

<img width="424" height="524" alt="image" src="https://github.com/user-attachments/assets/39d9623f-700b-447c-851e-2ec0a268b921" />

<img width="411" height="518" alt="image" src="https://github.com/user-attachments/assets/c0ec03ef-1e8e-4487-8531-0da43582753f" />

<img width="452" height="521" alt="image" src="https://github.com/user-attachments/assets/e42efde1-f252-4044-b2b8-6645a176be68" />

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## Output:
### SOBEL EDGE DETECTOR

<img width="403" height="514" alt="image" src="https://github.com/user-attachments/assets/602e8bdf-0177-4507-9e8c-3c8e42264ba7" />


<img width="422" height="509" alt="image" src="https://github.com/user-attachments/assets/ad560f50-156d-4b5c-b52d-a979766d0b2d" />


### LAPLACIAN EDGE DETECTOR
<img width="391" height="503" alt="image" src="https://github.com/user-attachments/assets/dd90d947-f726-45db-bf77-83040b97265d" />

### CANNY EDGE DETECTOR
<img width="382" height="506" alt="image" src="https://github.com/user-attachments/assets/583881ad-f543-4184-9d45-9134e1e468c0" />


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
