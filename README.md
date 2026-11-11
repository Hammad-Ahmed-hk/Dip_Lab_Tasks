# Digital Image Processing (DIP): Lab Tasks

Python and OpenCV solutions for the Digital Image Processing course labs, plus an open-ended lab on skin cancer detection. Each folder has a Jupyter notebook and a README that explains the approach.

## Labs

| Folder | Topic |
|---|---|
| [`Lab 1`](Lab%201) | Colour component extraction, grayscale and binary images |
| [`Lab_Task_02`](Lab_Task_02) | Connected component labelling (counting objects in a binary image) |
| [`Lab 3,4`](Lab%203%2C4) | Histogram equalization and contrast stretching (built-in vs custom) |
| [`Lab 05`](Lab%2005) | Mean, median and Gaussian smoothing filters |
| [`Task_6`](Task_6) | Image smoothing and noise removal with spatial filters |
| [`Lab_Task_07`](Lab_Task_07) | Frequency-domain filtering with low-pass and high-pass filters |
| [`lab_Task_08`](lab_Task_08) | Image restoration and noise analysis (Gaussian, salt-and-pepper, motion blur) |
| [`Lab_Task_09`](Lab_Task_09) | Colour spaces (RGB, HSV, YCbCr, Lab) and segmentation |
| [`Lab_Task_10`](Lab_Task_10) | Image compression: Huffman coding and DCT, with CR, MSE and PSNR metrics |
| [`Lab_Task_11`](Lab_Task_11) | Morphological operations (erosion, dilation and related) |
| [`Lab_Task_12`](Lab_Task_12) | Grayscale conversion and thresholding |
| [`OEL_DIP`](OEL_DIP) | **Open-ended lab:** skin cancer detection on the PH2 dataset |

`Lab 1` and `Lab_Task_02` contain the same notebook, which covers Tasks 1 and 2.

## Tech stack

Python, OpenCV, NumPy, Matplotlib, SciPy, scikit-learn, Jupyter / Google Colab

## Running the notebooks

```bash
git clone https://github.com/Hammad-Ahmed-hk/Dip_Lab_Tasks.git
cd Dip_Lab_Tasks
pip install numpy opencv-python matplotlib scipy scikit-learn jupyter
jupyter notebook
```

Several notebooks were written for Google Colab and mount Google Drive to read images. If you run them locally, change the image paths to the sample images in each folder.

## Related repository

See also [Skin_Cancer_Detection](https://github.com/Hammad-Ahmed-hk/Skin_Cancer_Detection) for the skin cancer work.

## Author

Hammad Ahmed, [@Hammad-Ahmed-hk](https://github.com/Hammad-Ahmed-hk)
