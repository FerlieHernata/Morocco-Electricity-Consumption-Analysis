# Data Analytics Final Project - Morocco Electricity Consumption Analysis

Proyek ini menganalisis konsumsi listrik di Maroko pada tahun 2017 menggunakan dataset dari Maven Analytics.  
Analisis dilakukan dengan **Python (Jupyter Notebook)** untuk data preprocessing & eksplorasi, serta **Power BI** untuk visualisasi interaktif.  
Laporan akhir disusun untuk menjelaskan metodologi, hasil, dan insight utama.

## Dataset
- Sumber: Maven Analytics (UCI Machine Learning Repository)  
- Periode: Tahun 2017  
- Jumlah data: 61.755 baris dengan 9 atribut  
- Atribut utama:  
  - Datetime (pencatatan tiap 10 menit)  
  - Temperature, Humidity, WindSpeed  
  - PowerConsumption_Zone1  
  - PowerConsumption_Zone2  
  - PowerConsumption_Zone3  


## Analisis
Dilakukan dengan Python pada Google Colab (lihat `analysis.ipynb`):  
- **Data Preprocessing**: konversi datetime, handling missing values, tetap mempertahankan outlier karena relevan.  
- **Basic Statistics**: mean, median, max, min, boxplot.  
- **Korelasi**: Pearson correlation antara faktor lingkungan (suhu, kelembaban, angin) dan konsumsi listrik.  
- **Regression**: simple linear regression suhu terhadap konsumsi listrik.  
- **Time Series**: pola harian, mingguan, dan musiman.  

## Dashboard Power BI
File Power BI: `morocco-consumption.pbix`  

## Insight Utama
- **Zona 1** → konsumsi listrik tertinggi dan stabil (median ~32.265 watt), kemungkinan area industri/komersial.  
- **Zona 2** → tingkat menengah (~20.823 watt), lebih fluktuatif, indikasi semi-komersial/campuran.  
- **Zona 3** → terendah (~16.415 watt) dengan banyak outlier, menunjukkan karakter residensial.  
- **Faktor Lingkungan**:  
  - Suhu → faktor paling dominan (semakin tinggi suhu, konsumsi meningkat).  
  - Kelembaban → pengaruh negatif lemah.  
  - Kecepatan angin → pengaruh sangat kecil.  
- **Pola Harian** → dua puncak konsumsi: siang (~13.00) & malam (~20.00).  
- **Pola Mingguan** → konsumsi menurun pada hari Minggu, terutama di Zona 1 & 2.  
- **Pola Musiman** → puncak konsumsi di musim panas (Juli–Agustus), terendah di musim dingin/awal musim semi.  

## Anggota
- Josh Nicholas Sutanto - 2702234825  
- Ferlie Hernata - 2702231262  
- Giovincent Ricel's Tanoto - 2702226786  
- Nikolaus Marvin Liayasa - 2702233702  
- Rendy Riady - 2702234421  
- Rasxelz Cornelius Khu - 2702237316  

