# Machine-Learning-Bitcoin-Classification

---Prediksi Pergerakan Harga Bitcoin Menggunakan Algoritma Machine Learning (Klasifikasi)---

Repositori ini berisi proyek tugas mata kuliah Machine Learning. Proyek ini bertujuan untuk membangun model prediktif berbasis Machine Learning untuk mengklasifikasikan arah pergerakan harian harga Bitcoin (BTC-USD) apakah akan mengalami kenaikan atau penurunan pada hari berikutnya.

    #Deskripsi Proyek & Tujuan Penelitian
Tujuan Penelitian: Membangun dan melatih model Machine Learning untuk memprediksi kecenderungan arah pergerakan harga Bitcoin (Naik/Turun) berdasarkan data historis, serta memahami penerapan alur kerja pipeline Data Science secara utuh.

    #Mengapa Menggunakan Bitcoin?
Bitcoin dipilih sebagai objek studi karena memiliki volatilitas tinggi, data perdagangan harian yang terbuka secara global, serta jumlah baris data historis yang sangat masif (>1.000 data baris), sehingga sangat ideal untuk pengujian algoritma time-series.

    #Nama Dataset 
Bitcoin BTC-USD stock dataset, adalah dataset yg saya gunakan dan saya download dari Kaggle, tapi file nya saya rename agar tidak kepanjangan jadinya saya rename menjadi BTC_Price.csv 

    #Jumlah Data:
>1000 atau tepatnya : 2836(Baris) dan 7(Kolom)

    #Total Variabel / Kolom:
Variabel Fitur (Input / $X$): Open, High, Low, Close, Volume, dan MA_20 (Moving Average 20 hari sebagai tambahan feature engineering).
Variabel Target (Output / $y$): Target (Kategori biner: 1 jika harga Close besok naik, 0 jika turun/tetap).

    #Alur & Metodologi
-Data Loading & Cleaning: Memuat dataset ke Google Colab menggunakan pustaka pandas, mengecek dimensi data, serta membersihkan missing values.

-Feature Engineering: Membuat kolom target kategorikal (Target) dan indikator teknikal sederhana (MA_20).

-Data Splitting (Time-Series Split): Membagi data dengan rasio 80% Training dan 20% Testing secara sekuensial kronologis (tanpa pengacakan / tanpa shuffle) untuk mencegah data leakage.

-Data Modeling: Menggunakan algoritma Random Forest Classifier untuk melatih model klasifikasi.

-Model Evaluation: Mengevaluasi performa model menggunakan metrik Accuracy, Precision, dan Recall (karena menggunakan pendekatan klasifikasi).


