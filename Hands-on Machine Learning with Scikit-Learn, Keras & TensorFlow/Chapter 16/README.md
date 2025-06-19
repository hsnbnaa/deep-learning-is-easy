# 🧠 Bab 16: NLP dengan RNN dan Attention  
📁 File: `16_nlp_with_rnns_and_attention.ipynb`

---

## 📜 Ringkasan Bab

Bab ini memperkenalkan **Pemrosesan Bahasa Alami (Natural Language Processing / NLP)** — bidang AI yang berfokus pada pemahaman dan generasi bahasa manusia. Topik utama mencakup penggunaan **RNN**, **mekanisme perhatian (attention)**, dan **Transformer**, yang telah merevolusi NLP modern.

---

## 📚 Fokus NLP

- 🗣️ **Tugas-Tugas NLP Umum**:
  - Klasifikasi teks
  - Terjemahan mesin
  - Ringkasan otomatis
  - Penjawaban pertanyaan
  - Pembuatan teks

- 📖 **RNN Karakter**:
  - Model dilatih untuk memprediksi karakter berikutnya dari teks.
  - Dapat digunakan untuk menghasilkan teks baru dari contoh pelatihan.

---

## 🔄 Arsitektur Terjemahan Bahasa

- 🔁 **Encoder–Decoder RNN**:
  - Encoder memproses input (bahasa sumber).
  - Decoder menghasilkan output (bahasa target).
  - Digunakan untuk tugas terjemahan mesin.

---

## ⚡ Revolusi Transformer

- ⚙️ **Transformer Model**:
  - Mengandalkan **self-attention**.
  - Mengatasi keterbatasan RNN pada urutan panjang dan pelatihan lambat.
  - Mendukung paralelisme dan lebih efisien di GPU.

- 🧮 **Keunggulan**:
  - Menangani dependensi jangka panjang dengan lebih baik.
  - Lebih mudah ditingkatkan dan dilatih secara efisien.

---

## 🧠 Model Bahasa Besar

- 🔀 **Switch Transformers**:
  - Mengaktifkan subset parameter berbeda untuk tiap token input.

- 🔤 **DistilBERT, T5, dan PaLM**:
  - Model besar yang sukses dalam banyak tugas NLP.

- 🧩 **Chain-of-Thought Prompting**:
  - Memungkinkan model menyusun langkah penalaran sebelum jawaban akhir.
  - Meningkatkan kemampuan reasoning dan akurasi.

---

## 🔁 Transformasi ke Luar NLP

- 🖼️ **Vision Transformers (ViT)**:
  - Gambar dibagi menjadi patch, lalu diproses seperti token teks.
  - Dapat menangani tugas visi komputer secara efisien.

- 🌐 **Model Visual Transformer Lain**:
  - DeiT, Perceiver, DINO

- 🌟 **Model Multimodal Besar**:
  - CLIP, DALL·E, Flamingo, GATO
  - Mampu memproses kombinasi modalitas: teks, gambar, audio, dll.

---

## 💡 Insight Penting

> Arsitektur Transformer dan attention telah mentransformasi NLP dan memperluas kemampuan deep learning ke berbagai domain — menandai era **model serbaguna dan multimodal**.

---
