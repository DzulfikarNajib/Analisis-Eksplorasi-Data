# Analisis Eksplorasi Data (Exploratory Data Analysis)

[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()
[![Course](https://img.shields.io/badge/Course-IPB--University-green.svg)]()

## Deskripsi Mata Kuliah
Repositori ini berisi implementasi dari mata kuliah **Analisis Eksplorasi Data (STA1232)**. Berbeda dengan analisis klasik yang langsung masuk ke pemodelan, di sini saya belajar untuk membiarkan "data yang berbicara" melalui identifikasi struktur, pola, dan anomali menggunakan teknik visual dan statistik yang fleksibel.

---

## Apa yang Saya Pelajari? (Based on Syllabus)

### 1. Statistika Deskriptif & Bentuk Sebaran
Bukan sekadar rata-rata, saya mendalami karakteristik bentuk data:
* **Pemusatan & Penyebaran:** Mean, Median, Modus, Quartile, dan Standard Deviation.
* **Bentuk Sebaran:** Menganalisis kemiringan (**Skewness**) dan keruncingan kurva (**Kurtosis**) menggunakan metode Karl Pearson dan Bowley.
* **Klasifikasi Kurtosis:** Membedakan data bersifat *Leptokurtik*, *Platikurtik*, atau *Mesokurtik*.

### 2. Visualisasi Sebaran Univariat
Teknik visualisasi untuk memahami distribusi satu variabel:
* **Histogram & Boxplot:** Alat utama untuk melihat sebaran dan mendeteksi anomali.
* **Kernel Density Estimation (KDE):** Menggunakan fungsi kernel dan pemilihan *bandwidth* ($h$) yang tepat untuk memuluskan kurva distribusi data kontinyu.

### 3. Pemeriksaan Sebaran Data (Normality Test)
Prosedur formal untuk mengecek apakah data mengikuti distribusi tertentu (terutama Normal):
* **QQ-Plot (Quantile-Quantile Plot):** Membandingkan kuantil data amatan dengan kuantil teoritis.
* **Uji Formal:** Menggunakan uji Kolmogorov-Smirnov, Shapiro-Wilk, dan Anderson-Darling.

### 4. Pendeteksian Pencilan (Outlier Detection)
Mempelajari berbagai jenis pencilan (Global, Kontekstual, dan Kolektif) menggunakan:
* **Metode Klasik:** Z-Score dan Interquartile Range (IQR).
* **Metode Robust:** Median Absolute Deviation (MAD) dan Schwertman’s Fence.

### 5. Statistika Kekar (Robust Statistics)
Mempelajari metode pendugaan parameter yang tidak sensitif terhadap *outlier*:
* **Penduga Lokasi Robust:** *Trimmed Mean* (rata-rata terpangkas) dan *Winsorized Mean*.
* **Pentingnya Robustness:** Memahami bahwa metode klasik bisa sangat bias jika data mengandung pencilan yang ekstrem.

---

## Tools & Libraries
* **Language:** Python / R (Tidyverse/ggplot2)
* **Key Libraries:** NumPy, Pandas, Scipy.stats, Matplotlib, Seaborn.

---

## Key Takeaway
"Pendekatan eksplorasi mendahulukan data sebelum model. Tujuannya adalah memastikan struktur data dipahami dengan benar agar kesimpulan yang diambil tidak menyesatkan akibat adanya pencilan atau pelanggaran asumsi distribusi."
