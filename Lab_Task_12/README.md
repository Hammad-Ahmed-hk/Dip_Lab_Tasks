Image Processing Lab: Grayscale Conversion
Overview
This project demonstrates fundamental digital image processing techniques using Python in a Google Colab environment. The primary focus is on environment setup, image acquisition from external storage (Google Drive), and performing a color-space transformation from BGR to Grayscale.

Technical Workflow
1. Environment Setup
The script is designed to run in Google Colab and utilizes the following libraries:

OpenCV (cv2): Used for core image processing tasks such as reading and converting color spaces.

NumPy (np): Used for handling images as multi-dimensional arrays.

Matplotlib (plt): Used for high-quality image visualization within the notebook.

2. Google Drive Integration
To access image files stored externally, the script mounts Google Drive to the /content/drive directory.

3. Core Functionalities
The code contains a modular utility function for image visualization:

display_image(image, title):

Automatically detects if the input is a color (3-channel) or grayscale (1-channel) image.

For color images, it performs a necessary conversion from BGR (OpenCV's default) to RGB (Matplotlib's requirement) to ensure accurate color rendering.

Removes axis labels for a cleaner presentation.

4. Image Processing Steps
Loading: Reads an image from a specified path (e.g., /content/task_12.jpg) using cv2.imread.

Transformation: Converts the source image to grayscale using the cv2.COLOR_BGR2GRAY flag.

Visualization: Displays the final processed grayscale image.

How to Use
Mount Drive: Run the first cell and follow the authentication prompts to mount your Google Drive.

Set Path: Update the image_path variable with the actual path to your image file.

Execute: Run the notebook cells to see the original image converted and displayed in grayscale.
