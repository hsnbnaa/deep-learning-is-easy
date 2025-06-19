# 📘 Bab 7: Pembelajaran Ensemble dan Hutan Acak (Ensemble Learning & Random Forests)  
📁 File: `07_ensemble_learning_and_random_forests.ipynb`

---

## 🧭 Tujuan Bab

Bab ini memperkenalkan konsep **Ensemble Learning**, strategi powerful dalam Machine Learning di mana beberapa model (prediktor) digabungkan untuk menciptakan prediksi yang lebih akurat, stabil, dan tangguh daripada model tunggal.

> 🧠 Konsep ini berakar pada prinsip **"wisdom of the crowd"** — gabungan banyak model sederhana seringkali mengungguli model tunggal yang kompleks.

---

## 🧩 Metode Ensemble yang Dibahas

### 📮 1. Voting Classifiers
- Menggabungkan output dari beberapa model klasifikasi berbeda.
- Prediksi akhir berdasarkan **suara mayoritas**.
- Cocok saat setiap model individu memiliki performa berbeda di kasus yang berbeda.

---

### 📦 2. Bagging & Pasting
#### 🟢 Bagging (Bootstrap Aggregating)
- Setiap model dilatih pada subset acak **dengan penggantian (bootstrap)**.
- Hasil model digabung (voting/mean) untuk generalisasi lebih baik.

#### 🔵 Pasting
- Seperti Bagging, tapi **tanpa penggantian** (tanpa bootstrap).

#### 🧪 Out-of-Bag Evaluation
- Digunakan untuk mengukur performa model **tanpa perlu set validasi terpisah**.
- Berdasarkan data yang **tidak terlihat oleh model saat pelatihan**.

#### 🔀 Random Patches & Subspaces
- Melatih model dengan subset instans **dan** subset fitur:
  - **Random Patches**: subset instans + fitur
  - **Random Subspaces**: semua instans + subset fitur

---

### 🌲 3. Random Forest
- Kumpulan **Decision Trees** dilatih menggunakan Bagging dan subset fitur.
- Sangat tangguh, akurat, dan populer untuk berbagai tugas ML.
- Bisa digunakan untuk:
  - Klasifikasi
  - Regresi
  - 📊 Menilai **Feature Importance**

#### 🔶 Extra-Trees
- Varian Random Forest dengan **lebih banyak randomisasi** (misalnya, split titik dipilih secara acak).
- ⚡️ Lebih cepat dan terkadang lebih baik generalisasinya.

---

### 🔺 4. Boosting
- **Model lemah dilatih secara berurutan**, dengan fokus pada kesalahan sebelumnya.
- Setiap model berusaha **memperbaiki kelemahan** dari model sebelumnya.

Contoh populer:
- ⚡ **AdaBoost (Adaptive Boosting)**
- 🚀 **Gradient Boosting**
- 🧱 **Histogram-Based Gradient Boosting**  
  (lebih efisien, diperkenalkan di Scikit-Learn edisi terbaru)

---

### 🧠 5. Stacking (Stacked Generalization)
- Level lanjutan dari ensemble:
  - Melatih model meta (**meta-learner**) untuk menggabungkan prediksi dari beberapa model dasar.
- Pendekatan cerdas: belajar **kapan harus mempercayai prediktor tertentu**.

---

## ✅ Kapan Menggunakan Ensemble?

- Ketika kamu sudah memiliki beberapa **model baik** → gabungkan untuk hasil lebih solid.
- Banyak solusi pemenang kompetisi ML (seperti Kaggle) memanfaatkan teknik ensemble.
- Fokus bukan pada "model terbaik", tapi membangun **sistem terbaik**.

---

## 💡 Insight Utama

> 💥 Ensemble Learning mengubah fokus ML modern dari mencari satu model terbaik  
> → menjadi **mengorkestrasi banyak model sederhana untuk hasil maksimal**.

> 🎯 Teknik ensemble seperti Random Forest dan Gradient Boosting adalah **senjata utama** dalam ML produksi.

---

