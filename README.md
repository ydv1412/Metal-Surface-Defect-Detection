# 🏭 Metal Surface Defect Detection

## 📌 Overview
This project aims to automate **metal surface defect detection** using **deep learning (CNN) and machine learning (SVM, Random Forest)** models. The objective is to classify defects in hot-rolled steel strips, improving quality control in manufacturing.

### 🔍 **Problem Statement**
Manual inspection of metal surfaces is **time-consuming, error-prone, and inefficient** for large-scale industries. This project automates **defect classification** using the **NEU Metal Surface Defects Dataset**, improving prediction and scalability.

---

## 📂 Dataset
We used the **NEU Metal Surface Defects Dataset**, which contains **6 defect types**:
- **Crazing**: Cracks on the metal surface.
- **Inclusion**: Embedded foreign particles.
- **Patches**: Irregular metal areas.
- **Pitted Surface**: Small, deep corroded holes.
- **Rolled-in Scale**: Embedded mill scale from rolling.
- **Scratches**: Surface abrasions.

### 📊 **Dataset Distribution**
- **Training**: 276 images per defect (Total: 1656)
- **Validation**: 12 images per defect (Total: 72)
- **Testing**: 12 images per defect (Total: 72)
- **Total Images**: **1800**

### 📏 **Image Characteristics**
- **Aspect Ratio**: All images are **square (1:1)**.
- **Pixel Intensity**: Most images have medium brightness.
- **Entropy**: Most images have moderate texture complexity.
- **Signal-to-Noise Ratio (SNR)**: High to moderate noise.

---

## ⚙️ **Models Implemented**
### **1️⃣ Convolutional Neural Network (CNN)**
- Achieved **96% accuracy** on test data.
- Mean f1 score was **96** on test data.
- Learned **feature embeddings** to differentiate between defects.
- Used **feature maps** to visualize model learning.

### **2️⃣ Support Vector Machine (SVM)**
- Achieved **80.55% accuracy**.
-  Mean f1 score was **88** on test data.
- Performed better than Random Forest.

### **3️⃣ Random Forest**
- Achieved **67.40% accuracy**.
- Mean f1 score was **72** on test data.
- Struggled with complex patterns.

### **🔍 Performance Comparison**
| Model  | Accuracy |   f1 Score |   
|--------|----------|------------|
| **CNN**  | **96.0%** | 96      |
| **SVM**  | 80.5% |     88      |
| **Random Forest** | 67.4% | 72 |

📌 **Observations:**
- **CNN outperforms ML models** because it learns spatial patterns effectively.
- **SVM performs better than Random Forest** due to better handling of high-dimensional data.
- Models struggle to differentiate **Scratches vs. Patches** and **Pitted vs. Inclusion** due to similarity.

---

## 🚀 **Installation & Setup**
### **🔹 Step 1: Clone the Repository**
```bash
git clone https://github.com/ydv1412/metal-surface-defect-detection.git
cd metal-surface-defect-detection

