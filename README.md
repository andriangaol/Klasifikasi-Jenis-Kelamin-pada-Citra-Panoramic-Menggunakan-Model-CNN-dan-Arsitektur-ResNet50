# 🦷 Klasifikasi Jenis Kelamin pada Citra Panoramic Menggunakan CNN dan ResNet50 🧑‍🔬

## 📖 Latar Belakang
Identifikasi jenis kelamin adalah langkah penting dalam **investigasi forensik**, terutama ketika kondisi fisik korban tidak memungkinkan untuk dikenali. Salah satu metode yang efektif adalah melalui **analisis citra panoramik gigi**, yang menunjukkan perbedaan struktural antara pria dan wanita pada rahang dan gigi. Penelitian ini bertujuan untuk **membandingkan kinerja dua model berbasis Convolutional Neural Network (CNN)**, yaitu **model CNN sederhana** dan **ResNet50** dengan pendekatan **Transfer Learning**, dalam klasifikasi jenis kelamin menggunakan citra panoramik gigi.

## ⚙️ Tujuan
1. Membangun model CNN dan ResNet50 untuk klasifikasi jenis kelamin berdasarkan citra panoramik gigi.
2. Mengukur akurasi, presisi, recall, dan F1-score dari kedua model.
3. Mengevaluasi efisiensi waktu pelatihan dari kedua model.

## 📊 Hasil
- **Model CNN**:
  - **Akurasi**: 94%
  - **Presisi**: 100% (Pria), 89% (Wanita)
  - **Recall**: 88% (Pria), 100% (Wanita)
  - **F1-Score**: 0.93 (Pria), 0.94 (Wanita)

- **Model ResNet50**:
  - **Akurasi**: 86%
  - **Presisi**: 93% (Pria), 80% (Wanita)
  - **Recall**: 78% (Pria), 94% (Wanita)
  - **F1-Score**: 0.84 (Pria), 0.87 (Wanita)

### Kesimpulan:
Model **CNN** terbukti lebih efektif dengan **akurasi lebih tinggi** dan **waktu pelatihan lebih singkat** dibandingkan **ResNet50**, menjadikannya pilihan yang lebih baik untuk aplikasi forensik berdasarkan citra panoramik gigi.

---

## ⚙️ Prasyarat

### Instalasi
```bash
pip install -r requirements.txt
```

---

## 🧑‍💻 Penggunaan
### Langkah 1: Persiapkan Dataset
- Dataset diunduh melalui Kaggle dan berisi dua kelas: **Pria** dan **Wanita**.
- Dataset dibagi menjadi **Data Latih (686 gambar)**, **Data Validasi (97 gambar)**, dan **Data Uji (196 gambar)**.

### Langkah 2: Pelatihan Model
Model CNN dan ResNet50 dibangun menggunakan Keras dan TensorFlow. Anda bisa memilih untuk melatih kedua model ini dan melihat perbandingannya berdasarkan **akurasi**, **presisi**, **recall**, dan **f1-score**.

### Langkah 3: Evaluasi Model
Evaluasi dilakukan menggunakan **confusion matrix** untuk mengukur kinerja model, dengan metrik utama sebagai berikut:

- **Akurasi**: Persentase prediksi yang benar.
- **Presisi**: Akurasi model dalam memprediksi kelas positif.
- **Recall**: Kemampuan model dalam mendeteksi semua kasus positif.
- **F1-Score**: Keseimbangan antara presisi dan recall.

---

## 📚 Referensi
1. A. Markande, M. David, dan A. Indira, "Mandibular ramus: An indicator for sex determination," *J. Forensic Dent. Sci.*, 2012.
2. F. Faqihuddin, S. M. T. Ibrahim, dan Y. Widiastiwi, "Klasifikasi Jenis Kelamin dengan LVQ," *Semin. Nas. Mhs. Ilmu Komput. dan Apl.*, 2021.

---

## 💬 Kontribusi
Jika Anda tertarik untuk berkontribusi pada proyek ini, silakan lakukan **fork** dan kirimkan **pull request** dengan perubahan yang Anda buat.

---

## 📚 Data
- [**Kaggle Dataset**](https://www.kaggle.com)
- [**ResNet50**](https://keras.io/api/applications/resnet/#resnet50-function)
```
