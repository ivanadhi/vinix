# Dasbor Analisis Umpan Balik SmartX

Ini adalah proyek dasbor interaktif yang dibuat sebagai file HTML mandiri untuk menganalisis dan memvisualisasikan data umpan balik pengguna untuk aplikasi fiksi bernama "SmartX". Dasbor ini dibangun menggunakan React, Recharts untuk pembuatan bagan, dan Tailwind CSS untuk penataan gaya.

## Pratinjau Dasbor

![Pratinjau Dasbor SmartX](https://i.imgur.com/YOUR_IMAGE_URL.png) 

## Deskripsi

Dasbor ini memberikan wawasan tentang metrik keterlibatan pengguna, penggunaan fitur, dan peringkat kepuasan di berbagai kecamatan selama periode enam bulan (Januari hingga Juni). Dasbor ini sepenuhnya mandiri, dengan data CSV yang disematkan langsung di dalam file HTML, dan dirender secara dinamis di browser menggunakan React dan Recharts.

Tujuan utama dari dasbor ini adalah untuk:
- Melacak tren pengguna aktif dari waktu ke waktu.
- Membandingkan popularitas berbagai fitur aplikasi.
- Menganalisis peringkat kepuasan pengguna untuk setiap fitur.
- Mengidentifikasi korelasi potensial antara penggunaan fitur dan kepuasan.

## Fitur Utama

- **HTML Mandiri:** Seluruh aplikasi, termasuk data, logika, dan gaya, terkandung dalam satu file HTML. Tidak diperlukan server atau proses build.
- **Visualisasi Data Interaktif:** Bagan yang dibuat dengan Recharts menyediakan tooltip interaktif untuk melihat titik data secara detail.
- **Analisis Komprehensif:** Dasbor mencakup beberapa visualisasi untuk memberikan pandangan 360 derajat tentang kinerja aplikasi:
    - **Pengguna Aktif dari Waktu ke Waktu:** Grafik garis yang menunjukkan tren pengguna aktif bulanan untuk setiap kecamatan.
    - **Penggunaan Fitur Rata-Rata:** Bagan batang bertumpuk yang membandingkan popularitas fitur Domisili, Pajak, Keluhan, dan Chatbot.
    - **Peringkat Fitur Rata-Rata:** Bagan batang yang menampilkan peringkat kepuasan rata-rata untuk setiap fitur di berbagai kecamatan.
    - **Penggunaan vs. Peringkat Chatbot:** Grafik sebar untuk mengeksplorasi hubungan antara persentase penggunaan chatbot dan peringkat kepuasannya.
- **Pewarnaan Dinamis:** Skema warna yang konsisten digunakan di seluruh bagan untuk memudahkan identifikasi kecamatan dan fitur.
- **Wawasan Utama:** Ringkasan dan fakta menarik disorot untuk memberikan kesimpulan yang dapat ditindaklanjuti dari data.

## Teknologi yang Digunakan

- **HTML:** Sebagai struktur dasar halaman.
- **CSS (Tailwind CSS):** Untuk penataan gaya dan tata letak yang responsif.
- **JavaScript (ES6+):** Untuk logika dan fungsionalitas aplikasi.
- **React:** Untuk membangun antarmuka pengguna sebagai aplikasi satu halaman.
- **Recharts:** Untuk membuat bagan yang responsif dan dapat disesuaikan.
- **PapaParse:** Untuk mengurai data CSV yang disematkan.
- **Babel (Standalone):** Untuk mentranspilasi kode JSX React langsung di browser.

## Sumber Data

Data umpan balik pengguna disematkan di dalam file HTML sebagai string dalam variabel JavaScript `gk_fileData`. Data tersebut mewakili 100 baris catatan umpan balik dari file `smartx_feedback_100rows.csv`.

Struktur data mencakup kolom-kolom berikut:
- `Bulan`: Bulan pengumpulan data.
- `Kecamatan`: Kecamatan tempat pengguna berada.
- `Pengguna_Aktif`: Jumlah pengguna aktif.
- `Domisili_Usage(%)`: Persentase penggunaan fitur domisili.
- `Pajak_Usage(%)`: Persentase penggunaan fitur pajak.
- `Keluhan_Usage(%)`: Persentase penggunaan fitur keluhan.
- `Chatbot_Usage(%)`: Persentase penggunaan fitur chatbot.
- `Rating_Domisili`: Peringkat rata-rata untuk fitur domisili (skala 1-5).
- `Rating_Pajak`: Peringkat rata-rata untuk fitur pajak (skala 1-5).
- `Rating_Keluhan`: Peringkat rata-rata untuk fitur keluhan (skala 1-5).
- `Rating_Chatbot`: Peringkat rata-rata untuk fitur chatbot (skala 1-5).

## Cara Menggunakan

Tidak ada instalasi atau proses build yang diperlukan. Cukup unduh file `nama_file_anda.html` dan buka langsung di peramban web modern apa pun (seperti Google Chrome, Firefox, atau Microsoft Edge).

```bash
# Cukup buka file HTML di browser Anda
buka nama_file_anda.html
