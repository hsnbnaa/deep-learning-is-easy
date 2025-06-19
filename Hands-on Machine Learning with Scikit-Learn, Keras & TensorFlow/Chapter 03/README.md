# 📘 Bab 3: Klasifikasi  
📁 File: `03_classification.ipynb`

---

## 🧭 Tujuan Bab

Bab ini membahas secara mendalam **tugas klasifikasi**, yaitu mengklasifikasikan instans data ke dalam kategori atau kelas tertentu. Contoh utama yang digunakan adalah dataset **MNIST**, berisi gambar digit tulisan tangan (0–9).

> 🎯 Fokus utama: Membangun pemahaman yang kuat tentang **evaluasi model klasifikasi** dan pemilihan metrik yang sesuai dengan tujuan bisnis.

---

## 📦 Topik Utama

### 1️⃣ Klasifikasi Biner
- Model diajarkan membedakan antara **dua kelas** (misal: angka 5 vs bukan 5)
- Digunakan sebagai pengantar konsep evaluasi kinerja

---

## 📊 Evaluasi Model Klasifikasi

### 🔢 Akurasi
- Mudah dipahami, tetapi **menyesatkan pada dataset tidak seimbang**
- ⚠️ Contoh: Model memprediksi semua negatif → akurasi tinggi tapi tidak berguna

### 🔁 Validasi Silang (Cross-Validation)
- Estimasi kinerja yang lebih **stabil dan andal**
- Menghindari bias evaluasi dari satu *split* data

### 📉 Matriks Kebingungan (Confusion Matrix)
- Menampilkan:
  - ✅ True Positives (TP)
  - ✅ True Negatives (TN)
  - ❌ False Positives (FP)
  - ❌ False Negatives (FN)
- Alat dasar untuk mengevaluasi dan memahami kesalahan model

---

### 🎯 Precision & Recall

| Metrik     | Rumus                          | Arti                                                                 |
|------------|--------------------------------|----------------------------------------------------------------------|
| Presisi    | `TP / (TP + FP)`              | Seberapa akurat prediksi positif                                    |
| Recall     | `TP / (TP + FN)`              | Seberapa baik model mendeteksi semua kasus positif                   |

- ⚖️ **Trade-off** antara Precision dan Recall sangat penting → tergantung konteks (misalnya: deteksi kanker vs spam)

### ⚖️ F1-Score
- Rata-rata harmonik dari precision dan recall
- Ideal saat perlu **keseimbangan** antara keduanya

---

### 📈 Kurva ROC dan AUC
- ROC: Plot **True Positive Rate (Recall)** vs **False Positive Rate**
- AUC: Luas di bawah kurva, semakin tinggi → semakin baik model membedakan kelas

---

## 🌈 Klasifikasi Lanjutan

### 🔢 Klasifikasi Multikelas
- Model memprediksi satu label dari banyak kelas (contoh: 0–9 di MNIST)

### 🔁 Klasifikasi Multioutput
- Model menghasilkan **beberapa label** untuk satu input
- Contoh: Multi-label tagging (film: aksi, komedi, sci-fi)

---

## 🔍 Analisis Kesalahan

> 🧠 Langkah penting: *"Di mana model sering salah?"*

Analisis kesalahan membantu:
- Menemukan kelemahan fitur atau arsitektur
- Mengidentifikasi pola kesalahan yang bisa dioptimasi

---

## 🧠 Insight Utama

> ✅ Evaluasi model bukan hanya soal akurasi  
> 🎯 Pilih metrik yang sesuai konteks: biaya kesalahan ≠ sama di semua kasus  
> 🛠️ Gunakan **visualisasi & analisis kesalahan** untuk meningkatkan model

---
