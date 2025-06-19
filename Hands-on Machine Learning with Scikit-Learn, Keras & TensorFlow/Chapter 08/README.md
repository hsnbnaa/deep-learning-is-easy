# 📘 Bab 8: Reduksi Dimensi (Dimensionality Reduction)  
📁 File: `08_dimensionality_reduction.ipynb`

---

## 🎯 Tujuan Bab

Bab ini membahas salah satu tantangan utama dalam Machine Learning modern:  
**🔺 Curse of Dimensionality** — ketika data memiliki terlalu banyak fitur, menyebabkan pelatihan lambat, performa buruk, dan sulitnya menemukan solusi yang baik.

🔧 Solusi yang ditawarkan adalah **Reduksi Dimensi**:  
→ Teknik untuk menyederhanakan representasi data dengan mengurangi jumlah fitur tanpa kehilangan terlalu banyak informasi penting.

---

## ⚖️ Trade-off Praktis

> 🎭 Reduksi dimensi = seperti kompresi JPEG → Lebih ringan, tapi bisa mengorbankan sedikit kualitas.

- ✅ Keuntungan:
  - Mempercepat pelatihan
  - Mengurangi overfitting
  - Memudahkan visualisasi data
- ❌ Kekurangan:
  - Kehilangan sebagian informasi
  - Menambah kompleksitas pipeline
  - Bisa sedikit menurunkan performa model

📌 Saran: Coba latih model dengan data asli dulu. Gunakan reduksi dimensi **jika** pelatihan terlalu lambat atau data terlalu besar.

---

## 🧭 Dua Pendekatan Utama

### 🪞 1. Proyeksi
- Memproyeksikan data dari dimensi tinggi → dimensi lebih rendah
- Teknik klasik dan cepat

### 🧩 2. Manifold Learning
- Asumsi: data sebenarnya hidup di "permukaan" (manifold) berdimensi rendah dalam ruang berdimensi tinggi
- Tujuan: temukan manifold tersebut

---

## 📌 Algoritma Utama: PCA (Principal Component Analysis)

### 🔎 Konsep:
- Menemukan **sumbu-sumbu baru (komponen utama)** yang menangkap varian terbesar
- Memungkinkan kita menyimpan **informasi terpenting dengan fitur lebih sedikit**

### ⚙️ Fitur PCA:
- 🔢 **Proyeksi ke d dimensi** → kurangi dimensi asli
- 📊 **Rasio Varians yang Dijelaskan** → bantu memilih berapa banyak dimensi yang dipertahankan
- 💾 **PCA untuk Kompresi** → simpan data dengan ukuran lebih kecil

### 🛠️ Implementasi:
- Gunakan `Scikit-Learn` untuk:
  - PCA biasa
  - Randomized PCA (untuk dataset besar)
  - Incremental PCA (untuk data streaming)

---

## 🔍 Algoritma Tambahan

### 📌 Random Projection
- Teknik proyeksi acak yang sangat cepat dan efisien

### 📌 LLE (Locally Linear Embedding)
- Metode manifold learning untuk menemukan struktur non-linear lokal

---

## 💡 Insight Utama

> 📉 **Reduksi Dimensi bukan hanya tentang efisiensi, tapi juga pemahaman struktur data.**  
> 🔀 Pilih teknik berdasarkan tujuan: kecepatan, interpretabilitas, atau akurasi.

> 🔧 Efisiensi model sering kali datang dengan harga: kehilangan presisi.  
> ⚖️ Penting untuk memahami trade-off dan menyesuaikan dengan kebutuhan proyek ML.

---
