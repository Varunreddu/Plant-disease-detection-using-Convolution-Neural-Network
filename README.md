# 🌿 Plant Disease Detection Using CNN

This project aims to develop an automated system for detecting and classifying diseases in apple plant leaves using Convolutional Neural Networks (CNNs). The goal is to reduce manual effort, provide faster diagnosis, and enhance productivity for farmers and researchers.

## 👥 Team Members

  **Anish Arun Sandaye** – CB.EN.P2EBS24003
  **Cheppalli Naga Sai Varun Reddy** – CB.EN.P2EBS24006
  **Course**: 21ES613 – Machine Learning for Embedded Applications
  **Institution**: Amrita Vishwa Vidyapeetham, Coimbatore

## 🎯 Objectives

* Detect and classify plant leaf diseases accurately.
* Automate disease diagnosis using a deep learning model.
* Deploy an efficient and lightweight CNN model suitable for real-time and embedded applications.

---

## 📊 Dataset

* **Source**: [Kaggle – Plant Pathology 2020 FGVC7](https://www.kaggle.com/competitions/plant-pathology-2020-fgvc7/data)
* **Total Images**: 3,651 JPEGs
* **Classes**:

  * Healthy
  * Multiple Diseases
  * Rust
  * Scab

## ⚙️ Methodology

### Step 1: Import Libraries

Used libraries include:

```python
os, pandas, numpy, matplotlib, tensorflow
```

### Step 2: Data Preprocessing

* Loaded 1821 labeled images (Train: 1456, Validation: 365)
* Performed:

  * Data augmentation
  * Resizing
  * Normalization

### Step 3: Exploratory Data Analysis (EDA)

* Analyzed label distribution
* Examined image size and color intensity patterns

### Step 4: CNN Architecture

* Input size: 128x128x3
* Convolution + ReLU + MaxPooling layers
* Flatten + Dense layers with Dropout
* Final output via Softmax layer

### Step 5: Model Training

* Optimizer: Adam (learning rate = 0.001)
* Loss Function: Categorical Crossentropy
* Several epochs with data augmentation

### Step 6: Model Evaluation

* Evaluated on validation set of 365 images
* Metrics: Accuracy and classification performance

## ✅ Results & Conclusion

* The custom CNN achieved competitive results, particularly in classifying **Rust** and **Scab**.
* Underperformed in "Multiple Diseases" due to class imbalance.
* Demonstrated potential for on-device real-time disease detection.

## 📚 References

1. Singh & Jain, ICRITO 2024 – DOI: 10.1109/ICRITO61523.2024.10522449
2. Li et al., IEEE Access 2021 – DOI: 10.1109/ACCESS.2021.3069646
3. Shrestha et al., ASPCON 2020 – DOI: 10.1109/ASPCON49795.2020.9276493
4. Ramesh et al., ICDI3C 2018 – DOI: 10.1109/ICDI3C.2018.00017
5. [NCBI Figure 18](https://www.ncbi.nlm.nih.gov/books/NBK597497/figure/ch3.Fig18/)
6. Siddhardhan – [GitHub CNN Leaf Classifier](https://github.com/siddhardhan23/plant-disease-prediction-cnn-deep-leanring-project)
7. Karol et al., IJAREEIE 2019 – DOI: 10.15662/IJAREEIE.2019.0803014





