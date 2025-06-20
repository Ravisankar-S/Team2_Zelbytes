# Team2_Zelbytes

Strawberry Ripeness Classification using MobileNetV2
##------------------------------------------------------------##

Team Name: Team 2
Team Members - Anila Roy, Ravisankar S, Saahil Manoj M P
Internship: AI & Data Science Internship @ Zelbytes Pvt. Ltd.
Company: Zelbytes Pvt. Ltd. — A product-based startup working on Robotics, IoT, Embedded Systems, and E-waste management through renovation.
##------------------------------------------------------------##

-- Project Objective --

This project aims to develop a deep learning model that classifies strawberries based on their ripeness level into three categories:

1.Ripe
2.Turning
3.Unripe

We leveraged the MobileNetV2 architecture using TensorFlow to create a lightweight yet powerful classifier optimized for performance.
##------------------------------------------------------------##


-- Model Details -- 

Model File: mobilenetv2_strawberry_ripeness_final.h5

Base Model Used: MobileNetV2 (pretrained on ImageNet)

Framework: TensorFlow (with Keras)


| Metric              | Value  |
| ------------------- | ------ |
| Accuracy            | 0.9934 |
| Loss                | 0.2628 |
| Validation Accuracy | 0.9867 |
| Validation Loss     | 0.2702 |


The model demonstrated good performance both during training and evaluation, with satisfactory generalization.
##------------------------------------------------------------##


-- Dataset Description -- 

Dataset File: dataset.zip

Total Images: 1,509 images

Classes:
1.Ripe → 722 images
2.Turning → 290 images
3.Unripe → 497 images

Data Split:
1.Training Set: 1,208 images (~80%)
2.Validation Set: 301 images (~20%)

Test Set: 10 images (test.zip) – used for final evaluation
##------------------------------------------------------------##


-- Test Results --

The model was evaluated on a set of 10 unseen images. Below are the results:

Confusion Matrix:

             Predicted →
            Ripe  Turning  Unripe
Actual ↓
Ripe        3       0        0
Turning     0       3        0
Unripe      0       0        4


Classification Report: 

              precision    recall  f1-score   support

        ripe     1.0000    1.0000    1.0000         3
     turning     1.0000    1.0000    1.0000         3
      unripe     1.0000    1.0000    1.0000         4

    accuracy                         1.0000        10
   macro avg     1.0000    1.0000    1.0000        10
weighted avg     1.0000    1.0000    1.0000        10

The model achieved 100% accuracy on the test set with perfect precision, recall, and F1-scores for each class.
##------------------------------------------------------------##


-- Colab Notebook --

File Name: day13_evaluation_Team2.ipynb

This notebook contains the code for loading the model, testing it on new images, and visualizing the results.
##------------------------------------------------------------##


-- GitHub Repository --

All project files are hosted in the following repository:
🔗 https://github.com/Ravisankar-S/Team2_Zelbytes/

##------------------------------------------------------------##


!!! -- Contact / Acknowledgement -- !!!

This work was completed under the AI & Data Science internship program at Zelbytes Pvt. Ltd.
