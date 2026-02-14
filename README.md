# Image Stitching & Panorama Construction 📷

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter&logoColor=white)

##  Overview
This project implements **Image Stitching** techniques to combine a series of overlapping images into a single, high-resolution panoramic image. Developed using **Python** and **OpenCV**, the system automatically detects features, matches them between images, and blends them seamlessly to create a wide-angle view.

##  Key Features
* **Automated Sorting:** Intelligently sorts input files numerically (e.g., `1.jpeg`, `2.jpeg`, ...) to ensure the correct stitching order.
* **Feature Detection:** Utilizes **SIFT (Scale-Invariant Feature Transform)** to identify unique keypoints in each image.
* **Feature Matching:** Implements **KNN (K-Nearest Neighbors)** and **RANSAC** to find correct correspondences between overlapping images.
* **Homography & Warping:** Calculates the transformation matrix to align images perfectly.
* **Seamless Blending:** Merges images while minimizing exposure differences and artifacts.

##  Dataset
The project uses a sequence of 6 overlapping images taken in a boat scenario.
* **Source:** `/kaggle/input/datasets/jauhanahmad/gambar/img/`
* **Format:** `.jpeg`

##  Results & Visualization

### 1. Keypoint Detection & Feature Matching
Before stitching, the system analyzes the images to find common points.
![Feature Matching](laporan_matches.jpg)
*Figure 1: Visualization of feature matching between two adjacent images.*

### 2. Final Panorama
The final result after stitching 6 input images:
![Final Panorama](hasil_panorama.jpg)
*(Note: Please ensure you upload your result image to this repository and update the filename above)*

## 🛠️ Installation & Usage

### Prerequisites
Ensure you have Python installed. Install the required dependencies:

```bash
pip install opencv-python numpy matplotlib
