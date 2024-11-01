# Proyek Clustering dan Classification Menggunakan Dataset Adult Income

**Dataset**: [Adult Income Dataset](https://archive.ics.uci.edu/dataset/2/adult)

Ini adalah proyek sederhana untuk melakukan clustering, kemudian hasil clustering tersebut digunakan untuk classification.

## Clustering

### Langkah-langkah
1. **Import Library**
2. **Memuat Dataset**
3. **Explanatory Data Analysis (EDA)**
   - Memeriksa Info Dataset (Jumlah Kolom, Baris, Fitur Numerik & Kategorikal)
   - Cek Missing Values, Duplicates, dan Penanganan
   - Analisis Statistik Distribusi dan Korelasi pada Data
4. **Data Preprocessing**
   - Cek dan Menangani Outliers pada Data
   - Encoding Data Kategorikal
   - Feature Standardization
   - Menggabungkan Train dan Test Sets ke dalam Satu DataFrame
5. **Pembangunan Model Clustering**
   - Menggunakan algoritma k-means
6. **Evaluasi Model Clustering**
   - Mencari optimal K (cluster) menggunakan elbow method
   - Mencari Optimal K (Cluster) Menggunakan Silhouette Score
7. **Feature Selection**
   - Memilih lima fitur dengan korelasi tertinggi dengan fitur income
   - Mencari Optimal K (Cluster) Menggunakan Silhouette Score dengan fitur yang telah dipilih
8. **Visualisasi Hasil Clustering**
   - Visualisasi dengan 2D PCA Projection
9. **Analisis dan Interpretasi Hasil Cluster**
   - Interpretasi dengan melihat nilai statistik deskriptif tiap cluster.
10. **Export Data Clustering**

Keseluruhan proses dapat dilihat disini: [Adult Income Clustering](https://github.com/Maoelan/adult-income-clustering-classification/blob/main/%5BClustering%5D%20Submission%20Akhir%20BMLP_Maulana%20Muhammad.ipynb)

Pada clustering ini, Silhouette Score akhir yang didapat adalah **0.71** dengan K (cluster) optimal **4**.

## Classification

### Langkah-langkah
1. **Import Library**
2. **Load Dataset Hasil Clustering**
3. **Data Splitting**
4. **Membangun Model**
   - Menggunakan 5 algoritma yaitu:
     - K-Nearest Neighbors
     - Ridge Classifier
     - Perceptron
     - Multinomial Naive Bayes
     - Logistic Regression
5. **Tuning Model**
6. **Analisis Hasil Evaluasi**

Keseluruhan proses dapat dilihat disini: [Adult Income Classification](https://github.com/Maoelan/adult-income-clustering-classification/blob/main/%5BKlasifikasi%5D_Submission_Akhir_BMLP_Maulana%20Muhammad.ipynb)

### Hasil Klasifikasi Sebelum dan Sesudah Tuning Model
| Model                                   | Total Accuracy | Weighted F1 Score | Precision | Recall |
|-----------------------------------------|----------------|--------------------|-----------|--------|
| K-Nearest Neighbors (Sebelum)          | 0.9455         | 0.9284             | 0.9296    | 0.9304 |
| K-Nearest Neighbors (Setelah)          | 0.9476         | 0.9464             | 0.9470    | 0.9476 |
| Ridge Classifier (Sebelum)             | 0.9805         | 0.9695             | 0.9601    | 0.9794 |
| Ridge Classifier (Setelah)             | 0.9794         | 0.9695             | 0.9601    | 0.9794 |
| Perceptron (Sebelum)                   | 0.9797         | 0.9698             | 0.9633    | 0.9785 |
| Perceptron (Setelah)                   | 0.9785         | 0.9698             | 0.9633    | 0.9785 |
| Multinomial Naive Bayes (Sebelum)     | 0.8821         | 0.8738             | 0.8997    | 0.8818 |
| Multinomial Naive Bayes (Setelah)     | 0.8818         | 0.8738             | 0.8997    | 0.8818 |
| Logistic Regression (Sebelum)          | 0.9853         | 0.9808             | 0.9857    | 0.9843 |
| Logistic Regression (Setelah)          | 1.0000         | 1.0000             | 1.0000    | 1.0000 |
