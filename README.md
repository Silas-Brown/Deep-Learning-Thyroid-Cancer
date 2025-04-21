# Deep Learning Thyroid Cancer 

## (1) Overview  

This project builds off of the thyroid cancer classification project, and replaces the SVM with a deep neural network. The preprocessing and feature selection is maintained from the previous project. The core focus of this project is to create a reasonable hyperparameter search space to optimize the deep neural network based on theoretical considerations, then compare the performance of the DNN to the SVM.

✅ **Dataset:** 383 patients, 16 features originally, but only 7 features considered.   
✅ **Goal:** Predict recurrence of thyroid cancer  
✅ **Result:** PR-AUC of final model is 98.94% on a holdout set. Mean of 5-fold PR-AUC is 93% with standard deviation of 3.90%
---

## (2) Methodology  
### 🔹 (2.1) Defining the hyperparameter space
  - **Using theory to infer a reasonable, efficient search space that respects computational costs**
  - **Hyperparameter defined as epochs, batch size, number of hidden layers, and a vector of layer widths**
  - **Epoch, batch size, layers, and vector of layer width search spaces restricted to**
      - Epochs in {50,75,100}
      - Batch sizes in {16,32,64}
      - Layers in {2,3,4}
      - Vector represented pyramidally as (2^(L), 2^(L-1), ... 2) 

## (3) Implementation  

### **🔗 Full Implementation in Colab:**  
https://colab.research.google.com/drive/1mx5QjBCkz7qxdkZtcvqhe4Dy3Cc61Z-R?usp=sharing

## (5) Contact  
📧 Email: **silasaverybrown@gmail.com**  
💡 LinkedIn: [Silas Brown](https://www.linkedin.com/in/silas-brown/) 



