# 🔁 Bab 15: Memproses Urutan dengan RNN & CNN  
📁 File: `15_processing_sequences_using_rnns_and_cnns.ipynb`

---

## 📜 Ringkasan Bab

Bab ini menjelajahi **pemrosesan urutan (sequential data)** seperti teks, audio, dan deret waktu. Fokus utama adalah **Jaringan Saraf Berulang (RNN)** dan cara mereka digunakan untuk memproses input dengan panjang variabel, mempertahankan **konteks temporal**, serta **memprediksi masa depan** dalam urutan.

---

## 🔄 Konsep Dasar RNN

- 🔁 **Neuron Berulang (Recurrent Neurons)**  
  Memiliki koneksi ke dirinya sendiri, menyimpan "memori" dari waktu sebelumnya.

- 🧠 **Sel Memori & Keadaan Internal**  
  Digunakan untuk menyimpan informasi dari langkah-langkah sebelumnya dalam urutan.

- 🧩 **Backpropagation Through Time (BPTT)**  
  Algoritma pelatihan RNN yang memperluas backpropagation ke domain waktu.

---

## 📈 Aplikasi: Peramalan Deret Waktu

- 🕰️ **Model ARMA**: Model statistik klasik untuk prediksi deret waktu.  
- ⚙️ **Persiapan Data** untuk pelatihan model ML dari deret waktu.  
- 📊 **Model RNN untuk Prediksi**:  
  - RNN sederhana  
  - RNN dalam (Deep RNN)  
  - Prediksi Multivariat  
  - Prediksi Beberapa Langkah ke Depan

---

## 🔄 Arsitektur Lanjutan

- 🧱 **Sequence-to-Sequence (Seq2Seq)**  
  Cocok untuk terjemahan, chatbot, dan output berurutan lainnya.

- 🧮 **Masalah Vanishing & Exploding Gradients**  
  Diatasi dengan:
  - Recurrent Dropout  
  - Layer Normalization  

- 🧠 **LSTM & GRU**  
  Arsitektur yang lebih canggih untuk mempertahankan **memori jangka panjang**, dengan mekanisme gerbang untuk mengontrol aliran informasi.

---

## 🧠 Aplikasi RNN dalam Dunia Nyata

- 📈 Prediksi harga saham / ekonomi
- 🚗 Prediksi lintasan mobil otonom
- 📝 Pengenalan tulisan tangan
- 🌍 Terjemahan bahasa otomatis
- 🗣️ Speech-to-text & chatbot

---

## 💡 Insight Penting

> RNN membuka potensi pembelajaran mesin untuk memahami **urutan dan konteks waktu**, menjadikannya fondasi banyak aplikasi AI canggih.

---
