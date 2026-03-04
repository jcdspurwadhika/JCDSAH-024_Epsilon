# JCDSAH-024_Epsilon

## Used Car Price Prediction
Project Used Car Price Prediction adalah sebuah project machine learning dimana model akan mempredeksi harga jual sebuah mobil bekas.

Goal utama dari project ini adalah memberikan sebuah prediksi harga mobil berdasarkan kriteria diantara lain Merk mobil, Milleage penggunaan mobil, dan Tahun pengeluaran/pembuatan mobil untuk mempermudah pengguna dalam menentukan harga yang kompetitif dengan cara membuat sebuah model machine learning yang akan mengestimasi harga berdasarkan spesifikasi kendaraan. Model ini dirancang sebagai sistem rekomendasi harga yang dapat diintegrasi ke dalam platform marketplace.

---
## Dataset
Dataset yang digunakan dalam project ini bisa diambil melalui link berikut >>> https://www.kaggle.com/datasets/turkibintalib/saudi-arabia-used-cars-dataset
Dataset berasal dari website penjualan mobil syarah.com.

Dataset mengandung attribute sebagai berikut 
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
---
## Streamlit Deployment
Setelah menjalankan notebook **Final Project - Price Prediction**, akan muncul file yang bernama **Used_cars_XGB.sav** yang merupakan model yang sudah tersimpan agar bisa digunakan oleh **app.py**.
### Cara untuk run streamlit di localhost
1. Install library yang dapat diperlukan (dapat dilihat dari **requirement.txt**)
2. Saat membukan **app.py**, masukan perintah berikut di console
```
streamlit run app.py
```

