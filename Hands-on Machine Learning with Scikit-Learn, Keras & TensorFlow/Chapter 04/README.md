# 📘 Bab 4: Melatih Model Linear  
📁 File: `04_training_linear_models.ipynb`

---

## 🧭 Tujuan Bab

Bab ini memperkenalkan **model linear**, yang merupakan dasar fundamental dalam Machine Learning. Fokus utamanya adalah bagaimana melatih model ini secara efisien, mengatasi tantangan overfitting/underfitting, serta memperkenalkan **teknik regularisasi** dan **klasifikasi linear**.

> 💡 Pemahaman kuat terhadap regresi linear & optimisasi menjadi fondasi penting untuk model kompleks seperti neural networks.

---

## 📐 Regresi Linear

### 📊 Persamaan Normal (Normal Equation)
- Solusi analitis langsung untuk meminimalkan fungsi biaya
- Cepat dan akurat untuk dataset kecil
- ⚠️ Kurang efisien untuk dataset besar (kompleksitas komputasi tinggi)

### 📉 Gradient Descent (GD)
- Pendekatan iteratif yang lebih scalable
- 3 varian utama:
  - 🟠 **Batch GD**: Semua data → stabil tapi lambat
  - 🔵 **Stochastic GD (SGD)**: Satu instans acak → cepat, cocok untuk online learning
  - 🟢 **Mini-Batch GD**: Subset data kecil → kombinasi efisiensi & kestabilan

---

## 📈 Regresi Polinomial

- Menambahkan **fitur berpangkat (polinomial)** dari fitur asli
- Memungkinkan model mempelajari hubungan **non-linear**
- ⚠️ Risiko overfitting jika derajat terlalu tinggi

### 📊 Kurva Pembelajaran (Learning Curves)
- Visualisasi kesalahan pelatihan & validasi
- Digunakan untuk mendeteksi:
  - **Underfitting**: Model terlalu sederhana
  - **Overfitting**: Model terlalu kompleks

---

## 🔒 Regularisasi Model Linear

### 🔵 Ridge Regression (L2 Regularization)
- Penalti terhadap **jumlah kuadrat bobot**
- Menghindari bobot besar → mendorong generalisasi

### 🟠 Lasso Regression (L1 Regularization)
- Penalti terhadap **jumlah absolut bobot**
- Mendorong **sparsity** → beberapa bobot menjadi nol

### 🟢 Elastic Net Regression
- Gabungan Ridge dan Lasso
- ⚖️ Seimbang antara regularisasi L1 dan L2

### ⏹️ Early Stopping
- Menghentikan pelatihan saat kinerja validasi memburuk
- Teknik regularisasi sederhana namun **sangat efektif**

---

## 🧮 Regresi Logistik

- Model klasifikasi linear → memetakan input ke **probabilitas kelas**
- Menggunakan fungsi **sigmoid**
- Cocok untuk **binary classification**
- Dilengkapi dengan:
  - **Fungsi Biaya Logistik**
  - **Batas Keputusan (Decision Boundaries)**

---

## 🌐 Softmax Regression

- Generalisasi dari regresi logistik untuk **klasifikasi multikelas**
- Menggunakan fungsi **Softmax** untuk menghitung probabilitas setiap kelas
- Model memilih kelas dengan probabilitas tertinggi sebagai prediksi

---

## 🧠 Insight Utama

> 🧱 Konsep dalam bab ini (optimisasi, regularisasi, kurva pembelajaran)  
> akan menjadi **pondasi penting** saat memasuki pembelajaran mendalam di bagian selanjutnya.

---
