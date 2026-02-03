Task_nmb_05:
1️⃣ Applying Mean, Median, and Gaussian Filters
What we did:
We applied three types of smoothing filters to reduce noise in the image.
1.Mean Filter (Average Filter): Replaces each pixel with the average of its neighbors.
Good for general smoothing, but can blur edges.
2.Median Filter: Replaces each pixel with the median of its neighbors.
Very effective for salt & pepper noise because it removes outliers without blurring edges.
3.Gaussian Filter: Uses a weighted average giving more importance to central pixels.
Smoothens the image and reduces Gaussian noise.
Purpose:
Compare different smoothing filters and see how they affect image clarity and noise reduction.

2️⃣ Applying Laplacian for Sharpening
What we did:
Applied the Laplacian operator which calculates the second derivative of the image.
Adding the Laplacian to the original image enhances edges and details, making it sharper.
Purpose:
To highlight edges and fine details that may be lost during smoothing.

3️⃣ Implementing a 3×3 Custom Convolution Kernel
What we did:
Created our own 3×3 matrix (kernel) to apply a custom effect.
Example kernel used:
[[ 0, -1,  0],
 [-1,  5, -1],
 [ 0, -1,  0]]
This kernel acts like a sharpening filter, enhancing edges and contrasts.
Purpose:
Learn how custom kernels can manipulate images in different ways (sharpen, blur, detect edges).

4️⃣ Comparing Noise Removal of Each Filter
What we did:
Added two types of synthetic noise to the image:
1.Salt & Pepper Noise: Random white and black pixels.
2.Gaussian Noise: Random small variations in pixel intensity.
Applied appropriate filters to remove noise:
oMedian Filter for Salt & Pepper → best because it removes outliers without blurring edges.
oGaussian Filter for Gaussian noise → best because it smooths the random variations effectively.
Purpose:
Observe how different filters handle different types of noise.
Understand the strengths and limitations of each filter.

5️⃣ Identifying the Best Filter
Salt & Pepper Noise → Median Filter is best.
Gaussian Noise → Gaussian Filter is best.
Conclusion:
Different types of noise require different filtering techniques.
Understanding the properties of each filter helps in choosing the most effective one for a specific problem.

✅ Summary of Skills Learned in this Lab:
1.Applying spatial filters to smooth or sharpen images.
2.Using Laplacian for edge enhancement.
3.Designing and applying custom convolution kernels.
4.Adding synthetic noise and analyzing filter performance.
5.Choosing the best filter based on the type of noise.

