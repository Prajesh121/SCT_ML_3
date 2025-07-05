# Defect Detection in Packaged Products using SVM

**Internship Project Task 3 – Handpac India Pvt. Ltd.**

This project demonstrates **image-based defect detection in packaged products** using a Support Vector Machine (SVM).  
It was completed as part of a machine learning internship.

---

## 📊 Features Used

| Feature                  | Description                                             |
|---------------------------|---------------------------------------------------------|
| Flattened image pixels    | Input features derived from resized images (64x64 px) |
| Target                    | `Good Product` vs `Defective Product`                  |

**Note:** The dataset uses images of cats and dogs repurposed to simulate good vs defective packages.

---

## 📁 Dataset

- Folder: `train/` containing images  
- Classes: `Good Product` and `Defective Product`  
- Limit: 500 images per class for faster training  
- Images are resized to **64x64 pixels** and flattened for SVM input  

**Optional:** You can expand the dataset with real packaging images for better accuracy.

---

## 🛠️ Tech Stack

- Python  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-Learn (SVM)  
- Jupyter Notebook  

---

## 📈 Output

- **SVM Model** trained to classify packages as good or defective  
- **Evaluation Metrics:**  
  - Accuracy  
  - Classification Report (Precision, Recall, F1-score)  
- **Visualization:** Sample images with predicted labels  

---

## 🔍 How to Run

1. Clone the repository:
```bash
git clone https://github.com/Prajesh121/SCT_ML_3.git
