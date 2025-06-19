# 📘 Bab 2: Proyek Pembelajaran Mesin End-to-End  
📁 File: `02_end_to_end_machine_learning_project.ipynb`

---

## 🧭 Tujuan Bab

Bab ini memandu pembaca melalui **siklus hidup proyek Machine Learning secara end-to-end**, menekankan bahwa pelatihan model hanyalah satu bagian kecil dari keseluruhan proses.  
> 📌 ML bukan sekadar pelatihan model—tapi disiplin rekayasa menyeluruh yang mencakup data, domain, dan deployment.

---

## 🛠️ Langkah-Langkah Proyek ML

### 1️⃣ Memahami Masalah
- Definisikan tujuan bisnis dan kesuksesan model
- Identifikasi solusi saat ini & asumsi yang harus divalidasi
- Tentukan **metrik performa** yang selaras dengan kebutuhan bisnis

---

### 2️⃣ Mendapatkan Data
- Tentukan kebutuhan dan sumber data
- Perhatikan isu legal & privasi
- ⚠️ Buat dan simpan *test set* di awal, **jangan digunakan selama eksplorasi/pelatihan!**

---

### 3️⃣ Eksplorasi dan Visualisasi Data
- Analisis atribut: tipe data, nilai hilang, distribusi, outlier
- Visualisasi: Histogram, korelasi, hubungan antar fitur
- Eksperimen kombinasi fitur → temukan fitur menjanjikan

---

### 4️⃣ Persiapan Data untuk Algoritma ML

#### 📌 Pembersihan Data
- Hapus nilai hilang atau imputasi (mean, median, dll)

#### 📌 Penanganan Fitur Kategorikal/Tekstual
- Ubah ke bentuk numerik agar bisa diproses algoritma

#### 📌 Penskalaan dan Transformasi
- 🔄 Normalisasi / Standarisasi → penting untuk kinerja model

#### 📌 Rekayasa Fitur
- Pilih, buat, atau gabungkan fitur
- Gunakan teknik seperti PCA, ekstraksi statistik, dll

#### ⚙️ Pipeline Transformasi
- Bungkus semua transformasi dalam *pipeline* → reusable & bersih

---

### 5️⃣ Memilih & Melatih Model
- Coba berbagai algoritma klasifikasi/regresi
- Gunakan **Cross-Validation** untuk evaluasi performa yang akurat

---

### 6️⃣ Fine-Tuning Model
- Optimasi hyperparameter via:
  - 🔍 `GridSearchCV`
  - 🎲 `RandomizedSearchCV`
- Pertimbangkan **Ensemble Learning** untuk kinerja yang lebih baik

---

### 7️⃣ Deployment, Monitoring, Maintenance
- Terapkan model ke sistem produksi
- Lakukan monitoring performa berkelanjutan
- Siapkan strategi retraining, update data, dan pemeliharaan sistem

---

## 🧠 Insight Utama

> 📌 Bab ini mengubah mindset dari *“model trainer”* ke *“ML engineer”* yang bertanggung jawab atas **seluruh siklus hidup proyek ML**.

---
