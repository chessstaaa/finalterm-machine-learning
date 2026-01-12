# Final Term CNN Fish Classification Project

## 📊 Project Overview
Proyek ini merupakan **image classification pipeline berbasis Convolutional Neural Network (CNN)** untuk mengklasifikasikan **31 spesies ikan** menggunakan dataset citra ikan.  
Model yang dibandingkan:

- CNN From Scratch  
- MobileNetV2 (Frozen Feature Extractor)  
- MobileNetV2 Fine-Tuned  

Tujuan utama proyek ini adalah **mencari model dengan akurasi tertinggi dan F1-Score terbaik**.

---

## 📈 Dataset Information

- Dataset berupa citra ikan multi-kelas (31 kelas)  
- Data dibagi menjadi:
  - Train  
  - Validation  
  - Test  
- Semua citra di-resize menjadi **224 × 224 pixel**

---

## 🛠️ Data Preprocessing

- Dataset dimuat menggunakan TensorFlow Dataset API  
- Preprocessing yang digunakan:
  - Resize citra ke 224 × 224
  - Normalisasi pixel (0–1)
  - Data Augmentation (flip, rotation, zoom)
  - Cache & Prefetch untuk akselerasi training GPU  
- **Class weighting** digunakan untuk mengatasi class imbalance

---

## 🤖 Models Implemented

### 1. CNN From Scratch
Digunakan sebagai baseline model.

### 2. MobileNetV2 (Frozen)
Model transfer learning menggunakan backbone MobileNetV2 dengan weight ImageNet (frozen).

### 3. MobileNetV2 Fine-Tuned
Model MobileNetV2 dengan sebagian layer dibuka (unfrozen) untuk fine-tuning agar meningkatkan performa.

---

## 📊 Model Evaluation Metrics

| Metric | Description |
|------|-------------|
| Accuracy | Overall classification accuracy |
| Macro F1 | Balanced class performance |
| Weighted F1 | Frequency-weighted performance |

---

## 🏆 Final Model Comparison

| Model | Validation Accuracy | Macro F1 | Weighted F1 |
|------|---------------------|----------|-------------|
| **MobileNetV2 Fine-Tuned** | **91.28%** | **0.9157** | **0.9151** |
| MobileNetV2 Frozen | 90.08% | – | – |
| CNN Scratch | 71.18% | 0.7035 | 0.7159 |

---

## 📁 Outputs

| Output | Description |
|------|------------|
| cnn_scratch_best.keras | Best baseline CNN |
| mobilenetv2_frozen_best.keras | Best frozen MobileNetV2 |
| mobilenetv2_finetuned_best.keras | **Final production model** |
| cnn_model_comparison.csv | Final model comparison |

---

## ✅ Project Status

- Multi-model CNN implemented  
- Transfer learning & fine-tuning applied  
- Automatic model comparison  
- Final model selected  
- Ready for academic submission & report  

---

## 🔧 Tech Stack

- Python 3.x  
- TensorFlow / Keras  
- NumPy, Pandas  
- Scikit-learn  
- Matplotlib  

---

## 🚀 Summary

- Proyek ini mengimplementasikan pipeline CNN lengkap  
- Menggunakan transfer learning untuk meningkatkan akurasi  
- MobileNetV2 Fine-Tuned dipilih sebagai **model final produksi**  
- Sistem siap digunakan untuk keperluan akademik dan penelitian  

---

**Final Term CNN Classification Model – Ready to Submit 🚀**
