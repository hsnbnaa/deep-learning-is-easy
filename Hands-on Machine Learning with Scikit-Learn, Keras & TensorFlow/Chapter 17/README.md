# 🧠 Bab 17: Autoencoder, GAN, dan Model Difusi  
📁 File: `17_autoencoders_gans_and_diffusion_models.ipynb`

---

## 🎯 Tujuan Utama Bab

Bab ini memperkenalkan **Model Generatif** dalam deep learning — model yang dapat menciptakan data baru yang realistis. Ini merupakan pergeseran dari fokus sebelumnya pada klasifikasi/prediksi menuju **kreasi data sintetis**.

---

## 🔧 Jenis Model Generatif

### 1. 🌀 Autoencoder

- **Tujuan**: Belajar menyalin input ke output → menemukan representasi laten yang padat.
- **Struktur**:
  - `Encoder`: Mengubah input ke representasi laten.
  - `Decoder`: Mengembalikan representasi laten ke bentuk semirip mungkin dengan input.
- **Reconstruction Loss**: Mengukur selisih antara input dan output, digunakan untuk pelatihan.
- **Undercomplete Autoencoder**:
  - Representasi laten berdimensi lebih kecil → memaksa autoencoder mempelajari fitur penting.
- **Aplikasi**:
  - Reduksi dimensi
  - Visualisasi
  - Pretraining unsupervised
  - Model generatif sederhana
- ✅ **Implementasi**: Autoencoder bertumpuk (stacked autoencoder) dengan Keras

---

### 2. 🤖 Generative Adversarial Networks (GAN)

- **Struktur**:
  - `Generator`: Mengubah vektor acak (mis. distribusi Gaussian) menjadi data (gambar palsu).
  - `Discriminator`: Menilai apakah gambar asli atau palsu.
- **Pelatihan Adversarial**:
  - Generator → mencoba menipu Discriminator
  - Discriminator → mencoba membedakan asli vs palsu
  - Proses kompetitif mendorong kualitas tinggi
- **Aplikasi GAN**:
  - Super resolution (peningkatan resolusi gambar)
  - Colorization (memberi warna)
  - Image-to-image translation
  - Video prediction
  - Dataset augmentation

---

### 3. 🌫️ Diffusion Models

- **Contoh**: Denoising Diffusion Probabilistic Model (DDPM)
- **Prinsip Dasar**:
  - Belajar menghilangkan noise secara bertahap dari gambar
  - Dari noise → menjadi gambar yang realistis
- **Kelebihan**:
  - Mampu menghasilkan gambar dengan kualitas tinggi
  - Semakin populer dalam generative AI
- ✅ **Implementasi**: Disusun langkah demi langkah dari awal untuk pemahaman mendalam

---

## 💡 Insight Penting

> Model generatif mengubah paradigma machine learning dari sekadar "memahami data" menjadi **"menciptakan data baru"**.  
> Ini membuka aplikasi baru dalam:
> - 🎨 Seni dan desain  
> - 📊 Augmentasi data  
> - 🎮 Simulasi  
> - 🧪 Riset ilmiah  

---
