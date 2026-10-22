# Identification, Elimination, Optimization: A Linear Programming and Machine Learning Approach for Rice Supply Chain Profit Maximization

Repositori ini berisi kode sumber dan analisis untuk studi penelitian operasional mengenai efisiensi rantai pasok beras di Jawa Barat, Indonesia. Proyek ini mengintegrasikan pendekatan **Data Envelopment Analysis (DEA)**, **Machine Learning**, dan **Pemrograman Linier (Linear Programming)** untuk mengidentifikasi inefisiensi, menganalisis faktor-faktor kerugian, serta memberikan rekomendasi optimalisasi laba berbasis data bagi seluruh aktor dalam rantai pasok.

## 🌾 Data Overview

Penelitian ini menggunakan data rantai pasok beras dari 5 kabupaten utama di Jawa Barat: **Garut, Subang, Karawang, Indramayu, dan Tasikmalaya**. Rantai pasok ini melibatkan 5 aktor utama dengan karakteristik operasional yang berbeda-beda:
1. **Petani (Farmers):** Biaya sewa lahan, tenaga kerja, benih, pupuk, pestisida, dan nilai produksi.
2. **Penggilingan (Millers):** Jumlah mesin, nilai gabah, jumlah beras giling, biaya tenaga kerja, dan pendapatan.
3. **Penebas / Tengkulak (Middlemen):** Pembelian beras, biaya sewa bangunan, susut penyusutan (shrinkage loss), dan nilai penjualan.
4. **Grosir (Wholesalers):** Pembelian beras, biaya operasional, dan nilai penjualan.
5. **Pengecer (Retailers):** Pembelian beras, biaya operasional, susut kualitas, dan nilai penjualan.

## 🛠️ Tech Stack & Libraries

Proyek ini dikembangkan menggunakan Python dengan pustaka analitik dan optimasi berikut:
* **Data Manipulation & Analysis:** `pandas`, `numpy`, `scipy`
* **Machine Learning & Modeling:** `scikit-learn`, `xgboost`, `catboost`
* **Optimization & Efficiency:** `pulp` (Linear Programming)
* **Explainable AI (XAI):** `shap`
* **Visualization:** `matplotlib`, `seaborn`

## 📂 Project Structure

```text
├── Data Raw/                  # Direktori data mentah (.xlsx)
│   ├── Farmer Data.xlsx
│   ├── Miller Data.xlsx
│   ├── Middlemen Data.xlsx
│   ├── Wholesale Data.xlsx
│   └── Retail Data.xlsx
├── README.md                  # Dokumentasi Proyek
└── main_analysis.ipynb        # Jupyter Notebook utama (EDA, DEA, ML, & Optimasi)
```

## 🚀 Key Features & Workflow

1. **Data Preprocessing & Validation:** Pemeriksaan *missing values*, duplikasi, serta standarisasi tipe data untuk setiap aktor rantai pasok.
2. **Data Envelopment Analysis (DEA):** Perhitungan skor efisiensi input-oriented untuk mengukur efisiensi teknis dan skala.
3. **Predictive Modeling & XAI:** Pelatihan model Machine Learning dan analisis SHAP untuk mengidentifikasi faktor utama penentu keuntungan.
4. **Linear Programming Optimization:** Pemodelan preskriptif untuk menentukan alokasi sumber daya optimal guna memaksimumkan laba.

## ⚙️ How to Run

1. Pastikan Anda telah menginstal pustaka Python yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost catboost pulp scipy openpyxl shap
   ```
2. Letakkan file dataset mentah ke dalam folder `Data Raw/` sesuai struktur di atas.
3. Buka dan jalankan `main_analysis.ipynb` untuk mereproduksi hasil analisis.
