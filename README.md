# 🍓 Strawberry Ripeness Classification using MobileNetV2  
**Team2_Zelbytes** | AI & Data Science Internship @ Zelbytes Pvt. Ltd.

---

### 👥 Team Details
- **Team Name**: Team 2  
- **Team Members**: Anila Roy, Ravisankar S, Saahil Manoj M P  
- **Company**: [Zelbytes Pvt. Ltd.](https://zelbytes.com) — A product-based startup working on Robotics, IoT, Embedded Systems, and E-waste management through renovation.

---

## 🎯 Project Objective
This project aims to develop a deep learning model that classifies strawberry images into three ripeness categories:
1. **Ripe**  
2. **Turning**  
3. **Unripe**  

We leveraged the **MobileNetV2** architecture using **TensorFlow** to create a lightweight yet powerful classifier optimized for performance.

---

## 🧠 Model Details
- **Model File**: `mobilenetv2_strawberry_ripeness_final.h5`  
- **Base Model**: MobileNetV2 (pretrained on ImageNet)  
- **Framework**: TensorFlow (with Keras)  

```text
| Metric               | Value   |
|----------------------|--------:|
| **Accuracy**         | 0.9934  |
| **Loss**             | 0.2628  |
| **Val. Accuracy**    | 0.9867  |
| **Val. Loss**        | 0.2702  |
```
> ✅ The model demonstrated excellent training and evaluation performance with strong generalization.

---

## 📂 Dataset Description
- **Dataset File**: `dataset.zip`  
- **Total Images**: 1,509  

```text
| Class   | Image Count |
|:--------|------------:|
| **Ripe**    | 722         |
| **Turning** | 290         |
| **Unripe**  | 497         |
```
### 📊 Data Split
```text
| Split       | # Images | Percentage |
|:------------|---------:|-----------:|
| Training    | 1,208    | ~80%       |
| Validation  | 301      | ~20%       |
```
---

## ✅ Test Results
The model was evaluated on **10 unseen test images**.

### Confusion Matrix
```text
             Predicted →
           Ripe  Turning  Unripe
Actual ↓
Ripe        3       0        0
Turning     0       3        0
Unripe      0       0        4


              precision    recall  f1-score   support

        ripe     1.0000    1.0000    1.0000         3
     turning     1.0000    1.0000    1.0000         3
      unripe     1.0000    1.0000    1.0000         4

    accuracy                         1.0000        10
   macro avg     1.0000    1.0000    1.0000        10
weighted avg     1.0000    1.0000    1.0000        10
```
🏆 100% accuracy on the test set with perfect precision, recall, and F1-score for all classes.

### Colab Notebook 

Notebook: day13_evaluation_Team2.ipynb
Contains model loading, evaluation, test predictions, and visualizations.

### GitHub Repository
🔗 https://github.com/Ravisankar-S/Team2_Zelbytes/


!!! -- Contact / Acknowledgement -- !!!

This work was completed under the AI & Data Science internship program at Zelbytes Pvt. Ltd.
