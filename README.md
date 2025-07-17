# 🗑️ AI-Based Waste Segregation

This project uses a **Convolutional Neural Network (CNN)** to classify waste into 6 categories using the **TrashNet dataset**.

## 📂 Dataset
- **TrashNet Dataset (resized version)** with classes:
  - Cardboard, Glass, Metal, Paper, Plastic, Trash

## 📊 Results
- **Before Augmentation:** 55% validation accuracy  
- **After Augmentation:** 64% validation accuracy  
- Correctly predicted test images (e.g., *Metal ✅*)

## 📎 Files in this Repo
- `AI_waste_segregation.ipynb` → Full training notebook  

⚠️ **The trained model is too large for GitHub. You can download it from Google Drive:**  
👉 [Download waste_model_improved.h5](https://drive.google.com/file/d/1fQa9ajzWk_86efmVmYJQJ-3izQj5GWr5/view?usp=sharing)  
👉 [Download waste_model_improved.keras](https://drive.google.com/file/d/183c9_UIjR-d7bKF_4Ya6yLK8phhXm42O/view?usp=sharing)  

You can also **retrain the model** by running the notebook.

## 🔗 How to Load Model
```python
from tensorflow.keras.models import load_model
model = load_model("waste_model_improved.h5")
