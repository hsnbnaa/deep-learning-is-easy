# 🧠 Bab 11: Melatih Jaringan Saraf Dalam  
📁 File: `11_training_deep_neural_networks.ipynb`

---

## 🎯 Fokus Bab

Bab ini membahas **tantangan utama dalam pelatihan Deep Neural Networks (DNN)** dan menyediakan **teknik lanjutan** untuk mengatasinya. Topik-topik mencakup masalah optimasi, overfitting, inisialisasi bobot, dan penggunaan kembali model yang telah dilatih.

---

## ⚠️ Tantangan Utama dalam Pelatihan DNN

- 📉 **Vanishing / Exploding Gradients**  
  Gradien terlalu kecil atau terlalu besar, menghambat pelatihan lapisan terdalam.

- 🧪 **Data Berlabel Tidak Cukup**  
  DNN membutuhkan data besar dan mahal untuk dilabeli secara manual.

- 🐢 **Pelatihan Lambat**  
  Karena ukuran jaringan dan kompleksitas data.

- 🧠 **Overfitting**  
  Model kompleks mudah menyesuaikan data pelatihan terlalu baik, merugikan generalisasi.

---

## 🧰 Solusi untuk Masalah Gradien

- 📏 **Inisialisasi Bobot**  
  - **Xavier (Glorot) Initialization**  
  - **He Initialization**

- 🔁 **Fungsi Aktivasi yang Stabil**  
  - **ReLU**, **Leaky ReLU**, **ELU**, **SELU**

- ⚖️ **Normalisasi**  
  - **Batch Normalization**  
  - **Layer Normalization**

- ✂️ **Gradient Clipping**  
  Membatasi ukuran gradien untuk mencegah exploding gradients.

---

## 🔁 Transfer Learning & Pretraining

- 🔄 **Transfer Learning**  
  Gunakan model yang telah dilatih sebelumnya (misal: ImageNet).

- 🧩 **Unsupervised Pretraining**  
  Pelajari representasi menggunakan autoencoder sebelum supervised learning.

- 🧠 **Auxiliary Tasks**  
  Gunakan tugas pembantu dengan banyak data sebagai pretraining.

---

## ⚡ Optimizer Canggih

- 💡 Alternatif dari SGD biasa:
  - **Momentum**
  - **Nesterov**
  - **AdaGrad**
  - **RMSProp**
  - **Adam**, **AdaMax**, **Nadam**, **AdamW**

- 📉 **Learning Rate Scheduling**  
  Sesuaikan learning rate selama pelatihan untuk hasil lebih stabil.

---

## 🛡️ Regularisasi untuk Cegah Overfitting

- 🧮 **L1 / L2 Regularization**  
  Penalti terhadap besarnya bobot.

- 🔄 **Dropout**  
  Nonaktifkan neuron acak saat pelatihan.

- 🎲 **Monte Carlo Dropout**  
  Gunakan dropout juga saat inferensi untuk mengukur ketidakpastian.

- 📉 **Max-Norm Regularization**  
  Batasi besarnya bobot maksimum per neuron.

---

## 📘 Ringkasan

> Deep Learning bukan hanya soal membuat arsitektur besar, tapi juga menguasai seni **penyetelan, normalisasi, dan regularisasi**. Bab ini mengajarkan bahwa sukses dalam DL memerlukan pemahaman teknik canggih serta praktik terbaik dalam pelatihan model.

---
