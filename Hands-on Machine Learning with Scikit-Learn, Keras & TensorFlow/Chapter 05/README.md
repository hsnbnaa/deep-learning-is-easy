# 📘 Bab 5: Mesin Vektor Dukungan (Support Vector Machines)  
📁 File: `05_support_vector_machines.ipynb`

---

## 🧭 Tujuan Bab

Bab ini memperkenalkan **Support Vector Machines (SVM)** — salah satu algoritma pembelajaran mesin yang paling kuat dan serbaguna.  
SVM digunakan untuk:
- 📊 Klasifikasi Linear & Non-Linear
- 📈 Regresi (SVR)
- 🛡️ Deteksi Keanehan (Novelty Detection)

> 💡 SVM sangat efektif untuk **dataset kecil hingga menengah** yang tidak terlalu besar (ratusan hingga ribuan instans).

---

## ✳️ Konsep Inti: Margin Maksimum

- Tujuan SVM adalah menemukan **hyperplane optimal** yang **memisahkan kelas** sejauh mungkin.
- **Support Vectors**: Titik data di tepi margin yang **menentukan posisi hyperplane**.

---

## ⚖️ Klasifikasi Margin

### 🟥 Hard Margin Classification
- Hanya berfungsi jika data **dapat dipisahkan secara sempurna**
- ❌ Sangat sensitif terhadap **outlier**
- ⚠️ Tidak cocok untuk data yang tidak sepenuhnya linear

### 🟧 Soft Margin Classification
- Memungkinkan **beberapa pelanggaran margin**
- Gunakan **hyperparameter C** untuk mengontrol:
  - **C kecil** → margin lebar, lebih toleran terhadap pelanggaran (⬇ overfitting)
  - **C besar** → margin sempit, toleransi rendah terhadap pelanggaran (⬆ risiko overfitting)
- ⚖️ Trade-off antara **kompleksitas model vs generalisasi**

---

## 🔮 Klasifikasi SVM Non-Linear

### 🧠 Kernel Trick
- Alih-alih mentransformasi data secara eksplisit → **gunakan fungsi kernel** untuk menghitung jarak dalam ruang berdimensi tinggi
- Contoh kernel:
  - 🧮 Polynomial Kernel
  - 🔗 Similarity Features (misalnya Gaussian RBF)

> ✨ Trik kernel memungkinkan SVM mempelajari batas non-linear **tanpa** biaya komputasi tinggi dari transformasi nyata.

---

## 📉 Regresi SVM (Support Vector Regression - SVR)

- Ekstensi dari SVM untuk memprediksi **nilai kontinu**
- Tujuan: Menemukan **margin optimal** di mana kesalahan masih dapat diterima
- Mirip klasifikasi, tapi untuk output numerik

---

## ✅ Kelebihan SVM

- ⚙️ **Fungsi Kernel yang fleksibel** → cocok untuk berbagai jenis data
- 📐 Bekerja sangat baik di **ruang berdimensi tinggi**
- 🧪 Efektif ketika jumlah fitur >> jumlah instans

---

## ❌ Kelemahan SVM

- 🔊 **Sensitif terhadap outlier**
- 🐌 Skalabilitas buruk untuk dataset besar (butuh banyak RAM dan komputasi)
- Tidak sefleksibel neural networks dalam **representasi non-linear kompleks**

---

## 🧠 Insight Utama

> 📌 SVM sangat kuat dalam kondisi yang tepat, tetapi bukan solusi universal.  
> Pemilihan model harus mempertimbangkan **ukuran data, dimensi fitur, dan kompleksitas pola**.

---

