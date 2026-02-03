**Skin Cancer Detection using PH2 Dataset**
Overview
This project implements an automated system for Skin Cancer Detection focusing specifically on the PH2 dataset. The system utilizes Digital Image Processing (DIP) techniques to analyze dermoscopic images, identify lesion areas, and extract features to assist in the diagnosis of melanoma.

Author: 2023-SE-01

Course: Digital Image Processing

Dataset: PH2
The project utilizes the PH2 Dataset, a dermoscopic image database acquired at the Dermatology Service of Hospital Pedro Hispano.

Image Format: 8-bit RGB color images.

Content: Clinical diagnosis, dermoscopic criteria (asymmetry, pigment network, etc.), and the manual segmentation of the lesion (ground truth).

Project Workflow
1. Data Preparation and Environment
The notebook is designed for execution in a Google Colab environment. It handles the mounting of Google Drive and navigates a specific folder hierarchy to access images and their corresponding lesion masks.

Project Path: /content/drive/MyDrive/OEL

Data Structure: Organized by folder (e.g., IMD002), containing subfolders for the original image and the ground truth lesion mask.

2. Image Acquisition & Pre-processing
The code reads .bmp files and utilizes OpenCV for initial processing.

Image Loading: Iterates through dataset directories to fetch dermoscopic images and ROI (Region of Interest) masks.

Visualization: Includes modules to display the original clinical image side-by-side with the binary lesion mask for verification.

3. Feature Extraction & Classification
(Based on the code logic and evaluation metrics) The system prepares data for classification by comparing processed images against the ground truth. While the specific classifier parameters are flexible (e.g., Random Forest or SVM), the methodology focuses on distinguishing melanoma from benign lesions using extracted dermoscopic features.

4. Performance Evaluation
The project measures success using standard medical diagnostic metrics:

Accuracy: The overall correctness of the model.

Sensitivity (Recall): The ability of the model to correctly identify patients with melanoma.

Specificity: The ability of the model to correctly identify patients who do not have melanoma.

Requirements
To run this notebook, the following libraries are required:

numpy

opencv-python

matplotlib

scikit-learn

google-colab (for Drive mounting)

How to Run
Mount Drive: Ensure your PH2 dataset is located in My Drive/OEL/PH2Dataset/.

Execute Cells: Run the cells sequentially to load the images and visualize the masks.

Analysis: The final cells will output the evaluation metrics (Accuracy, Sensitivity, Specificity) based on the model's predictions.

Results
The system evaluates performance using the confusion matrix. Example results indicated in the notebook target high sensitivity to ensure no potential melanoma cases are missed during the screening process.
