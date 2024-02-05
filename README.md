# Analisa Tren dan Pola Belanja di Istanbul Tahun 2021-2022

Tool : Jupyter Notebook <br>
Programming Language : Python <br>
Visualization : Matplotlib, Seaborn, Looker Data Studio <br>
Dataset : [Lihat Disini](https://www.kaggle.com/datasets/mehmettahiraslan/customer-shopping-dataset/data)

---

## Introduction
Project ini merupakan final project dari program pelatihan PROA yang diselenggarakan oleh Digitalent KOMINFO bekerjasama dengan Cisco sebagai bentuk pengaplikasian bahasa pemrograman Python di dalam Big Data. Pada project ini saya berperan sebagai Data Analyst yang melakukan analisa tren dan pola belanja di Istanbul.

## Objective
Memberikan insight terhadap tren dan pola belanja di Mall yang ada di Istanbul.

---

## Overview
Dataset terdiri dari 99457 baris dan 10 kolom.
<p align="center">
   <img src="picture/Picture1.png" width = 400 px>
</p>

## Data Cleaning
1. Tidak ditemukan data kosong.
2. Tidak ditemukan data duplikat.
   
## Data Preprocessing
### Feature Engineering
1. Membuat feature baru yaitu `total_payment`
2. Mengurai kolom `invoice_date` menjadi hari, bulan, dan tahun.
3. Membuat feature baru yaitu `age_category`.

### Merubah Tipe Data
1. `invoice_date` menjadi datetime
2. `month` menjadi object
3. `year` menjadi object

### Menghapus Data yang Tidak Diperlukan
Feature yang tidak digunakan dan di drop adalah `customer_id`.

### Filter Data
Dataset yang diberikan adalah dari tahun 2021-2023, namun karena pada tahun 2023 data tidak lengkap (hanya sampai bulan Maret), maka diputuskan untuk menggunakan data tahun 2021-2022.

---

## Analysis
### 1. Persebaran Harga dan Total Pembelanjaan Customer di Mall

<p align="center">
   <img src="picture/picture2.png" width = 400 px> <img src="picture/picture3.png" width = 400 px>
</p>

### 2. Transaksi per Bulan Berdasarkan Category 

<p align="center">
   <img src="picture/output6.png" width = 400 px> 
</p>

Di setiap bulannya, categori yang paling banyak transaksinya adalah **clothing**. Bulan Juli, transaksi clothing merupakan transaksi tertinggi dibandingkan dengan bulan lainnya. Hal ini mungkin dikarenakan bulan Juli merupakan puncak musim panas di Istanbul, dimana sehingga ada kemungkinan masyarakat cenderung sering berganti pakaian.
