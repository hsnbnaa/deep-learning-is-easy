# 📘 Bab 9: Pembelajaran Tanpa Pengawasan (Unsupervised Learning)  
📁 File: `09_unsupervised_learning.ipynb`

---

## 🎯 Tujuan Bab

Bab ini memperkenalkan **Unsupervised Learning**, pendekatan pembelajaran mesin yang digunakan untuk mengekstrak pola, struktur tersembunyi, atau hubungan dari **data tanpa label**.

> 🧠 Cocok untuk eksplorasi data, data mining, segmentasi, dan generasi data  
> 📊 Sangat berguna dalam dunia nyata di mana label sering kali tidak tersedia

---

## 🧩 Fokus Utama: Klastering

### 🔹 k-Means Clustering
- Salah satu algoritma paling populer
- Membagi data menjadi `k` klaster berdasarkan jarak
- ⚠️ Keterbatasan:
  - Sensitif terhadap inisialisasi centroid
  - Tidak cocok untuk bentuk klaster non-konveks
- 📸 Aplikasi:
  - Segmentasi gambar
  - Pseudo-labeling dalam **semi-supervised learning**

### 🔹 DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
- Mendeteksi klaster berdasarkan kepadatan titik
- ✔️ Dapat menemukan klaster berbentuk arbitrer
- ✔️ Dapat mengidentifikasi outlier/noise
- ❌ Tidak cocok untuk data berdimensi tinggi

### 🔹 Hierarchical Clustering (HCA)
- Membentuk hierarki klaster (dendrogram)
- Cocok untuk visualisasi relasi antar kelompok data

### 🔹 Expectation Maximization (EM)
- Berdasarkan model probabilistik (iteratif)
- Sering digunakan dalam model campuran Gaussian

---

## 📈 Gaussian Mixture Models (GMM)

### 🔬 Konsep:
- Data diasumsikan berasal dari **gabungan distribusi Gaussian**
- Memberikan pendekatan **probabilistik** untuk klastering

### 📌 Aplikasi:
- 🔍 **Anomaly Detection**: Titik data dengan probabilitas rendah dianggap sebagai anomali
- 🔢 **Model Selection**: Memilih jumlah klaster optimal adalah tantangan utama

### 🧪 Variasi: Bayesian Gaussian Mixture
- Dapat menentukan jumlah klaster secara otomatis menggunakan prior

---

## 🚨 Deteksi Anomali & Novelty Detection

Selain GMM, bab ini juga menyebutkan berbagai algoritma untuk:
- Mengenali **data tidak biasa** (anomali)
- Mengenali **kasus baru** (novelty) yang belum pernah dilihat model

---

## 💡 Insight Utama

> 🔁 Unsupervised learning bukan hanya pelengkap supervised learning,  
> tetapi **pilar penting** dalam memahami struktur alami data.

📍 Teknik seperti klastering dan model probabilistik membantu:
- Menjelajahi data tanpa label
- Mengurangi kebutuhan akan anotasi manual
- Menghasilkan **label pseudo** untuk memperluas dataset

---
