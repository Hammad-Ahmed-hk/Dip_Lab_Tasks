Explanation of the Task
In this task, we performed image filtering using frequency domain techniques. The main goal was to understand how Low Pass Filters (LPF) and High Pass Filters (HPF) work on images and to compare different types of filters.
What we did step by step
1.Imported Libraries
We used:
NumPy for mathematical operations
OpenCV (cv2) for image handling
Matplotlib for displaying images
2.Loaded the Image
An image was loaded and converted into grayscale.
Grayscale images are easier to process in frequency domain.
3.Converted Image to Frequency Domain
We applied the 2D Fast Fourier Transform (FFT) to convert the image from:
Spatial domain → Frequency domain
The FFT was shifted so that low frequencies appear in the center.
4.Created Low Pass Filters (LPF) 
We implemented three types of LPFs:
Ideal Low Pass Filter
Allows only low frequencies inside a circular region.
Butterworth Low Pass Filter
Smooth transition between low and high frequencies.
Gaussian Low Pass Filter
Very smooth filtering without sharp edges.
🔹 LPFs remove high-frequency details, so the image becomes blurred.
5.Created High Pass Filters (HPF)
High pass filters were created by subtracting LPFs from 1.
Types used:
Ideal HPF
Butterworth HPF
Gaussian HPF
🔹 HPFs remove low-frequency components and highlight edges and fine details.
6.Applied Filters
Each filter mask was multiplied with the FFT of the image.
Then we applied Inverse FFT to convert the image back to spatial domain.
7.Displayed Results
The original image and all filtered images were displayed for comparison.
8.Spatial Domain Comparison
We also applied Gaussian Blur in spatial domain using OpenCV.
This helped us compare frequency domain filtering vs spatial filtering.
Conclusion
Low Pass Filters smooth the image and reduce noise.
High Pass Filters enhance edges and details.
Butterworth and Gaussian filters give smoother results than Ideal filters.
Frequency domain filtering provides more control compared to spatial filtering
