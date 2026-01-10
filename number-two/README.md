# Final Term Regression Project

## 📊 Project Overview
Proyek ini merupakan **regression modeling pipeline** untuk memprediksi nilai target numerik (tahun) menggunakan beberapa pendekatan machine learning dan deep learning.  
Model yang dibandingkan:

- Linear Regression  
- Random Forest Regressor  
- LightGBM Regressor  
- Neural Network (Keras / TensorFlow)

Tujuan utama proyek ini adalah **mencari model dengan error terkecil (MSE & MAE) dan R² terbaik**.

---

## 📈 Dataset Information

- Dataset tidak memiliki header
- Kolom pertama adalah **target variable (y)**  
- Kolom lainnya merupakan fitur numerik  
- Data dibagi menggunakan train-test split (80/20)

---

## 🛠️ Data Preprocessing

- Data dibaca menggunakan Pandas
- Fitur numerik di-handle menggunakan:
  - `SimpleImputer(strategy="median")`
  - `StandardScaler()` untuk model neural network
- Split data menggunakan `train_test_split`

---

## 🤖 Models Implemented

### 1. Linear Regression
Digunakan sebagai baseline model.

### 2. Random Forest Regressor
Model tree-based ensemble untuk menangkap hubungan non-linear.

### 3. LightGBM Regressor
Gradient boosting model yang efisien dan powerful.

### 4. Neural Network (Keras)
Feed-forward neural network dengan:
- Dense layers
- ReLU activation
- Adam optimizer
- Mean Squared Error loss

---

## 📊 Model Evaluation Metrics

Semua model dievaluasi menggunakan:

| Metric | Description |
|------|-------------|
| MSE | Mean Squared Error |
| MAE | Mean Absolute Error |
| R² Score | Coefficient of Determination |

Model terbaik dipilih berdasarkan **nilai MSE terendah & R² tertinggi**.

---

## 🏆 Model Selection Logic

Notebook secara otomatis:
1. Menghitung metrik untuk setiap model  
2. Membandingkan hasil performa  
3. Memilih model terbaik secara otomatis  
4. Menyimpan hasil prediksi dari model terbaik  

---

## 📈 Feature Importance

Untuk model **LightGBM**, dilakukan analisis:
- Visualisasi **Top 20 feature importance**
- Memberikan interpretabilitas terhadap model

---

## 📁 Outputs

| Output | Description |
|------|------------|
| Visualisasi Feature Importance | Plot LightGBM |
| Prediksi Model Terbaik | Array hasil prediksi |
| Evaluation Metrics | Printed evaluation summary |

---

## ✅ Project Status

- Multiple regression models implemented  
- Automatic model comparison  
- Feature importance visualization  
- Ready for academic submission & report  

---

## 🔧 Tech Stack

- Python 3.x  
- Pandas, NumPy  
- Scikit-learn  
- LightGBM  
- TensorFlow / Keras  
- Matplotlib  

---

## 🚀 Summary

- Proyek ini mengimplementasikan pipeline regression lengkap
- Melakukan perbandingan berbagai model ML & DL
- Model terbaik dipilih otomatis berdasarkan performa
- Menyediakan interpretasi melalui feature importance (LightGBM)

---

**Final Term Regression Model – Ready to Submit 🚀**