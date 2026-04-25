# Mall Customer Segmentation Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)](https://scikit-learn.org/)
[![Visualization](https://img.shields.io/badge/Viz-Plotly%20%7C%20Seaborn-green.svg)](https://plotly.com/)

Project ini merupakan analisis segmentasi pelanggan menggunakan teknik **Unsupervised Learning** (K-Means Clustering). Analisis ini bertujuan untuk mengidentifikasi profil pelanggan di sebuah pusat perbelanjaan (mall) berdasarkan perilaku belanja dan pendapatan tahunan untuk mendukung strategi pemasaran yang lebih presisi.

## Fitur Utama
- **Advanced EDA**: Analisis distribusi usia dengan *Skewness* dan *Kernel Density Estimate* (KDE).
- **Statistical Validation**: Penentuan jumlah cluster optimal menggunakan **Elbow Method** dan **Silhouette Score**.
- **Interactive Visualization**: Visualisasi data multivariate 3D menggunakan Plotly untuk pemahaman spasial cluster yang lebih baik.
- **Actionable Insights**: Rekomendasi strategi bisnis konkret untuk setiap segmen pelanggan yang ditemukan.

## Struktur Dataset
Dataset yang digunakan adalah `Mall_Customers.csv` yang mencakup fitur:
- `Gender`: Jenis kelamin pelanggan.
- `Age`: Usia pelanggan.
- `Annual Income (k$)`: Pendapatan tahunan dalam ribuan dollar.
- `Spending Score (1-100)` : Skor perilaku belanja yang ditetapkan oleh pihak mall.

## Metodologi Analisis
1. **Data Pre-processing**:
   - Menghapus fitur non-informatif (`CustomerID`).
   - Transformasi fitur kategorikal menggunakan `LabelEncoder`.
2. **Exploratory Data Analysis (EDA)**:
   - Visualisasi korelasi Pearson.
   - Analisis distribusi demografis.
3. **Clustering**:
   - Algoritma: K-Means Clustering.
   - Optimasi: Inisialisasi `k-means++`.
   - Validasi: Perhitungan *Within-Cluster Sum of Squares* (WCSS) dan *Silhouette Coefficient*.

## Hasil Segmentasi
Berdasarkan analisis, pelanggan dibagi menjadi 5 cluster utama:
1. **Cluster Target**: Pendapatan tinggi & pengeluaran tinggi.
2. **Cluster Konservatif**: Pendapatan tinggi & pengeluaran rendah.
3. **Cluster Moderat**: Pendapatan & pengeluaran menengah.
4. **Cluster Impulsif**: Pendapatan rendah & pengeluaran tinggi.
5. **Cluster Hemat**: Pendapatan rendah & pengeluaran rendah.

## Cara Menjalankan
1. Clone repository ini:
   ```bash
   git clone: https://github.com/Zahrah-FA/KMeans-Clustering-Optimization-MallData.git
