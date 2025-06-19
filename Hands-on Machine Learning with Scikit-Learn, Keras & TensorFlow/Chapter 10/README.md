# 🧠 Bab 10: Jaringan Saraf dengan Keras  
📁 File: `10_neural_nets_with_keras.ipynb`

---

## 🚀 Transisi ke Deep Learning

Bab ini menandai transisi dari pembelajaran mesin klasik ke **pembelajaran mendalam** dengan pengenalan **Artificial Neural Networks (ANN)** dan implementasinya menggunakan **Keras**, API tinggi dari TensorFlow.

ANN dirancang berdasarkan inspirasi dari **neuron biologis**, dan telah menjadi pilar utama untuk:
- 🔤 Pengenalan suara
- 📷 Klasifikasi gambar berskala besar
- 🧬 Tugas-tugas kompleks lainnya di dunia nyata

---

## 🧬 Evolusi Konsep

- 🧠 **Neuron Biologis** → Inspirasi awal
- ⚙️ **Neuron Buatan** → Unit dasar ANN
- 🔘 **Perceptron** → Model ANN linear sederhana
- 🧱 **Multilayer Perceptron (MLP)** → ANN berlapis-lapis
- 🔄 **Backpropagation** → Algoritma pelatihan utama MLP

MLP dapat digunakan untuk:
- 🔢 Regresi
- 🏷️ Klasifikasi

---

## 🛠️ Membangun Jaringan Saraf dengan Keras

### 🔹 Sequential API
- Cara termudah untuk membangun jaringan sekuensial lapisan
- Cocok untuk model linier sederhana

### 🔹 Functional API
- Lebih fleksibel
- Bisa menangani input/output ganda dan koneksi non-linier antar lapisan

### 🔹 Subclassing API
- Kontrol penuh atas arsitektur
- Cocok untuk model dinamis dan eksperimen lanjutan

---

## 💾 Fitur Penting

- 💽 **Saving & Loading Models**  
  Simpan bobot dan arsitektur model untuk reuse / kelanjutan pelatihan

- ⚙️ **Callbacks**  
  Contoh: EarlyStopping, ModelCheckpoint, LearningRateScheduler

- 📊 **TensorBoard**  
  Alat visualisasi untuk:
  - Kurva pelatihan
  - Grafik model
  - Analisis hyperparameter

---

## 🧪 Penyetelan Hyperparameter

Penting dalam meningkatkan performa jaringan saraf. Termasuk:
- 🔢 Jumlah lapisan tersembunyi
- 🔘 Jumlah neuron per lapisan
- ⚡ Learning rate
- 📦 Batch size
- 🔁 Epochs

> 🔍 Memahami pengaruh masing-masing hyperparameter penting untuk pelatihan model yang efisien dan optimal

---

## 📘 Ringkasan

> Bab ini membekali Anda untuk membangun dan melatih **neural networks** dari nol menggunakan **Keras**, sekaligus memahami struktur internal dan proses pembelajarannya.

---
