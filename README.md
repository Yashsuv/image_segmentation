## Morphological Transformations in Image Preprocessing

### 👥 Team Members:

* **Sholwyn** – Roll No: 4SO22CD050
* **Sruthi** – Roll No: 4SO22CD053
* **Yash** – Roll No: 4SO22CD063

---

### 📌 Problem Statement:

In many image processing tasks, raw images suffer from noise, irregular shapes, and low feature visibility, making it difficult to perform accurate object detection and segmentation. Morphological transformations provide a set of powerful tools to refine image structures, remove noise, and highlight essential shapes, thereby improving the performance of subsequent analysis and computer vision applications.
---

### 🔁 Program Flow & Techniques:

1. **Original Image Loading**

   * **Input**: MRI brain scan images (grayscale or color).
   * **Purpose**: Serves as the baseline for all further processing.

2. **CLAHE Enhancement**

   * **Technique**: Contrast Limited Adaptive Histogram Equalization
   * **Purpose**: Enhances local contrast to better define tumor boundaries.

3. **Edge Detection**

   * **Technique**: Canny or Sobel Edge Detector
   * **Purpose**: Highlights boundaries of tissues and tumors.

4. **HOG Feature Extraction**

   * **Technique**: Histogram of Oriented Gradients
   * **Purpose**: Captures gradient and texture features critical for tumor structure recognition.

5. **K-means Clustering**

   * **Technique**: Unsupervised clustering (k=2 or 3)
   * **Purpose**: Segments image into clusters (tumor vs. non-tumor regions).

6. **Random Forest Segmentation**

   * **Technique**: Supervised machine learning (Random Forest Classifier)
   * **Purpose**: Trains on labeled data to improve segmentation accuracy.

7. **Watershed Segmentation**

   * **Technique**: Watershed Algorithm
   * **Purpose**: Refines object boundaries, especially useful for overlapping regions.

8. **Final Segmentation Mask**

   * **Combination**: Best segmentation outputs are merged to form a binary mask highlighting tumor regions.

9. **Overlay and Visualization**

   * **Technique**: Color mask overlay using OpenCV or Matplotlib
   * **Purpose**: Clearly highlights tumor regions on the original MRI image.

---

### 🧰 Technologies Used:

* **Python 3.x**
* **OpenCV**
* **NumPy**
* **Matplotlib**
* **scikit-image**
* **scikit-learn**
* **pandas**
* **scipy**

---

### 📦 Installation:

Install all project dependencies using:

```bash
pip install -r requirements.txt
```
