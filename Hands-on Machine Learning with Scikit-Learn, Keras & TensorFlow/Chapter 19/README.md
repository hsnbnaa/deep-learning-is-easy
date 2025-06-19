# 🚀 Bab 19: Pelatihan dan Penerapan Model TensorFlow dalam Skala Besar  
📁 File: `19_training_and_deploying_at_scale.ipynb`

---

## 🎯 Tujuan Bab

Bab ini menekankan pentingnya **menerapkan model ML ke lingkungan produksi**, karena prediksi yang akurat hanya bernilai jika bisa digunakan secara nyata oleh sistem operasional atau pengguna akhir.

---

## 🧪 Skenario Penerapan Model

| Skema             | Deskripsi                                                                 |
|-------------------|---------------------------------------------------------------------------|
| **Batch Processing** | Menjalankan model pada kumpulan data secara berkala (misalnya setiap malam). |
| **Web Service**      | Menyediakan model dalam bentuk REST API untuk prediksi secara real-time.     |

---

## ⚠️ Tantangan dalam Penerapan Skala Besar

### 🧬 Versi Model
- Model harus terus diperbarui, diuji, dan dapat **rollback** jika performanya menurun.

### ⚙️ Skalabilitas
- Sistem harus mampu melayani ribuan kueri per detik (QPS) saat produk digunakan luas.

### 🧪 A/B Testing
- Menjalankan beberapa versi model sekaligus untuk membandingkan kinerja di dunia nyata.

---

## 🛠️ Alat dan Teknologi Skala Produksi

### 🧾 TensorFlow Serving
- Menyediakan model TensorFlow dengan efisien.
- Mendukung transisi antar versi model secara mulus.

### ☁️ Google Vertex AI
- Platform cloud untuk:
  - Pelatihan besar-besaran
  - Penyetelan hyperparameter
  - Menerapkan model ML end-to-end

### 🎯 Distributed Keras Tuner
- Menjalankan pencarian hyperparameter secara paralel dalam skala besar.

### 🌐 TensorFlow.js
- Menjalankan dan menguji model langsung di browser web pengguna.

---

## 🧩 Teknik Pelatihan Skala Besar

### ⛓️ PipeDream dan Pathways
- Pelatihan model besar secara efisien pada infrastruktur multi-node.

### 🧠 Model vs. Data Parallelism
| Strategi            | Penjelasan                                                               |
|---------------------|--------------------------------------------------------------------------|
| **Data Parallelism** | Membagi data ke banyak device, tiap device melatih model penuh.         |
| **Model Parallelism**| Membagi bagian model ke banyak device, setiap device melatih sebagian. |

### 🖥️ Pelatihan di TensorFlow Cluster
- Cara mengatur pelatihan pada klaster terdistribusi agar efisien dalam skala besar.

---

## ✅ Kesimpulan

> Menerapkan model ML secara efektif di dunia nyata memerlukan perpaduan antara *machine learning* dan *rekayasa sistem skala besar*.

💡 **Pembelajaran mesin bukan selesai saat model dilatih, tapi ketika model memberikan dampak nyata melalui sistem produksi.**

---
