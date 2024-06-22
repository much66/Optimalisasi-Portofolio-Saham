# Optimalisasi-Portofolio-Saham

**Dataset** : [source](https://www.kaggle.com/competitions/home-data-for-ml-course/data) <br>
**Notebook** : [view](https://github.com/much66/Optimalisasi-Portofolio-Saham/blob/main/Banking_Stock_Forecasting.ipynb)<br>
**Deck** : [view](https://github.com/much66/Optimalisasi-Portofolio-Saham/blob/main/Deck%20Presentasi.pdf)<br>

<br>

**Table of Contents**
- [Business Understanding]()
- [Workflow]()
- [Insight]()
- [Modeling and Evaluation]()
<br>


## 📂 Business Understanding
### Problem Statement
Perusahaan Hedge Fund dan Reksa Dana menghadapi tantangan dalam mengelola portofolio investasi mereka di tengah volatilitas pasar yang tinggi. Volatilitas ini dapat mengakibatkan risiko kerugian yang signifikan bagi perusahaan dan investor mereka. Oleh karena itu, perusahaan memerlukan solusi untuk memprediksi pergerakan harga saham, menghitung risiko dengan Value at Risk (VaR) dan Volatilitas, serta mengoptimalkan portofolio investasi untuk meminimalkan risiko dan memaksimalkan return.

### Goals
- Meminimalkan Risiko: Mengidentifikasi dan meminimalkan risiko kerugian yang terkait dengan volatilitas pasar dalam portofolio Hedge Fund dan Reksa Dana.
- Memaksimalkan Return: Mengoptimalkan portofolio investasi untuk mencapai return yang optimal sambil mempertahankan risiko pada level yang dapat diterima.
  
### Objectives
- Membuat Prediksi Harga Saham: Mengembangkan model prediksi menggunakan Prophet untuk memprediksi harga saham perusahaan Hedge Fund dan Reksa Dana.
- Menghitung VaR dan Volatilitas: Menggunakan hasil prediksi untuk menghitung Value at Risk (VaR) dan Volatilitas portofolio investasi.
- Optimasi Portofolio: Mengidentifikasi komposisi portofolio optimal dengan VaR dan Volatilitas terendah untuk meminimalkan risiko dan memaksimalkan return.

<br>


## 📂 Workflow
<p align="center">
    <kbd> <img width="1000" alt="workflow" src="Workflow Forecasting.png"> </kbd> <br>
    Gambar 1 — Workflow Pembuatan Model
</p>
<br>

## 📂 Insight
- Tingkat default kredit nasabah dari dataset mencapai 9%
- Karakteristik mayoritas nasabah yang cenderung mengalami masalah dalam pembayaran kredit yaitu:
  - Laki-laki
  - Kelompok pendidikan rendah, "lower secondary"
  - Rentang usia 25 - 40 tahun
  - Lama bekerja 1 - 5 tahun
  - Tipe kredit "Cash Loan"
<br>

## 📂 Modeling and Evaluation
- Split dataset dengan rasio 80% Train : 20% Test
- Mengatasi data Train yang tidak seimbang menggunakan RandomUnderSampler
- Scaling data dengan RobustScaler
- Eksperimen menggunakan beberapa algoritma Logistic Regression, Random Forest, dan XGBoost
- Best fit model didapatkan menggunakan Logistic Regression dengan hyperparameter tuning, menghasilkan akurasi 87% dan AUC 73%

<br>
<p align="center">
    <kbd> <img width="800" alt="feats" src="#"> </kbd> <br>
    Gambar 2 — Feature Importance
</p>
<br>


## 📂 Recommendations
- Mempertimbangkan untuk membuat Credit Scorecard, menggunakan Information Value dan Feature Engineering menggunakan Weight of Evidence
- Melakukan analisis kredit yang lebih mendalam 
- Meningkatkan seleksi calon peminjam dengan memperketat persyaratan dan mengumpulkan informasi yang lebih lengkap tentang calon peminjam
