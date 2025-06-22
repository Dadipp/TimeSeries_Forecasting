# 📈 Time Series Forecasting - Daily Sales & Orders

Repository ini berisi analisis dan pemodelan time series untuk memprediksi penjualan harian (`daily_sales`) dan jumlah pesanan harian (`daily_order_count`) berdasarkan data historis.

## 📊 Tahapan Analisis

### 1. Eksplorasi Data
Melakukan eksplorasi awal untuk memahami struktur dan karakteristik data time series.

### 2. Pembersihan Data
Tahapan ini meliputi penanganan data kosong, penggabungan kolom waktu, serta konversi format waktu.

### 3. Agregasi Data Harian
Data dikonsolidasikan ke dalam format harian untuk memudahkan analisis tren dan peramalan.

### 4. Analisis Tren dan Pola
Visualisasi `daily_sales` dari tahun 2014–2017 menunjukkan pola yang sangat fluktuatif tanpa tren yang konsisten. Terdapat banyak lonjakan penjualan yang diduga berasal dari:
- Promosi besar-besaran
- Event khusus atau hari libur
- Pembelian massal
- Outlier atau anomali data

Polanya sangat tidak beraturan sehingga memerlukan pendekatan lanjutan seperti dekomposisi time series atau model prediktif berbasis machine learning.

## 📦 Model yang Digunakan

Model-model berikut digunakan untuk memprediksi `daily_sales` dan `daily_order_count`:
- **Naive Forecasting**
- **Holt-Winters Exponential Smoothing**
- **SARIMA**
- **Prophet**
- **LightGBM**
- **XGBoost**

## 📈 Evaluasi Model

Setiap model dievaluasi menggunakan metrik:
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **MAPE** (Mean Absolute Percentage Error)

Model terbaik dalam studi ini adalah **XGBoost** dan **Tuned LightGBM**, terutama dalam memprediksi `daily_order_count` dengan akurasi tinggi dan MAPE terendah.
