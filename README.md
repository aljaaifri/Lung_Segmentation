# 🫁 Automated Segmentation of Lung Lesions in Chest CT Using Hybrid Approaches

This project presents a **hybrid segmentation model** for detecting lung lesions (such as COVID-19 and cancer) in chest CT images. The model combines **traditional image processing techniques** with an advanced deep learning architecture (**SKICU-Net**) enhanced with **Selective Kernel (SK) blocks** and **attention mechanisms**.

---

## 📌 Features

- Automatic segmentation of lung lesions in CT scans
- Combines thresholding, K-means, and GMM with SKICU-Net
- Built-in attention modules to focus on critical image regions
- High segmentation accuracy (Dice ≈ 0.98, IoU ≈ 0.96)
- Visual explanations using Grad-CAM++
- Histogram & edge analysis for qualitative validation

---

## 🛠️ Technologies Used

- **Google Colab Pro** (TPU)
- **Python 3.11**
- **TensorFlow 2.18 + Keras 3.8**
- OpenCV (`cv2`)
- scikit-learn (`KMeans`, `GaussianMixture`)
- Matplotlib & Seaborn
- Multiprocessing
- Grad-CAM++

---

## 📂 Project Structure

lung-lesion-segmentation/
│
├── Auto_segmentation_SKICU_Net_with_attention.ipynb # Main notebook
├── data/ # Processed CT images and masks
├── models/ # Trained SKICU-Net model (optional)
├── results/ # Sample outputs (masks, overlays, CAMs)
└── README.md # This file

---

## 🚀 How to Run

1. Open the notebook in Google Colab:  
   [Open in Colab](https://colab.research.google.com)

2. Upload or link the CT dataset (e.g., COVIDx CT from Kaggle).

3. Run cells in order:
   - Preprocessing (crop, resize, clean)
   - Mask generation (threshold, K-means, GMM)
   - SKICU-Net model building & training
   - Evaluation & visualization (Dice, IoU, Grad-CAM++, Histogram)

---

## 📊 Results

| Metric        | Value     |
|---------------|-----------|
| Dice Score    | 0.9822    |
| IoU           | 0.9651    |
| F1-Score      | 0.9884    |
| Sensitivity   | 0.9880    |
| Specificity   | 0.9845    |
| Accuracy      | 0.9205    |

---

## 🧠 Visual Outputs

- ✅ Grad-CAM++ Heatmaps
- ✅ Predicted vs Traditional Masks
- ✅ Histogram Analysis
- ✅ Edge Detection Validation

---

## 📚 Citation

If you use this work in your research or academic setting, please cite:

> Raed Hamid Lateef. *Automated Segmentation of Lung Lesions in Chest Using Hybrid Approaches*. Al-Nahrain University, MSc Thesis, 2025.

---

## 📧 Contact

For questions or collaboration:  
📨 `raedhamid.engineer [at] gmail [dot] com`  
🏫 Biomedical Engineering Department, Al-Nahrain University

