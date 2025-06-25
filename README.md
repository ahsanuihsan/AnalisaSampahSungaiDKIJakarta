# 🌊 Analisis Interaktif Volume Sampah Sungai DKI Jakarta 🌿

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-orange.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellow.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)

Selamat datang di proyek analisis lingkungan interaktif! 🚀 Proyek ini menggunakan **Jupyter Notebook** untuk menganalisis **volume sampah sungai** di DKI Jakarta berdasarkan dataset `RataRataVolumeSampahSungaiDKIJakarta.csv`. Dengan visualisasi **Plotly**, Anda dapat menjelajahi data dari Januari hingga Mei 2025 dengan fitur seperti *hover*, *zoom*, dan *filter*. Ideal untuk peneliti, penggiat lingkungan, atau siapa saja yang peduli dengan isu sampah! 🌏

## 📋 Deskripsi Proyek
Proyek ini menganalisis data volume sampah sungai di DKI Jakarta menggunakan **Python** dalam file Jupyter Notebook `analisis_sampah_jakarta_interaktif.ipynb`. Library **Pandas** digunakan untuk pengolahan data, dan **Plotly** untuk visualisasi interaktif. Tujuannya adalah memberikan wawasan tentang pola, distribusi, dan hubungan volume sampah di kecamatan dan wilayah administratif Jakarta.

**Fitur Interaktif**:
- 🖱️ *Hover* untuk melihat detail data.
- 🔍 *Zoom* dan *pan* untuk eksplorasi visual.
- 🎚️ *Toggle* legenda untuk memfilter data.
- 📥 Ekspor plot sebagai PNG atau HTML.

## 📊 Struktur Dataset
Dataset `RataRataVolumeSampahSungaiDKIJakarta.csv` berisi:
| Kolom                | Deskripsi                                                                 |
|----------------------|---------------------------------------------------------------------------|
| `periode_data`       | Periode pengumpulan data (format: YYYYMM, e.g., 202401 untuk Januari 2024) |
| `wilayah`            | Wilayah administratif (e.g., KOTA ADM. JAKARTA PUSAT)                     |
| `kecamatan`          | Nama kecamatan di wilayah tersebut                                       |
| `volume_sampah`      | Total volume sampah yang dikumpulkan (ton)                               |
| `total_sampah_residu`| Total sampah residu setelah pengelolaan (ton)                            |
| `rata_rata`          | Rata-rata volume sampah per hari dalam periode tersebut (ton)            |

## 🔍 Daftar Analisis
Notebook `analisis_sampah_jakarta_interaktif.ipynb` mencakup lima analisis berikut:

| No | Analisis                              | Deskripsi                                                                 | Output Interaktif                                                                 |
|----|---------------------------------------|---------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| 1  | **Tren Volume Sampah per Wilayah**    | Tren rata-rata volume sampah per wilayah (Jan-Mei 2025)                  | Line plot dengan hover dan toggle wilayah                                         |
| 2  | **Top 5 Kecamatan Volume Tertinggi**  | 5 kecamatan dengan volume sampah tertinggi per periode                    | Bar plot dengan tooltip dan filter periode                                        |
| 3  | **Perbandingan Antar Wilayah**        | Distribusi volume sampah antar wilayah                                   | Box plot dengan tooltip untuk statistik                                          |
| 4  | **Korelasi Volume dan Residu**        | Hubungan antara volume sampah dan sampah residu                          | Scatter plot dengan garis regresi dan hover                                       |
| 5  | **Pola Musiman Jagakarsa**            | Fluktuasi volume sampah di kecamatan Jagakarsa                           | Line plot dengan tooltip untuk detail periode                                    |

> **Catatan**: Untuk menyimpan visualisasi interaktif, gunakan `fig.write_html('nama_file.html')` di notebook atau klik ikon kamera di toolbar Plotly untuk PNG.

## 📂 Struktur File
- `RataRataVolumeSampahSungaiDKIJakarta.csv`: Dataset utama.
- `analisis_sampah_jakarta_interaktif.ipynb`: Jupyter Notebook dengan semua analisis interaktif.

## 🚀 Cara Menjalankan
1. **Prasyarat** 📦
   - Instal Python 3.8+.
   - Instal dependensi:
     ```bash
     pip install pandas plotly jupyter
     ```
   - Pastikan Jupyter Notebook terinstal.

2. **Langkah-langkah** 🛠️
   - Simpan `RataRataVolumeSampahSungaiDKIJakarta.csv` di direktori yang sama dengan `analisis_sampah_jakarta_interaktif.ipynb`.
   - Buka Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Buka `analisis_sampah_jakarta_interaktif.ipynb` dan jalankan sel satu per satu.
   - **Interaksi**:
     - 🖱️ *Hover* untuk detail data.
     - 🔍 *Zoom* dengan klik dan drag.
     - 🎚️ *Toggle* legenda untuk filter data.
     - 📥 Klik ikon kamera untuk menyimpan plot.

3. **Tips** 💡
   - Pastikan path dataset di sel `pd.read_csv()` sesuai.
   - Gunakan VS Code dengan ekstensi Jupyter untuk pengalaman lebih lancar.
   - Ekspor plot ke HTML untuk berbagi: `fig.write_html('nama_file.html')`.

## 🛠️ Dependensi
- Python 3.8+
- Pandas 🐼
- Plotly 📈
- Jupyter Notebook 📒

## 📈 Contoh Output
- **Tren Volume Sampah**: Line plot dengan garis per wilayah, hover untuk nilai rata-rata, toggle wilayah.
- **Top Kecamatan**: Bar plot dengan tooltip untuk kecamatan dan volume.
- **Perbandingan Wilayah**: Box plot dengan tooltip untuk median, kuartil, outlier.
- **Korelasi**: Scatter plot dengan garis regresi, hover untuk nilai data.
- **Pola Musiman Jagakarsa**: Line plot dengan tooltip untuk volume per periode.

> **Lihat demo**: Tambahkan `fig.write_html()` untuk menyimpan plot dan unggah ke GitHub untuk akses publik.

## 📝 Struktur Notebook
`analisis_sampah_jakarta_interaktif.ipynb` terdiri dari:
1. **Sel Markdown**: Penjelasan proyek dan dataset.
2. **Sel Kode**: Import library, pemuatan dataset, pembersihan data.
3. **Sel Analisis**: Lima query analisis dengan visualisasi Plotly, dipisahkan oleh markdown.

## 📊 Kesimpulan dan Rekomendasi
Berdasarkan analisis dataset dari Januari hingga Mei 2025, berikut adalah temuan utama dan rekomendasi:

### Kesimpulan
1. **Hotspot Sampah Sungai** 🌊:
   - **Kecamatan**: Jagakarsa (Jakarta Selatan), Penjaringan (Jakarta Utara), Cengkareng (Jakarta Barat), dan Cakung (Jakarta Timur) adalah penyumbang utama volume sampah, dengan Jagakarsa mencatat puncak 220 ton/hari pada Februari 2024.
   - **Wilayah**: Jakarta Selatan dan Utara memiliki volume tertinggi dengan distribusi tidak merata, ditandai oleh outlier signifikan seperti Jagakarsa dan Penjaringan.

2. **Pola Musiman** 📅:
   - Volume sampah melonjak pada Februari-Maret (misalnya, Jagakarsa: 220 ton/hari pada Februari 2024, 130.16 ton/hari pada Maret 2025), kemungkinan karena musim hujan meningkatkan aliran sampah ke sungai.
   - Penurunan terjadi pada April-Mei, menunjukkan potensi musim kemarau atau efektivitas pembersihan.

3. **Efisiensi Pengelolaan Sampah** 🗑️:
   - Korelasi tinggi (~0.95) antara volume sampah dan residu menunjukkan inefisiensi pengelolaan, dengan ~95-98% sampah menjadi residu tanpa daur ulang signifikan.
   - Kecamatan seperti Jagakarsa dan Penjaringan menghasilkan residu besar, menandakan kurangnya pengolahan efektif.

4. **Variasi Antar Wilayah** 📍:
   - Jakarta Selatan dan Utara memiliki variansi besar dengan outlier ekstrem, menunjukkan tantangan pengelolaan di kecamatan tertentu.
   - Jakarta Pusat memiliki volume rendah (~18 ton/hari) dan distribusi seragam, menandakan pengelolaan yang lebih terkendali.

5. **Manfaat Visualisasi Interaktif** 📈:
   - Plotly memungkinkan identifikasi cepat hotspot, pola musiman, dan inefisiensi melalui fitur *hover*, *zoom*, dan *toggle* legenda.

### Rekomendasi
1. **Prioritaskan Hotspot** 🔧:
   - Fokuskan pembersihan sungai, fasilitas pengumpulan sampah, dan edukasi di Jagakarsa, Penjaringan, Cengkareng, dan Cakung.
   - Investigasi penyebab volume ekstrem di Jagakarsa (misalnya, saluran sungai atau pembuangan ilegal).

2. **Pengelolaan Musiman** ⛈️:
   - Tingkatkan pembersihan dan kampanye pengurangan sampah sebelum Februari-Maret, terutama di Jakarta Selatan dan Utara.
   - Pasang penyaring sampah di sungai Jagakarsa untuk menangani lonjakan musiman.

3. **Tingkatkan Efisiensi** ♻️:
   - Investasikan dalam daur ulang dan pemisahan sampah di sumbernya untuk mengurangi residu.
   - Uji coba program daur ulang di Jagakarsa dan Penjaringan.

4. **Tangani Outlier** 🕵️:
   - Selidiki outlier seperti Jagakarsa (Februari 2024: 220 ton/hari) untuk faktor seperti banjir atau pembuangan industri.
   - Perkuat penegakan aturan terhadap pembuangan ilegal di Penjaringan dan Cakung.

5. **Edukasi Masyarakat** 📢:
   - Luncurkan kampanye di kecamatan hotspot untuk mendorong pengurangan sampah dan pemisahan.
   - Gunakan visualisasi Plotly untuk menyampaikan urgensi kepada publik dan pemangku kepentingan.

> **Catatan**: Beberapa entri (misalnya, Kramat Jati pada Februari 2024: 28741 ton) mungkin anomali dan perlu divalidasi.

🌟 **Jelajahi data sampah Jakarta sekarang dengan visualisasi interaktif dan wawasan actionable!** 🌟
