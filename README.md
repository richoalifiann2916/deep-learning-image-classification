# Proyek Klasifikasi Gambar Daun Tanaman

## Deskripsi Proyek
Proyek ini bertujuan untuk mengklasifikasikan kondisi daun tanaman ke dalam tiga kategori:
- healthy
- stressed
- diseased

Model utama yang digunakan adalah Custom CNN berbasis Sequential dengan layer Conv2D dan Pooling.

---

## Dataset
Dataset terdiri dari gambar daun tanaman yang telah dipetakan ke dalam tiga kelas utama:
- healthy
- stressed
- diseased

---

## Arsitektur Model
Model menggunakan:
- Conv2D
- MaxPooling2D
- BatchNormalization
- GlobalAveragePooling
- Dense
- Dropout

---

## Tahapan Proyek

### 1. Preprocessing
- Resize gambar ke 224x224
- Normalisasi pixel (0–1)

### 2. Training
- Optimizer: Adam
- Loss: Categorical Crossentropy (label smoothing)
- Epoch: 10

### 3. Evaluasi
Menggunakan:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 4. Inference
Model diuji menggunakan gambar baru untuk melihat generalisasi.

---

## Hasil
Model Custom CNN menunjukkan performa yang baik dengan akurasi tinggi dan training yang stabil.

---

## Struktur Folder
submission/
├── tfjs_model/
├── tflite/
├── saved_model/
├── notebook.ipynb
├── README.md
├── requirements.txt

---

## Cara Menjalankan

Install dependency:
pip install -r requirements.txt

Jalankan notebook:
jupyter notebook notebook.ipynb

---

## Deployment
Model dikonversi ke:
- SavedModel
- TensorFlow Lite
- TensorFlow.js

---

## Kesimpulan
Model berhasil melakukan klasifikasi kondisi daun tanaman dengan baik dan dapat digunakan untuk implementasi lebih lanjut.
