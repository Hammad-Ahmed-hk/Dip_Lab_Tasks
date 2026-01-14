Color Space Analysis and Segmentation Using RGB, HSV, YCbCr, and Lab Color Models
📖 Introduction

This project demonstrates fundamental image processing techniques using different color spaces. The main objective is to analyze how various color models behave in segmentation tasks and to compare their effectiveness. Operations such as RGB channel extraction, color space conversion, white balance correction, and color masking are implemented and evaluated.

🎯 Objectives

The goals of this project are:

To extract Red, Green, and Blue (RGB) channels from an image

To convert an RGB image into HSV, YCbCr, and Lab color spaces

To apply white balance correction for illumination normalization

To perform color masking for object segmentation

To compare segmentation strength of different color spaces

🛠 Tools & Technologies

Programming Language: Python

Libraries Used:

OpenCV (cv2)

NumPy

Matplotlib

Platform: Jupyter Notebook / Google Colab / Python IDE

📂 Project Workflow
1️⃣ RGB Channel Extraction

The input image is split into its individual Red, Green, and Blue channels.
This helps analyze the contribution of each channel to the overall image appearance.

2️⃣ Color Space Conversion

The RGB image is converted into the following color spaces:

HSV (Hue, Saturation, Value)

Useful for color-based segmentation

Separates color information from brightness

YCbCr

Separates luminance (Y) from chrominance (Cb, Cr)

Commonly used in video processing

Lab (L*a*b*)

Device-independent color space

Effective under varying lighting conditions

3️⃣ White Balance Correction

White balance is applied using the Gray World Assumption, which assumes the average color of an image should be gray.
This step improves color consistency by reducing illumination effects.

4️⃣ Color Masking

Color masking is performed using thresholding techniques (e.g., in HSV color space) to isolate specific colors such as green.
This process is useful for object detection and segmentation.

5️⃣ Segmentation Strength Comparison

Segmentation results are compared across different color spaces:

Color Space	Segmentation Strength
RGB	Sensitive to lighting changes
HSV	Strong for color-based segmentation
YCbCr	Good luminance separation
Lab	Most robust under varying illumination
📊 Results & Observations

HSV provides better segmentation for color-based objects.

Lab color space performs well in varying lighting conditions.

RGB is less reliable for segmentation due to illumination dependency.

White balance improves overall segmentation accuracy.

📌 Conclusion

This project demonstrates that selecting the appropriate color space significantly improves segmentation performance. HSV and Lab color spaces outperform RGB for color-based segmentation tasks, especially under changing lighting conditions.
