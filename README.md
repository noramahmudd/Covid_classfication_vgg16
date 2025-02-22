# Covid Classification using VGG16

This project implements a **COVID-19 classification** model using the **VGG16** deep learning architecture. The model is trained to classify chest X-ray images into different categories: **COVID-19, Normal, and Pneumonia**.

## 📂 Dataset
The dataset consists of chest X-ray images categorized into:
- 🦠 **COVID-19 Positive**
- ✅ **Normal**
- 🏥 **Pneumonia**

Ensure that the dataset is properly structured before running the notebook.

## ⚙️ Installation & Requirements
To run this notebook, install the required dependencies using:

```bash
pip install tensorflow numpy matplotlib seaborn
```

You may also need **Jupyter Notebook** to run the `.ipynb` file:
```bash
pip install notebook
```

## 🚀 How to Run
1. Open the notebook:
   ```bash
   jupyter notebook Covid_classfication_vgg16.ipynb
   ```
2. Run the cells step by step to preprocess the dataset, train the VGG16 model, and evaluate performance.

## 🏗️ Model & Training
- **Pretrained VGG16** model is used with transfer learning.
- Fully connected layers are added for classification.
- The model is trained using **categorical cross-entropy** loss and **Adam optimizer**.

## 📊 Results
### 🔢 Performance Metrics
- **Train Loss:** `0.0537`
- **Test Loss:** `0.1175`
- **Train Accuracy:** `98.4%`
- **Test Accuracy:** `97%`

### 📉 Confusion Matrix
#### **Actual vs Predicted:**
```
 [[18  2  0]
 [ 0 20  0]
 [ 0  0 26]]
```
#### **Perfect Confusion Matrix:**
```
 [[20  0  0]
 [ 0 20  0]
 [ 0  0 26]]
```

### 📑 Classification Report
```
                  precision    recall  f1-score   support

         Normal       1.00      0.90      0.95        20
Viral Pneumonia       0.91      1.00      0.95        20
          Covid       1.00      1.00      1.00        26

       accuracy                           0.97        66
      macro avg       0.97      0.97      0.97        66
   weighted avg       0.97      0.97      0.97        66
```

## ✨ Author
**Nourhan Mahmoud**

---


