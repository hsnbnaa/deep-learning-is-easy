# 📘 Bab 6: Pohon Keputusan (Decision Trees)  
📁 File: `06_decision_trees.ipynb`

---

## 🧭 Tujuan Bab

Bab ini membahas **Decision Trees**, salah satu algoritma ML paling intuitif dan serbaguna, yang dapat digunakan untuk:
- 🏷️ Klasifikasi
- 📈 Regresi
- 🔀 Multi-output prediction

> 🌲 Decision Trees sangat powerful namun berisiko **overfitting**, terutama pada dataset kompleks seperti dataset perumahan California (Bab 2).

---

## 🧠 Konsep Dasar

- Decision Tree membagi data secara rekursif ke dalam subset berdasarkan **fitur paling informatif**
- Hasil pembelajaran adalah struktur pohon yang **mudah divisualisasikan dan diinterpretasikan**
- 📍 Implementasi di Scikit-Learn menggunakan algoritma:
  ### 🔍 **CART (Classification And Regression Tree)**

---

## 📏 Regularisasi: Mencegah Overfitting

Untuk menghindari pohon tumbuh terlalu kompleks dan overfit:

### ✂️ Pruning (Pemangkasan Pohon)
- 🔧 Gunakan hyperparameter seperti:
  - `max_depth` → membatasi kedalaman pohon
  - `min_samples_split` / `min_samples_leaf`
- 🌿 Dapat dilakukan:
  - **Selama pelatihan (pre-pruning)**
  - **Setelah pelatihan (post-pruning)**

---

## 📊 Pohon untuk Regresi

- Tidak hanya klasifikasi! Pohon juga dapat digunakan untuk **prediksi nilai kontinu**
- Pohon regresi membagi ruang fitur menjadi region dan **mengeluarkan nilai rata-rata target** di setiap region sebagai prediksi

---

## ⚠️ Kelebihan dan Keterbatasan

### ✅ Kelebihan:
- 🔎 Transparan dan mudah dipahami
- ❌ Tidak membutuhkan banyak pra-pemrosesan
- 🌐 Dapat menangani fitur kategorikal dan numerik

### ❌ Keterbatasan:
- 💥 Rentan terhadap overfitting
- 📉 Performa kurang stabil terhadap fluktuasi data (sedikit perubahan → struktur pohon berubah total)

---

## 🔗 Menuju Model Lebih Kuat: Ensemble Learning

> 📌 Decision Trees adalah fondasi penting untuk algoritma **Ensemble** seperti:
- 🌲 **Random Forest**
- 🎯 **Gradient Boosted Trees**

Bab ini menjadi transisi strategis menuju **model yang lebih tangguh** dengan menggabungkan banyak pohon → dibahas di bab selanjutnya.

---

## 🧠 Insight Utama

> ✅ Memahami Decision Trees = memahami dasar dari banyak algoritma ensemble yang powerful  
> 🎯 Regularisasi sangat penting untuk menjaga model tetap generalisatif dan tidak overfit

---
