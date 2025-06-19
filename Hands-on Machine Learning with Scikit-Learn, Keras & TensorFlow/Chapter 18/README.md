# 🎮 Bab 18: Pembelajaran Penguatan (Reinforcement Learning)  
📁 File: `18_reinforcement_learning.ipynb`

---

## 🧠 Tujuan Utama Bab

Bab ini memperkenalkan **Reinforcement Learning (RL)** — cabang pembelajaran mesin di mana **agen** belajar dari **interaksi dengan lingkungan** untuk memaksimalkan imbalan kumulatif.

---

## 🧩 Konsep Dasar RL

| Komponen       | Penjelasan                                                                 |
|----------------|----------------------------------------------------------------------------|
| **Agen**       | Entitas yang belajar dan mengambil keputusan.                              |
| **Lingkungan** | Dunia di mana agen beroperasi dan menerima feedback dari aksinya.         |
| **Tindakan**   | Pilihan yang tersedia untuk agen lakukan dalam lingkungan.                 |
| **Imbalan**    | Umpan balik numerik dari lingkungan (positif/negatif).                     |
| **Kebijakan**  | Strategi agen dalam memilih tindakan optimal berdasarkan pengalaman.       |

---

## 🧠 Tujuan RL

Agen bertujuan **belajar kebijakan optimal** melalui:
- Coba-coba (trial and error)
- Eksplorasi dan eksploitasi
- Optimisasi jangka panjang terhadap **imbal balik kumulatif**

---

## 💡 Contoh Sukses RL
- **Deep Blue**: Mengalahkan Garry Kasparov dalam catur.
- **AlphaGo**: Mengalahkan pemain terbaik dunia dalam Go.
- 🔗 **Deep Reinforcement Learning**: Kombinasi kekuatan **Deep Learning + RL** yang membuka era baru AI preskriptif.

---

## ⚙️ Algoritma RL yang Dibahas

### 🧊 Fixed Q-Value Targets
- Menggunakan nilai Q tetap (beku) selama pelatihan → stabilitas.

### 🧠 Double DQN (Deep Q-Network)
- Mengurangi overestimation dengan menggunakan dua jaringan Q yang berbeda.

### 🧮 Prioritized Experience Replay
- Memilih pengalaman masa lalu yang lebih *informatif* untuk dilatih ulang.

### ⚔️ Dueling DQN
- Memisahkan:
  - Estimasi nilai keadaan (*state value*)
  - Estimasi keuntungan tindakan (*advantage*)
- Meningkatkan efisiensi belajar dalam banyak skenario.

---

## 🏭 Aplikasi RL di Dunia Nyata

- 🤖 **Robotika**: Agen yang belajar bergerak atau memanipulasi objek.
- 🚘 **Sistem Otonom**: Mobil, drone, atau agen navigasi.
- 🕹️ **Game AI**: Game board atau video game kompleks.
- 🏭 **Optimisasi Industri**: Jadwal produksi, pengendalian suhu, dll.

---

## 🚀 Insight Akhir

> RL membuka era baru model **preskriptif** yang bukan hanya memahami data, tapi **mengambil keputusan** secara otonom dan adaptif.  
> Dari game hingga robot, Reinforcement Learning adalah inti dari agen cerdas masa depan.

---
