Lab Task 03,and 04:Histogram Equalization and Contrast Stretching
Objective
To enhance the visual quality of an image using histogram equalization and contrast stretching techniques.
To compare the effectiveness of built-in vs custom histogram equalization.
To observe the effect of different contrast stretching transformations and compare them with histogram equalization.

1️⃣ Histogram Equalization
a) Concept
Histogram equalization improves image contrast by redistributing pixel intensity values.
Dark or washed-out images often have pixel intensities clustered in a small range.
HE spreads these intensities across the full range (0–255), enhancing image details.
b) Built-in Histogram Equalization
Used a library function to automatically equalize the image histogram.
Observed a contrast-enhanced image where details in dark and bright regions became more visible.
c) Custom Histogram Equalization
Performed manually following class steps:
1.Compute the histogram of the image (frequency of each pixel intensity).
2.Calculate the Cumulative Distribution Function (CDF) from the histogram.
3.Normalize the CDF to map intensity values to 0–255.
4.Transform the original image using the normalized CDF.
Observation:
The manually equalized image closely matched the built-in function result.
This step-by-step process helped understand how HE works internally.

2️⃣ Contrast Stretching
a) Concept
Contrast stretching expands the range of pixel intensities using linear or non-linear transformations, improving image visibility.
b) Applied Transformations
1.Linear Stretching: Maps minimum intensity to 0 and maximum to 255.
oEnhances overall contrast in a straightforward way.
2.Logarithmic Transformation: Expands darker pixels more than brighter ones.
oHighlights details in dark regions.
3.Gamma (Power-law) Transformation: Adjusts image brightness and contrast using a gamma value.
oHelps correct lighting conditions.
Observation:
Each transformation emphasized different intensity ranges.
Some transformations made dark areas brighter, while others preserved overall balance.

3️⃣ Comparison of Results
Enhancement Technique	Observation
Built-in Histogram Equalization	Quick and automatic; enhances contrast uniformly.
Custom Histogram Equalization	Manual method; results similar to built-in; shows internal working.
Linear Contrast Stretching	Simple; expands full intensity range; may not enhance local details.
Log Transformation	Brightens dark regions; enhances low-intensity details.
Gamma Transformation	Flexible control over brightness and contrast; can correct lighting issues.
Conclusion:
Histogram Equalization is ideal for uniform contrast enhancement.
Contrast Stretching provides more control over specific intensity ranges.
Comparing the methods helps choose the most suitable technique based on image characteristics.

4️⃣ Skills Learned
1.Understanding the histogram and its importance in image processing.
2.Applying built-in and manual histogram equalization.
3.Implementing contrast stretching using linear, logarithmic, and gamma transformations.
4.Comparing different techniques for image enhancement.
5.Observing the impact of enhancement on image details and visual quality.
Histogram Equalization and Contrast Stretching
Objective
To enhance the visual quality of an image using histogram equalization and contrast stretching techniques.
To compare the effectiveness of built-in vs custom histogram equalization.
To observe the effect of different contrast stretching transformations and compare them with histogram equalization.

1️⃣ Histogram Equalization
a) Concept
Histogram equalization improves image contrast by redistributing pixel intensity values.
Dark or washed-out images often have pixel intensities clustered in a small range.
HE spreads these intensities across the full range (0–255), enhancing image details.
b) Built-in Histogram Equalization
Used a library function to automatically equalize the image histogram.
Observed a contrast-enhanced image where details in dark and bright regions became more visible.
c) Custom Histogram Equalization
Performed manually following class steps:
1.Compute the histogram of the image (frequency of each pixel intensity).
2.Calculate the Cumulative Distribution Function (CDF) from the histogram.
3.Normalize the CDF to map intensity values to 0–255.
4.Transform the original image using the normalized CDF.
Observation:
The manually equalized image closely matched the built-in function result.
This step-by-step process helped understand how HE works internally.

2️⃣ Contrast Stretching
a) Concept
Contrast stretching expands the range of pixel intensities using linear or non-linear transformations, improving image visibility.
b) Applied Transformations
1.Linear Stretching: Maps minimum intensity to 0 and maximum to 255.
oEnhances overall contrast in a straightforward way.
2.Logarithmic Transformation: Expands darker pixels more than brighter ones.
oHighlights details in dark regions.
3.Gamma (Power-law) Transformation: Adjusts image brightness and contrast using a gamma value.
oHelps correct lighting conditions.
Observation:
Each transformation emphasized different intensity ranges.
Some transformations made dark areas brighter, while others preserved overall balance.

3️⃣ Comparison of Results
Enhancement Technique	Observation
Built-in Histogram Equalization	Quick and automatic; enhances contrast uniformly.
Custom Histogram Equalization	Manual method; results similar to built-in; shows internal working.
Linear Contrast Stretching	Simple; expands full intensity range; may not enhance local details.
Log Transformation	Brightens dark regions; enhances low-intensity details.
Gamma Transformation	Flexible control over brightness and contrast; can correct lighting issues.
Conclusion:
Histogram Equalization is ideal for uniform contrast enhancement.
Contrast Stretching provides more control over specific intensity ranges.
Comparing the methods helps choose the most suitable technique based on image characteristics.

4️⃣ Skills Learned
1.Understanding the histogram and its importance in image processing.
2.Applying built-in and manual histogram equalization.
3.Implementing contrast stretching using linear, logarithmic, and gamma transformations.
4.Comparing different techniques for image enhancement.
5.Observing the impact of enhancement on image details and visual quality.

