# README: Image Manipulation and Processing

## **Task 1: Understanding and Manipulating an Image**
This task involves basic operations to read, analyze, and transform an image using OpenCV.

### **1.1 Read the Image**
- Load an image using OpenCV (`cv2.imread()`).

### **1.2 Display the Image**
- Use `cv2.imshow()` to visualize the image.

### **1.3 Extract Image Size**
- Retrieve dimensions (width, height, channels) using `.shape` attribute.

### **1.4 Calculate Image Pixels**
- Compute the total number of pixels as `width × height`.

### **1.5 Convert RGB to Grayscale**
- Convert the image from BGR to Grayscale using `cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)`.

### **1.6 Convert RGB to Grayscale and Binary Image (Thresholding)**
- Apply a binary threshold using `cv2.threshold()`, setting pixels above the threshold to white and below it to black.
- **Count the area of black pixels** and extract the image size.

#### **📌 Note:**
- OpenCV loads images in **BGR format** by default.
- Convert images to **RGB format** before processing.
- Save each transformed image with a **new filename**.

---

## **Task 2: Understanding and Manipulating Image Properties**
This task focuses on edge detection and segmentation techniques for analyzing images.

### **2.1 Perform Edge Detection Using Operators**
- **Sobel Operator** (`cv2.Sobel()`): Detects edges by computing gradients.
- **Prewitt Operator** (Implemented manually using convolution filters).
- **Roberts Cross Operator** (Another gradient-based edge detection technique).
- **Canny Edge Detector** (`cv2.Canny()`): Multi-stage algorithm for accurate edge detection.

### **2.2 Perform Image Segmentation Techniques**
- **Global Thresholding for Image Segmentation** (`cv2.threshold()`): Separates objects based on intensity.
- **Adaptive Thresholding** (`cv2.adaptiveThreshold()`): Applies different thresholds to different image regions.
- **Edge Detection-Based Segmentation (Canny Edge Detection)**: Uses edges as boundaries for segmentation.
- **Region-Based Segmentation (Watershed Algorithm)** (`cv2.watershed()`): Identifies object boundaries based on distance maps.

---

## **Libraries Used**
- **OpenCV (`cv2`)**: For image processing.
- **NumPy (`numpy`)**: For numerical operations.
- **Matplotlib (`matplotlib.pyplot`)**: For visualizing images.

---

## **Execution Steps**
1. Ensure OpenCV and NumPy are installed:
   ```bash
   pip install opencv-python numpy matplotlib
   ```
2. Run the Python script for image processing:
   ```bash
   python image_processing.py
   ```
3. View the processed images saved with new filenames.

---

## **Author**
*Ayush Singh*

---
📌 **Ensure all processed images are saved and included in the submission.**

