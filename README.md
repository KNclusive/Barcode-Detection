# Barcode-Detection
This repository is for an Computer Vision task of barcode detection in Images without using ML/ DL approaches.
This repository contains combination of image thresholding, edge detection and morphological operations to detect a bar code in an image.

### Steps to Barcode-Detection
* Convert Image to Grey-Scale.
* Calculate Image Gradients : cv2.Sobel (Horizontal and Vertical gradients) / cv2.Laplacian.
* Blur the image (Noise and other small gradients removal).
* Convert to binary Image (Thresholding both manual and automatic).
* Perform erosion and dilation (For defining Box Shape Area where the barcode is).
* Barcode Detection by drawing contour over largest Object in the processed image.

### Extras
* A peak into a better approach for edge detection (Canny filter).
