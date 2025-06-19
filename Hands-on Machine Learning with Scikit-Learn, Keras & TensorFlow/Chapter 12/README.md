# ⚙️ Bab 12: Model Kustom dan Pelatihan dengan TensorFlow  
📁 File: `12_custom_models_and_training_with_tensorflow.ipynb`

---

## 🧭 Ringkasan Bab

Bab ini memperkenalkan penggunaan **API tingkat rendah TensorFlow** untuk membangun dan melatih model secara **kustom**. Meskipun `tf.keras` mencakup 95% kasus penggunaan, terdapat skenario di mana pengembang membutuhkan **kontrol penuh**, seperti saat membuat:

- Fungsi loss/metrik kustom
- Lapisan atau model tidak standar
- Regularisasi dan batasan bobot unik
- Training loop yang kompleks

---

## 🔧 Tur Cepat TensorFlow

- 🔢 **Tensors & Operasi** mirip NumPy
- 🔄 **Konversi tipe dan variabel**
- 📦 Struktur data internal TensorFlow

---

## 🛠️ Komponen Kustom

> Untuk fleksibilitas dan eksperimen lanjutan, Anda dapat membuat:

- 🧮 **Fungsi Loss Kustom**  
  Dirancang khusus untuk target atau strategi optimasi unik.

- 📏 **Metrik Kustom**  
  Ukur performa model dengan cara yang tidak umum/standar.

- 🔢 **Fungsi Aktivasi, Regularisasi, Inisialisasi, Batasan**  
  Modifikasi detail perilaku lapisan.

- 🧱 **Lapisan Kustom**  
  Buat arsitektur model yang benar-benar unik.

- 🧠 **Model Kustom dengan Subclassing API**  
  Kontrol penuh atas proses `forward()` dan struktur.

- 🎯 **Loss atau metrik berbasis nilai internal model**  
  Misal: penalti terhadap aktivasi tertentu di hidden layer.

---

## 🔁 Training Loop Kustom

> Berguna untuk:
- Modifikasi gradien secara manual
- Penggunaan optimizer berbeda di bagian berbeda model
- Logging/monitoring non-standar

Meliputi:

- 🔬 **Autodiff**: Gunakan `tf.GradientTape()` untuk menghitung gradien otomatis.
- ⚙️ **Step-by-step training loop**: Kendali penuh atas training, evaluasi, dan logging.

---

## 🚀 Fungsi & Grafik TensorFlow

- 📜 **AutoGraph**: Konversi fungsi Python ke grafik TensorFlow otomatis.
- 🔄 **Tracing**: Proses konversi fungsi ke bentuk grafik (sekali, lalu dieksekusi cepat).
- 📏 **Aturan Fungsi TF**: Best practices agar fungsi Python kompatibel dengan AutoGraph.
- 📦 **Pengelolaan variabel dan resource** saat menggunakan grafik (misalnya model checkpoint, stateful layer).

---

## 🧠 Insight Penting

TensorFlow adalah framework **berlapis**:
- 💡 **Tingkat tinggi**: `tf.keras` → mudah dan cepat untuk penggunaan umum.
- 🔍 **Tingkat rendah**: API kustom TensorFlow → kontrol penuh untuk kasus riset, eksperimen lanjutan, atau pengembangan fitur baru.

---
