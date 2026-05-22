# IMPLEMENTATION-OF-EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
Anaconda - Python 3.7
OpenCV

## Algorithm:
# Step 1:
Import necessary libraries, including OpenCV (cv2) and Matplotlib (plt), to load, manipulate, and display images.

# Step 2:
Use cv2.putText() to add text to the image at a specific location with chosen font, size, color, and thickness.

# Step 3:
Define a structuring element using cv2.getStructuringElement() to specify the shape and size for morphological transformations.

# Step 4:
Apply erosion to the image using cv2.erode() with the structuring element to shrink white regions and reduce noise.

# Step 5:
Dilate the eroded image using cv2.dilate() with the structuring element to expand white regions and enhance features.

# Step 6:
Display the original and processed images using plt.imshow() with proper axis configuration and titles for comparison.

# Step 7:
Finalize by calling plt.show() to display all images in a single figure for easy visualization and comparison.

## Program:
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((300, 600, 3), dtype="uint8")
Create the Text using cv2.putText

text = "clarissa"
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, text, (50, 150), font, 2, (255, 255, 255), 3)
Create the structuring element

kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
plt.figure(figsize=(10, 5))
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
Erode the image

eroded_image = cv2.erode(image, kernel, iterations=1)
plt.imshow(eroded_image_rgb)
plt.title("Eroded Image")
plt.axis("off")
Dilate the image

dilated_image = cv2.dilate(image, kernel, iterations=1)
plt.imshow(dilated_image_rgb)
plt.title("Dilated Image")
plt.axis("off")
```

## Output:
# Display the input Image

<img width="473" height="475" alt="image" src="https://github.com/user-attachments/assets/e9acfa24-aeb3-4926-a3d1-6e90c22c308e" />

# Display the Eroded Image

<img width="457" height="471" alt="image" src="https://github.com/user-attachments/assets/f2c48a6c-1dd5-4a22-8c50-ca0d445aabb1" />

# Display the Dilated Image

<img width="541" height="478" alt="image" src="https://github.com/user-attachments/assets/96c13024-3b5e-4615-accc-11104fd199ef" />

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.



