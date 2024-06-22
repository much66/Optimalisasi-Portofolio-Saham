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
- Prediksi harga setiap saham 7 periode mendatang
- Maksimal kerugian setiap saham
- Kestabilan harga setiap saham
- Rekomendasi saham berdasarkan Volatility dan VaR Terkecil
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
    Gambar 2 — Perbandingan model
</p>
<br>


## 📂 Recommendations
- Penggunaan Metode Prophet dan Simulasi Monte Carlo: Gunakan Prophet untuk prediksi harga saham dan Simulasi Monte Carlo untuk memperkirakan skenario pergerakan harga di masa depan, memahami risiko dan return dengan lebih baik.
- Portofolio Jangka Pendek: Fokuskan investasi pada jangka pendek (1-3 bulan) untuk responsif terhadap perubahan pasar, monitor kinerja secara berkala, dan sesuaikan portofolio dengan analisis risiko terkini.
- Diversifikasi Saham dengan Volatilitas dan VaR Terendah: Diversifikasikan portofolio dengan saham berisiko rendah, prioritaskan kestabilan harga dan minimalkan potensi kerugian, sehingga portofolio tetap terlindungi dari fluktuasi ekstrem dan memberikan return yang stabil.
