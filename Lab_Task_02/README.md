**Task 2: Connected Component Labelling (CCL) – Explanation**
In this task, we used the binary image obtained from Task 1 to detect and count objects.
1️⃣ Concept of Connected Component Labelling
A connected component is a group of adjacent pixels that share the same value.
In a binary image, the white pixels (value 255) are considered foreground objects, and black pixels (value 0) are considered background.
Connected Component Labelling (CCL) assigns a unique label to each separate group of connected white pixels.
Purpose:
To identify and distinguish each individual object in an image.
To enable counting and further analysis of objects.

2️⃣ Steps Performed
1.Binary Image as Input:
oUsed the binary image from Task 1 where objects are white and the background is black.
2.Labeling Connected Components:
oEach group of connected white pixels is assigned a unique label (number).
oBackground pixels are labeled as 0.
3.Counting Objects:
oTotal objects are counted by subtracting 1 from the total number of labels (because one label is for the background).
4.Visualization (Optional):
oEach object can be displayed in a different color to easily see and verify the detected objects.

3️⃣ Key Observations
CCL works only on binary images, so converting the original image to binary is necessary.
It can handle multiple disconnected objects and count them automatically.
This technique is widely used in object detection, industrial inspection, medical imaging, and shape analysis.

4️⃣ Conclusion
By applying Connected Component Labelling, we can automatically detect and count objects in an image.
This task demonstrates the importance of binary images for object detection and the practical use of labeling techniques in image analysis.

