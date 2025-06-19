# 📊 Bab 13: Memuat dan Memproses Data dengan TensorFlow  
📁 File: `13_loading_and_preprocessing_data.ipynb`

---

## 🧭 Ringkasan Bab

Bab ini membahas pentingnya **memuat dan memproses data secara efisien**, terutama untuk **dataset skala besar** yang tidak dapat ditangani sepenuhnya oleh Pandas atau transformer Scikit-Learn. Solusi utama yang diperkenalkan adalah **TensorFlow `tf.data` API**, yang dirancang untuk efisiensi, paralelisme, dan skalabilitas.

---

## ⚙️ Mengapa `tf.data`?

- 🚅 **Efisien dan Paralel**  
  Mendukung pemuatan data secara **multithreaded**, **parallel**, dan **streaming**.

- 🔁 **Pipelining Otomatis**  
  Saat GPU/TPU melatih batch saat ini, CPU menyiapkan batch berikutnya.

- 🔄 **Optimalisasi Aliran Data**  
  Sering kali **bottleneck bukan di model**, melainkan di tahap pemuatan data.

---

## 📂 Format File yang Didukung

- 📄 **CSV dan file teks**  
- 📦 **File biner tetap atau variabel**
- 🧬 **TFRecord**  
  Format biner efisien untuk skala besar; mendukung Protocol Buffers.

---

## 🧪 Langkah-Langkah Kunci dalam Pipeline Data

1. 🔗 **Chaining Transformations**  
   Susun berbagai tahap transformasi (`map`, `filter`, `batch`, dll.) ke dalam satu alur pipeline.

2. 🔀 **Shuffling**  
   Acak data untuk mencegah pembelajaran urutan tidak relevan.

3. 📎 **Interleaving from Multiple Files**  
   Membaca baris dari banyak file secara serentak (efisien dan merata).

4. 🧹 **Preprocessing Data**  
   Termasuk normalisasi, encoding kategori, penanganan nilai hilang, dan transformasi lainnya.

5. ⚡ **Prefetching**  
   Data batch berikutnya dimuat sambil model melatih batch saat ini → meningkatkan utilisasi GPU.

---

## 🤖 Integrasi dengan `tf.keras`

- Dataset `tf.data` dapat **langsung digunakan** sebagai input ke `.fit()`, `.evaluate()`, dan `.predict()` dalam Keras.
- Dukungan penuh untuk **batching otomatis**, **shuffling**, dan **prefetching**.

---

## 🧠 Insight Penting

Mengoptimalkan proses **loading & preprocessing data** sama pentingnya dengan merancang arsitektur model. Untuk pelatihan berskala besar, **efisiensi data pipeline** dapat berdampak langsung pada waktu pelatihan dan penggunaan sumber daya.

---
