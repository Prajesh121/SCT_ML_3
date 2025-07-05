# Defect Detection in Packaged Products (SVM + HOG)

**Internship Project Task 3 – Handpac India Pvt. Ltd.**

This project demonstrates a prototype for **detecting defective vs good packaged products** using image-based machine learning.  
It repurposes a classic Cat vs Dog SVM pipeline and applies it to manufacturing: classify images as `good` or `defective`.

---

## 📁 Dataset
- **Source:** You can reuse an image dataset (e.g., Cat vs Dog samples) and remap categories to `good`/`defective`, or collect sample images from the factory.
- **Expected layout:** `data/images/good/` and `data/images/defective/`. Put JPEG/PNG images in these folders.
- **Note:** Do not push large image datasets to GitHub. Instead include a small sample and instructions to obtain the full dataset if required.

---

## 🛠️ Approach
1. Preprocess images (resize, grayscale)
2. Extract HOG (Histogram of Oriented Gradients) features per image
3. Train SVM classifier (GridSearchCV over linear and RBF kernels)
4. Evaluate using accuracy, confusion matrix, and classification report
5. Save trained model (`models/svm_defect_model.pkl`)

---

## 📂 Files
- `notebooks/defect_detection_svm.ipynb` — full notebook (code + visualizations)
- `src/train_svm.py` — standalone training script
- `data/images/` — expected local image folders (`good/`, `defective/`)
- `models/svm_defect_model.pkl` — saved model (after training)
- `README.md` — this file

---

## ▶️ How to run (local)
1. Install dependencies:
```bash
pip install -r requirements.txt
