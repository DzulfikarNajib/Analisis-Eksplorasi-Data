# Analisis Eksplorasi Data (AED) - Studi Kasus Susenas 2023
**Kelompok 5 AED** **Wilayah Analisis:** Kota Bandung (Kode Wilayah: 73)

## Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis karakteristik pengeluaran rumah tangga di Kota Bandung menggunakan data Susenas Maret 2023. Analisis difokuskan pada aspek statistik deskriptif untuk memahami distribusi kesejahteraan, pola konsumsi pangan, serta kesenjangan ekonomi berdasarkan kepemilikan aset (mobil).

## Metodologi
Analisis dilakukan dengan menggunakan bahasa pemrograman Python (Pandas & Numpy) dengan tahapan:
1. **Data Preprocessing:** Penggabungan (*merging*) data Blok 4.3 (Pengeluaran) dengan KOR Rumah Tangga (Karakteristik Fasilitas).
2. **Data Cleaning:** Konversi tipe data string ke numerik dan penanganan nilai hilang (*missing values*).
3. **Statistik Deskriptif:** Perhitungan Rata-rata, Simpangan Baku, Skewness, dan Kurtosis.

## Hasil Analisis Statistik

### 1. Total Pengeluaran Rumah Tangga per Bulan
Analisis ini mencakup total belanja rutin rumah tangga (makanan dan non-makanan).

| Indikator | Nilai | Interpretasi |
| :--- | :--- | :--- |
| **Rata-rata** | Rp 8.644.742 | Standar biaya hidup bulanan rumah tangga di wilayah target. |
| **Simpangan Baku** | Rp 9.218.992 | Variasi sangat tinggi, menunjukkan adanya disparitas ekonomi yang lebar. |
| **Skewness** | 5,04 | Distribusi miring ke kanan (Positif); mayoritas warga berada di bawah rata-rata. |
| **Kurtosis** | 44,05 | Distribusi sangat runcing (Leptokurtic) dengan banyak nilai pencilan (*outliers*). |

[Image of Positive Skewness Distribution]

### 2. Proporsi Pengeluaran Makanan (Hukum Engel)
Melihat persentase anggaran yang dialokasikan untuk kebutuhan pangan.

| Indikator | Nilai | Interpretasi |
| :--- | :--- | :--- |
| **Rata-rata** | 0,457 (45,7%) | Indikator kesejahteraan baik (Hukum Engel: pangan < 50%). |
| **Simpangan Baku** | 0,139 | Pola pembagian anggaran pangan cenderung homogen antar rumah tangga. |
| **Skewness** | -0,226 | Miring ke kiri; terdapat kelompok kecil dengan proporsi pangan sangat rendah. |
| **Kurtosis** | -0,373 | Distribusi landai; tidak ada penumpukan ekstrem pada satu nilai proporsi. |

### 3. Komparasi Berdasarkan Kepemilikan Mobil
Segmentasi rumah tangga berdasarkan kepemilikan aset kendaraan roda empat sebagai proksi kekayaan.

| Statistik | Memiliki Mobil | Tidak Memiliki Mobil |
| :--- | :--- | :--- |
| **Rata-rata Pengeluaran** | **Rp 19.206.930** | **Rp 6.602.268** |
| **Simpangan Baku** | Rp 16.116.560 | Rp 5.066.170 |
| **Skewness** | 3,27 | 3,47 |
| **Kurtosis** | 16,29 | 23,71 |

## Kesimpulan Utama
1. **Kesenjangan Ekonomi:** Terdapat jurang ekonomi yang signifikan, di mana rumah tangga pemilik mobil memiliki daya beli hampir **3 kali lipat** lebih tinggi dibandingkan non-pemilik mobil.
2. **Kesejahteraan Wilayah:** Berdasarkan Hukum Engel, wilayah ini dikategorikan sejahtera karena rata-rata pengeluaran pangan sudah berada di bawah 50% dari total anggaran bulanan.
3. **Distribusi Kekayaan:** Nilai Skewness dan Kurtosis yang ekstrem pada pengeluaran total menunjukkan bahwa distribusi kekayaan sangat terpusat pada kelompok elit kecil (pencilan).

---
*Dibuat untuk memenuhi Tugas 1 Mata Kuliah Analisis Eksplorasi Data.*
