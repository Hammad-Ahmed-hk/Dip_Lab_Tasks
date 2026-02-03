Lab 1 tasks for Digital Image Processing.
Task 1: Color Component Extraction, Grayscale, and Binary Images
1️⃣ Reading a Colored Image
We start by loading a colored image using OpenCV.
A colored image in computers is usually represented in RGB channels (Red, Green, Blue).
import cv2
from matplotlib import pyplot as plt

# Read a colored image
img = cv2.imread('your_image.jpg')  # BGR format in OpenCV
img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)  # Convert to RGB for display

2️⃣ Displaying Red, Green, and Blue Components Separately
Each colored image has three separate channels:
oRed channel: Shows the intensity of red color in the image.
oGreen channel: Shows the intensity of green color in the image.
oBlue channel: Shows the intensity of blue color in the image.
We can extract each channel:
# Extract R, G, B channels
R = img[:,:,0]
G = img[:,:,1]
B = img[:,:,2]

# Display channels
plt.figure(figsize=(10,3))
plt.subplot(1,3,1), plt.imshow(R, cmap='Reds'), plt.title('Red Channel')
plt.subplot(1,3,2), plt.imshow(G, cmap='Greens'), plt.title('Green Channel')
plt.subplot(1,3,3), plt.imshow(B, cmap='Blues'), plt.title('Blue Channel')
plt.show()
Purpose:
Helps us understand how each color contributes to the final image.
Useful in image processing tasks like color-based segmentation.

3️⃣ Creating a Grayscale Image
A grayscale image contains only shades of gray, where the intensity represents brightness.
It is computed as a weighted sum of R, G, B channels:
# Convert to grayscale
gray = cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)

# Display grayscale image
plt.imshow(gray, cmap='gray')
plt.title('Grayscale Image')
plt.show()
Purpose:
Simplifies the image by removing color information.
Useful for image analysis, edge detection, and filtering, where color is not important.

4️⃣ Creating a Binary Image
A binary image contains only two values: 0 (black) and 255 (white).
Created by applying a threshold to the grayscale image:
# Convert grayscale to binary using a threshold
_, binary = cv2.threshold(gray, 127, 255, cv2.THRESH_BINARY)

# Display binary image
plt.imshow(binary, cmap='gray')
plt.title('Binary Image')
plt.show()
Purpose:
Useful for detecting objects or regions in an image.
Simplifies analysis by reducing the image to only black and white pixels.

Explanation of What We Have Done in Task 1
1.Read a colored image:
oLoaded an image that contains Red, Green, and Blue color channels.
2.Separated R, G, B components:
oExtracted each color channel to see its contribution individually.
oRed channel shows red areas, Green shows green areas, Blue shows blue areas.
3.Created a grayscale image:
oCombined all three channels into a single intensity image.
oSimplifies the image while keeping brightness information.
4.Created a binary image:
oApplied a threshold on grayscale image.
oConverted the image to only black and white pixels.
oUseful for detecting shapes, objects, and edges.
✅ Skills Learned:
Understanding RGB color channels.
Converting colored images to grayscale and binary.
Image simplification for analysis.

