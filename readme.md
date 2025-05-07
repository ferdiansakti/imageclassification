# Proyek Klasifikasi Gambar: Rice Image Dataset

## Deskripsi Proyek
Proyek ini bertujuan untuk mengembangkan model klasifikasi gambar menggunakan dataset gambar beras (Rice Image Dataset). Dataset ini terdiri dari lima kelas beras: Arborio, Basmati, Ipsala, Jasmine, dan Karacadag. Proyek ini menggunakan TensorFlow dan TensorFlow.js untuk membangun dan melatih model deep learning, serta menyediakan visualisasi dan analisis hasil pelatihan.

## Dataset
Dataset yang digunakan adalah [Rice Image Dataset](https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset), yang berisi 75.000 gambar beras dari 5 kelas berbeda. Dataset ini diunduh langsung dari Kaggle menggunakan API.

## Struktur Direktori
- `dataset/`: Direktori yang berisi dataset gambar beras.
- `Submission_Akhir_Klasifikasi_Gambar_Ferdian_Sakti.ipynb`: Notebook Jupyter yang berisi kode implementasi proyek.

## Library yang Digunakan
- TensorFlow
- TensorFlow.js
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- OpenCV (untuk pra-pemrosesan gambar)

## Langkah-Langkah Proyek
1. **Persiapan Data**:
   - Mengunduh dataset dari Kaggle.
   - Mengekstrak dataset ke direktori yang sesuai.
   - Membagi dataset menjadi data latih dan data validasi.

2. **Pra-pemrosesan Data**:
   - Normalisasi gambar.
   - Augmentasi data untuk meningkatkan variasi data latih.

3. **Pembangunan Model**:
   - Membangun model CNN menggunakan TensorFlow.
   - Menambahkan lapisan Conv2D, MaxPooling2D, Flatten, Dense, Dropout, dan BatchNormalization.
   - Menggunakan optimizer RMSprop dan callback seperti EarlyStopping dan ModelCheckpoint.

4. **Pelatihan Model**:
   - Melatih model dengan data latih.
   - Memantau akurasi dan loss selama pelatihan.

5. **Evaluasi Model**:
   - Mengevaluasi model menggunakan data validasi.
   - Membuat visualisasi akurasi dan loss.
   - Menghasilkan classification report dan confusion matrix.

6. **Ekspor Model**:
   - Menyimpan model dalam format TensorFlow.js untuk penggunaan di web.

## Hasil
Model yang dikembangkan mencapai akurasi yang tinggi dalam mengklasifikasikan gambar beras ke dalam lima kelas yang berbeda. Hasil pelatihan dan evaluasi ditampilkan dalam bentuk grafik dan metrik evaluasi.

## Cara Menjalankan Proyek
1. Unduh dataset dari Kaggle dan letakkan di direktori `dataset/`.
2. Buka notebook `Submission_Akhir_Klasifikasi_Gambar_Ferdian_Sakti.ipynb` di Jupyter Notebook atau Google Colab.
3. Jalankan setiap sel secara berurutan untuk memproses data, melatih model, dan mengevaluasi hasil.

## Referensi
- Dokumentasi TensorFlow: https://www.tensorflow.org/
- Dokumentasi TensorFlow.js: https://www.tensorflow.org/js
- Dataset Rice Image: https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset

## Catatan
Pastikan untuk menginstal semua library yang diperlukan sebelum menjalankan notebook. Gunakan lingkungan virtual atau Google Colab untuk menghindari konflik dependensi.