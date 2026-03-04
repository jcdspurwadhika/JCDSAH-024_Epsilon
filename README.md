# JCDSAH-024_Epsilon

## Used Car Price Prediction
Project Used Car Price Prediction adalah sebuah project machine learning dimana model akan mempredeksi harga jual sebuah mobil bekas.

Goal utama dari project ini adalah memberikan sebuah prediksi harga mobil berdasarkan kriteria diantara lain Merk mobil, Milleage penggunaan mobil, dan Tahun pengeluaran/pembuatan mobil untuk mempermudah pengguna dalam menentukan harga yang kompetitif dengan cara membuat sebuah model machine learning yang akan mengestimasi harga berdasarkan spesifikasi kendaraan. Model ini dirancang sebagai sistem rekomendasi harga yang dapat diintegrasi ke dalam platform marketplace.

[Streamlit](https://used-cars-machine-learning-deployment-nn856zy4htkrhxgzpznoga.streamlit.app/)

---
## Project Flow
### Dataset
Dataset yang digunakan dalam project ini bisa diambil melalui link berikut (https://www.kaggle.com/datasets/turkibintalib/saudi-arabia-used-cars-dataset)

Dataset berasal dari website penjualan mobil syarah.com, dimana dataset merupakan listing mobil bekas yang dijual di website syarah.

Dataset sebelum cleaning berisi 8248 row dengan attribute sebagai berikut
| **Attribute** | **Data Type** | **Description**                                       |
| ------------- | ------------- | ----------------------------------------------------- |
| Link          | Object        | Link iklan mobil                                      |
| Make          | Object        | Merek mobil                                           |
| Type          | Object        | Tipe atau model mobil                                 |
| Year          | Integer       | Tahun produksi mobil                                  |
| Origin        | Object        | Negara asal kendaraan                                 |
| Color         | Object        | Warna mobil                                           |
| Options       | Object        | Tingkat kelengkapan fitur (Standard, Semi Full, Full) |
| Engine_Size   | Float         | Kapasitas mesin dalam liter                           |
| Fuel_Type     | Object        | Jenis bahan bakar                                     |
| Gear_Type     | Object        | Jenis transmisi (Manual / Automatic)                  |
| Condition     | Object        | Kondisi kendaraan (New / Used)                        |
| Mileage       | Integer       | Jarak tempuh kendaraan (km)                           |
| Region        | Object        | Wilayah tempat mobil dijual                           |
| Price         | Object        | Harga jual mobil dalam SAR                            |
| Negotiable    | Boolean       | Status apakah harga dapat dinegosiasikan              |

### Models
Beberapa model yang digunakan dalam project ini:
- Linear Regression
- KNN Regression
- Decision Tree Regression
- Random Forest Regression
- Extreme Gradient Boost (XGB)

Model Dievaluasi dengan metric berikut
- Root Mean Square Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- R-Square $$(R^2)$$

Metric RMSE menjadi metric acuan dalam menilai performa model karena digunakan untuk melihat error prediksi harga yang dilakukan oleh model.

### Output dari Project
Output dari project ini adalah model regresi yang di implementasi menggunakan Streamlit. Output dari modelling model XGBoost yang telah dilakukan tuning menggunakan RandomSearch dengan metric akhir sebagai berikut.

| **RMSE**      | **MAE**       | **MAPE**      | **MAPE**      |
| ------------- | ------------- | --------------| --------------|
| 36546.576091  | 13502.975586  | 	0.169580	  | 	0.817393    |

---
## Tableau Dashboard
https://public.tableau.com/app/profile/rivaldo.nugradwiyanto/viz/SyarahSaudiUsedCarPriceAnalysis/Dashboard1?publish=yes

---
## Streamlit Page
https://used-cars-machine-learning-deployment-nn856zy4htkrhxgzpznoga.streamlit.app/

Aplikasi Streamlit merupakan implementasi model Used Car Predictor. Streamlit dapat digunakan oleh penjual mobil untuk mencari estimasi harga mobil yang akan dijual. Aplikasi ini juga dapat digunakan oleh pembeli untuk melihat estimasi harga mobil yang akan dibeli.

Cara penggunaan Streamlit Used Car Predictor adalah sebagai berikut:
- Masukan kriteria mobil menggunakan dropdown menu, slider, dan manual input.
- Setelah kriteria mobil sudah sesuai, Klik tombol **Predict Price**.
- Streamlit akan menunjukan return estimasi harga dan range kemungkinan variasi harga.

---
## Streamlit Deployment
Setelah menjalankan notebook **Final Project - Price Prediction**, akan muncul file yang bernama **Used_cars_XGB.sav** yang merupakan model yang sudah tersimpan agar bisa digunakan oleh **app.py**.
### Cara untuk run streamlit di localhost
1. Install library yang diperlukan (dapat dilihat dari **requirement.txt**)
2. Saat membukan **app.py**, masukan perintah berikut di console
```
streamlit run app.py
```
---
