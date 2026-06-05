# Forecasting-Indonesia-Open-Unemployment-Rate
Forecasting Indonesia open unemployment rate using Time Series Analysis

Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis dan memprediksi Tingkat Pengangguran Terbuka (TPT) Provinsi Jawa Tengah menggunakan pendekatan Time Series Forecasting. Data yang digunakan merupakan data semesteran (Februari dan Agustus) dari tahun 2005 hingga 2026.

Melalui proyek ini dilakukan eksplorasi data, pengujian karakteristik time series, perbandingan beberapa model forecasting, serta pembuatan proyeksi TPT untuk beberapa tahun ke depan.

Tujuan Proyek
Menganalisis pola historis Tingkat Pengangguran Terbuka (TPT).
Mengidentifikasi tren dan pola musiman pada data.
Membandingkan performa beberapa model forecasting.
Membuat proyeksi TPT untuk mendukung pengambilan keputusan berbasis data.
Dataset

Karakteristik dataset:

Wilayah: Jawa Tengah
Variabel utama: Tingkat Pengangguran Terbuka (TPT)
Periode: Februari 2005 – Februari 2026
Frekuensi: Semesteran (Februari dan Agustus)
Jumlah observasi: 43 data
Tahapan Analisis

1. Data Preprocessing

Tahapan yang dilakukan:

Mengubah kolom tanggal menjadi format datetime.
Menjadikan tanggal sebagai index time series.
Memastikan urutan data berdasarkan waktu.
Memeriksa missing value dan konsistensi data.

2. Exploratory Data Analysis (EDA)

EDA dilakukan untuk memahami karakteristik data sebelum pemodelan.

Analisis yang dilakukan:

Visualisasi time series.
Analisis tren jangka panjang.
Seasonal decomposition.
Rolling Mean.
Rolling Standard Deviation.
Analisis perbandingan Februari dan Agustus.
Identifikasi dampak pandemi COVID-19 terhadap TPT.

3. Uji Stasioneritas

Pengujian menggunakan:

Augmented Dickey-Fuller Test (ADF)

Tujuan:

Menentukan apakah data sudah stasioner.
Menentukan kebutuhan differencing untuk model ARIMA.

4. Pemodelan Forecasting

Beberapa model yang digunakan:

Naive Forecast

Digunakan sebagai baseline model.

Asumsi:

Nilai periode berikutnya sama dengan nilai periode sebelumnya.
Holt's Linear Trend

Digunakan untuk menangkap tren jangka panjang pada data.

Karakteristik:

Cocok untuk data yang memiliki tren.
Tidak memodelkan seasonality secara eksplisit.
ETS (Error, Trend, Seasonality)

Digunakan untuk menguji pengaruh seasonality terhadap hasil forecasting.

ARIMA

Konfigurasi yang diuji:

ARIMA(1,1,1)
ARIMA(1,1,0)
ARIMA(0,1,1)
Evaluasi Model

Metrik evaluasi yang digunakan:

MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
MAPE (Mean Absolute Percentage Error)

Temuan Utama
Tren Jangka Panjang
TPT Jawa Tengah menunjukkan tren penurunan sejak tahun 2005.
Tingkat pengangguran menurun dari sekitar 9% menjadi sekitar 4% pada tahun 2026.
Dampak COVID-19
Terjadi lonjakan TPT yang signifikan pada tahun 2020.
Peningkatan ini sejalan dengan dampak pandemi COVID-19 terhadap pasar tenaga kerja.
Pemulihan Pasca Pandemi
Setelah tahun 2020, TPT kembali menunjukkan tren penurunan.
Hal ini mengindikasikan adanya pemulihan kondisi ketenagakerjaan.
Pola Semesteran
Secara umum TPT pada bulan Agustus cenderung lebih tinggi dibandingkan Februari.
Namun pengaruh pola semesteran relatif lebih kecil dibandingkan tren jangka panjang.
Hasil Forecasting

Model Holt dipilih sebagai model akhir karena:

Mampu menangkap tren penurunan TPT.
Memberikan hasil yang stabil dan mudah diinterpretasikan.
Memiliki performa yang kompetitif dibandingkan model lain yang diuji.

Hasil forecasting menunjukkan bahwa:

TPT diperkirakan terus menurun dalam beberapa tahun ke depan.
Pada tahun 2031, TPT diproyeksikan berada di sekitar 3,14%.

Catatan:

Forecast ini merupakan proyeksi berdasarkan pola historis dan tidak mempertimbangkan kejadian luar biasa seperti krisis ekonomi, pandemi, maupun perubahan kebijakan yang signifikan.

Tools dan Library

Library yang digunakan:

Pandas
NumPy
Matplotlib
Seaborn
Statsmodels
Scikit-Learn

Bahasa pemrograman:

Python

Kesimpulan

Analisis menunjukkan bahwa Tingkat Pengangguran Terbuka (TPT) Jawa Tengah memiliki tren penurunan dalam jangka panjang meskipun sempat mengalami kenaikan akibat pandemi COVID-19 pada tahun 2020. Berdasarkan hasil perbandingan beberapa model forecasting, model Holt dipilih sebagai model akhir dan menunjukkan bahwa TPT diperkirakan akan terus menurun hingga sekitar 3,14% pada tahun 2031 apabila tren historis tetap berlanjut.

Author

Dwi Julian Daffa
