# Computer Vision Lab 2: Image Filtering & Effects

This project demonstrates various image processing techniques using OpenCV and custom kernels in Python. The notebook covers fundamental and advanced filtering operations on images, providing both code and visual results for each effect.

## Contents
- **Edge Detection & Sharpening**: Highlights edges and enhances details using convolution kernels.
- **Blurring & Smoothing**: Applies average and Gaussian blur to reduce noise and smooth images.
- **Embossing & Outline Effect**: Creates 3D and outline effects using emboss and outline kernels.
- **Sobel & Laplacian Transformation**: Detects horizontal, vertical, and all-direction edges.
- **High-pass & Low-pass Filtering**: Enhances or suppresses image details using custom kernels.
- **Motion Detection Effect**: Simulates motion blur and highlights diagonal edges.
- **Custom Artistic Filters**: Combines multiple kernels for creative effects.

## How to Run
1. Make sure you have Python 3.x installed.
2. Install required packages:
   ```bash
   pip install opencv-python matplotlib numpy
   ```
3. Place the sample image (`pika wallpaper.webp`) in the same directory as the notebook.
4. Open and run the notebook `24225013_himanshu_CV_Lab2.ipynb` cell by cell to see the results.

## Kernels Used
- **Edge Detection**: `[[ -1, -1, -1], [ -1, 8, -1], [ -1, -1, -1 ]]`
- **Sharpening**: `[[ 0, -1, 0], [ -1, 5, -1], [ 0, -1, 0 ]]`
- **Emboss**: `[[-2, -1, 0], [-1, 1, 1], [0, 1, 2]]`
- **Outline**: `[[ -1, -1, -1], [ -1, 8, -1], [ -1, -1, -1 ]]`
- **High-pass**: `[[ -1, -1, -1], [ -1, 9, -1], [ -1, -1, -1 ]]`
- **Low-pass**: `np.ones((5,5), np.float32) / 25`
- **Motion Blur**: Horizontal line kernel
- **Diagonal Edge**: `[[2, -1, -1], [-1, 2, -1], [-1, -1, 2]]`
- **Custom Artistic**: Sharpen + Emboss

## Results
Each section of the notebook displays the original and processed images side by side for easy comparison. You can experiment with different kernels and parameters to see their effects.

## Requirements
- Python 3.x
- OpenCV (`opencv-python`)
- NumPy
- Matplotlib

## Author
Himanshu Heda

---
*For academic use. Feel free to modify and experiment with the code for learning purposes.*
