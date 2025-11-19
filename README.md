# Sistem Prakiraan Cuaca Kabupaten Jombang

Sistem informasi prakiraan cuaca untuk wilayah Kabupaten Jombang yang menggunakan data dari API BMKG (Badan Meteorologi, Klimatologi, dan Geofisika).

## 🌟 Fitur

- ✅ Prakiraan cuaca real-time dari API BMKG
- 🗺️ Pilihan wilayah untuk seluruh kelurahan/desa di Kabupaten Jombang
- 📊 Tampilan cuaca saat ini dengan detail lengkap
- 📅 Prakiraan cuaca 3 hari ke depan (per 3 jam)
- 💾 Cache data untuk performa lebih baik
- 📱 Responsive design untuk mobile dan desktop
- 🎯 Auto-load data saat memilih wilayah
- 💿 Menyimpan pilihan wilayah terakhir

## 🚀 Cara Menjalankan

### Prasyarat
- Node.js versi 14 atau lebih baru
- npm (biasanya sudah terinstal bersama Node.js)

### Instalasi dan Menjalankan

1. **Install dependensi:**
```bash
npm install
```

2. **Jalankan aplikasi:**
```bash
npm start
```

Aplikasi akan otomatis terbuka di browser pada http://localhost:3000

### Perintah Lain

- `npm run dev` - Menjalankan server dan membuka browser
- `npm run serve` - Menjalankan server tanpa membuka browser

## 📂 Struktur Proyek

```
new-prediksi-cuaca/
├── index.html              # Halaman utama
├── script.js              # Logika JavaScript untuk API BMKG
├── style.css              # Styling aplikasi
├── test-kode-wilayah.html # Halaman testing kode wilayah
├── package.json           # Konfigurasi npm
├── .gitignore            # File yang diabaikan git
└── README.md             # Dokumentasi
```

## 🔧 Cara Menggunakan (Metode Alternatif)

### Metode 1: Menggunakan npm (Direkomendasikan)

Gunakan perintah `npm start` seperti dijelaskan di atas.

### Metode 2: Langsung Buka File HTML

1. Buka file `index.html` di browser (Chrome, Firefox, Edge, dll)
2. Pilih kecamatan/wilayah Jombang dari dropdown
3. Data cuaca akan otomatis dimuat

### Metode 3: Menggunakan VS Code Live Server

1. Install extension "Live Server" di VS Code
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"

## 🌐 Sumber Data

Data cuaca diambil dari API resmi BMKG:
- **Base URL:** `https://api.bmkg.go.id/publik/prakiraan-cuaca`
- **Parameter:** `adm4` (kode wilayah tingkat desa/kelurahan)

## 📊 Data yang Ditampilkan

### Cuaca Saat Ini:
- Suhu udara (°C)
- Kondisi cuaca dengan icon
- Kelembapan udara (%)
- Kecepatan angin (km/jam)
- Arah angin
- Jarak pandang
- Tutupan awan (%)

### Prakiraan 3 Hari:
- 8 prakiraan per hari (setiap 3 jam)
- Informasi lengkap untuk setiap periode waktu
- Visualisasi dengan card yang interaktif

## 🗺️ Wilayah yang Tersedia

Sistem ini mendukung prakiraan cuaca untuk berbagai kelurahan/desa di 21 kecamatan Kabupaten Jombang:
- Kec. Jombang
- Kec. Mojoagung
- Kec. Peterongan
- Kec. Diwek
- Kec. Gudo
- Kec. Ngoro
- Kec. Perak
- Kec. Bareng
- Kec. Wonosalam
- Kec. Mojowarno
- Kec. Sumobito
- Kec. Kesamben
- Kec. Tembelang
- Kec. Ploso
- Kec. Plandaan
- Kec. Kabuh
- Kec. Bandarkedungmulyo
- Kec. Jogoroto
- Kec. Megaluh
- Kec. Ngusikan

## ⚠️ Catatan Penting

1. **Koneksi Internet**: Diperlukan koneksi internet untuk mengakses API BMKG
2. **CORS**: Jika mengalami masalah CORS saat membuka langsung file HTML, gunakan local server (npm start atau Live Server)
3. **Rate Limit**: API BMKG memiliki batas permintaan, gunakan cache untuk efisiensi
4. **Sumber Data**: Wajib mencantumkan BMKG sebagai sumber data sesuai ketentuan

## 🎨 Teknologi yang Digunakan

- **HTML5** - Struktur halaman web
- **CSS3** - Styling dengan gradient modern dan responsive design
- **JavaScript (Vanilla)** - Fetch API untuk mengambil data dari BMKG
- **BMKG API** - Sumber data cuaca resmi
- **http-server** - Local web server untuk development

## 🎓 Tentang

Proyek ini dikembangkan oleh **Universitas Brawijaya** sebagai bagian dari kontribusi kampus untuk masyarakat.

**Tagline:** *Dari Kampus untuk Negeri - Menyajikan Prakiraan Cuaca Berbasis Data BMKG*

## 📄 Lisensi

MIT License

Program ini menggunakan data dari BMKG yang bersifat terbuka. Wajib mencantumkan:

**"Sumber Data: BMKG (Badan Meteorologi, Klimatologi, dan Geofisika)"**

## 🔗 Referensi

- [BMKG Data Terbuka](https://data.bmkg.go.id/prakiraan-cuaca)
- [API BMKG Dokumentasi](https://api.bmkg.go.id/)

---

© 2025 Sistem Prakiraan Cuaca Kabupaten Jombang - Universitas Brawijaya. All rights reserved.

**Selamat menggunakan! 🌤️**
