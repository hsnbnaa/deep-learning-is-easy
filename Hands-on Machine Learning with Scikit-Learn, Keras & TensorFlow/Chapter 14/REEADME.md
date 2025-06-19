# 🖼️ Bab 14: Deep Computer Vision dengan CNN  
📁 File: `14_deep_computer_vision_with_cnns.ipynb`

---

## 🧠 Ringkasan Bab

Bab ini memperkenalkan **Jaringan Saraf Konvolusional (CNN)** — arsitektur utama dalam **visi komputer modern**, terinspirasi oleh cara kerja **korteks visual manusia**. CNN memungkinkan komputer untuk **belajar mengenali pola visual** dari data mentah seperti gambar.

---

## 🔍 Intuisi Biologis

CNN terinspirasi dari cara **sel di korteks visual** merespons area kecil dari medan pandang. Lapisan-lapisan CNN meniru cara otak mengenali pola visual, dimulai dari deteksi tepi, tekstur, hingga objek yang lebih kompleks.

---

## 🧱 Komponen Utama CNN

- 🧮 **Filter / Kernel**  
  Matriks kecil yang "meluncur" di atas gambar untuk mendeteksi fitur lokal seperti tepi atau pola.

- 🌐 **Feature Maps**  
  Output dari konvolusi. Setiap feature map menunjukkan di mana fitur tertentu muncul dalam input.

- 🏗️ **Stacking Multiple Feature Maps**  
  Digunakan untuk menangkap berbagai fitur pada waktu yang bersamaan.

- 🔽 **Pooling Layers**  
  Digunakan untuk **mengurangi dimensi spasial**, mengurangi jumlah parameter, dan meningkatkan ketahanan terhadap translasi kecil.
  
  - 📌 **Max Pooling**: Ambil nilai maksimum dalam jendela.  
  - 📌 **Average Pooling**: Ambil nilai rata-rata.

---

## 🛠️ Implementasi dengan Keras

Bab ini memandu pengguna dalam:

- Membangun arsitektur CNN menggunakan `tf.keras`
- Menyusun lapisan konvolusional, aktivasi (misal: ReLU), pooling, flattening, dan dense
- Menangani **masalah memori** dalam pelatihan CNN

---

## 💡 Aplikasi CNN

- 🚘 Mobil otonom
- 🔍 Pencarian gambar
- 📹 Analisis video real-time
- 🩺 Diagnostik medis otomatis

---

## 🧠 Insight Penting

> "CNN menunjukkan bagaimana kekuatan DL berasal dari sinergi antara inspirasi biologis, kekuatan komputasi modern, dan kemajuan algoritmik."

---
