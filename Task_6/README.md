Task number 06:
Title
Image Smoothing and Noise Removal Using Spatial Filters

Objective
The objective of this task is to study and compare different image smoothing filters used for noise reduction in digital images.

Tools and Software Used
Python
OpenCV (cv2)
NumPy
Matplotlib

Methodology
1.Image Loading
Two images were loaded using OpenCV. The images were converted from BGR format to RGB format for correct visualization.
2.Original Image Display
The original images were displayed to observe their quality before applying any filtering techniques.
3.Mean Filtering
A 5×5 Mean filter was applied to the images. This filter reduces noise by averaging the values of neighboring pixels, but it also causes blurring of edges.
4.Median Filtering
A 5×5 Median filter was applied to the images. This filter replaces each pixel with the median value of surrounding pixels and is effective in removing salt-and-pepper noise while preserving edges.
5.Gaussian Filtering
A 5×5 Gaussian filter was applied. This filter smooths the image using a Gaussian distribution and provides smoother results with less distortion.
6.Result Comparison
The original images and the filtered images were displayed side by side to compare the effects of each filter.

Results and Discussion
The Mean filter reduced noise but caused noticeable blurring. The Median filter performed better in preserving edges and removing impulse noise. The Gaussian filter produced smooth and visually pleasing results with balanced noise reduction and edge preservation.

Conclusion
In this task, image smoothing was successfully performed using Mean, Median, and Gaussian filters. Among the three, the Median and Gaussian filters gave better results compared to the Mean filter. This experiment helped in understanding the importance of selecting an appropriate filter for noise reduction in image processing.

