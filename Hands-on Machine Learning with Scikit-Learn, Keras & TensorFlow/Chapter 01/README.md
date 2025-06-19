# 📘 Bab 1: Machine Learning Landscape 
📁 File: `01_the_machine_learning_landscape.ipynb`

---

## 📌 Ikhtisar

Bab pertama ini membahas **dasar-dasar dan lanskap umum pembelajaran mesin (Machine Learning/ML)**, dengan menjawab pertanyaan penting:  
> 🔍 *Apa itu Machine Learning dan bagaimana ia berbeda dari pemrograman tradisional?*

ML didefinisikan sebagai proses memprogram komputer untuk mengoptimalkan kinerja berdasarkan **pengalaman sebelumnya (data)**. Konsep kunci dalam ML dijelaskan melalui tiga elemen:
- **Tugas (T)**: Misalnya, mengenali tulisan tangan
- **Pengalaman (E)**: Dataset dengan label
- **Ukuran Kinerja (P)**: Persentase klasifikasi benar

---

## 🧠 Jenis-Jenis Sistem Pembelajaran Mesin

### 1️⃣ Supervised Learning (*Pembelajaran Terawasi*)
- Menggunakan **data berlabel**
- Contoh:
  - 📬 Klasifikasi: Deteksi spam, pengenalan digit (MNIST)
  - 📈 Regresi: Prediksi harga rumah
- Sub-kategori:
  - 🔀 Semi-Supervised Learning
  - 🧩 Self-Supervised Learning

### 2️⃣ Unsupervised Learning (*Pembelajaran Tanpa Pengawasan*)
- **Tidak menggunakan label**
- Tujuan: Menemukan pola tersembunyi
- Teknik:
  - 🔗 Clustering: `k-Means`, `HCA`, `EM`
  - 🔍 Dimensi Reduksi & Visualisasi: `PCA`, `t-SNE`, `LLE`
  - 🔄 Asosiasi: `Apriori`, `Eclat`

### 3️⃣ Reinforcement Learning (*Pembelajaran Penguatan*)
- **Agen** belajar dari **lingkungan**
- Bertindak → Mendapat imbalan → Belajar kebijakan optimal

---

## 🔄 Cara Belajar Mesin

| Tipe Pembelajaran | Penjelasan |
|-------------------|------------|
| 🗃️ Batch Learning | Belajar dari seluruh data secara offline |
| 🔄 Online Learning | Belajar dari data secara bertahap (streaming / mini-batch) |
| 🧠 Instance-Based | Mengingat contoh & menggeneralisasi menggunakan kemiripan |
| 🧪 Model-Based     | Membangun model dari data pelatihan |

---

## ⚠️ Tantangan Umum dalam ML

- 📉 Data tidak cukup
- 🎯 Data tidak representatif
- 🧪 Kualitas data buruk
- ❌ Fitur tidak relevan
- 🔂 **Overfitting**: Terlalu cocok dengan data pelatihan
- 🔄 **Underfitting**: Terlalu sederhana, gagal menangkap pola

---

## 🧪 Evaluasi & Validasi Model

### Kenapa penting?
> Model yang tampak bagus di data pelatihan belum tentu bekerja baik di dunia nyata!

### Strategi:
- 🔀 Split: Data dilatih di *training set*, diuji di *test set*
- 🔧 Validasi & Tuning:
  - Gunakan *validation set* untuk menyetel **hyperparameter**
  - Gunakan teknik **cross-validation** untuk hasil yang lebih andal
  - Hindari **data leakage** (mengintip data uji!)

---

## 🧬 Fondasi Praktik ML

Bab ini membangun fondasi penting dengan:
- Memperkenalkan **terminologi dan paradigma utama**
- Menunjukkan pentingnya **generalization**
- Memperkuat praktik *robust ML engineering*

---
