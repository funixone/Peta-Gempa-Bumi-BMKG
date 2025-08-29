# 🌏 Peta Gempa Bumi BMKG

Aplikasi web untuk memantau gempa bumi terkini di Indonesia berdasarkan data dari **BMKG** (Badan Meteorologi, Klimatologi, dan Geofisika).  
Aplikasi ini menampilkan lokasi gempa pada peta interaktif dengan notifikasi real-time untuk gempa terbaru.

---

## ✨ Fitur

- 🗺️ **Peta Interaktif**: Menampilkan lokasi gempa dengan marker berbentuk lingkaran, ukuran dan warnanya bervariasi berdasarkan magnitudo.  
- 🔔 **Notifikasi Real-time**: Notifikasi otomatis muncul di pojok kanan bawah ketika ada gempa baru.  
- 🌍 **Multi-layer Peta**: Dukungan untuk peta standar dan citra satelit.  
- 📱 **Responsif**: Tampilan optimal di desktop maupun perangkat mobile.  
- ⏱️ **Auto-update**: Data gempa diperbarui otomatis setiap 1 menit.  
- ℹ️ **Informasi Detail**: Klik marker untuk melihat detail gempa (waktu, magnitudo, kedalaman, lokasi, dll.).  
- 🖍️ **Legenda**: Panduan visual untuk memahami makna warna dan ukuran marker.  

---

## 🛠️ Teknologi

- **HTML5, CSS3, JavaScript**  
- **Leaflet** → Library peta interaktif  
- **Font Awesome** → Ikon  
- **BMKG Data** → Sumber data gempa  

---

## 🚀 Cara Menggunakan

1. Clone atau download repository ini.  
2. Buka file `index.html` di browser web.  
3. Aplikasi akan otomatis menampilkan peta dan memuat data gempa terkini.  
4. Notifikasi akan muncul otomatis ketika ada gempa baru.  
5. Klik lingkaran gempa untuk melihat informasi detail.  
6. Gunakan kontrol di pojok kanan atas untuk mengganti jenis peta.  

---

## 📂 Struktur File

```
├── index.html          # File utama aplikasi
└── README.md           # Dokumentasi proyek
```

---

## 🎨 Warna Marker Berdasarkan Magnitudo

- 🔴 **Merah** (> 6 SR) → Gempa kuat  
- 🟠 **Oranye** (5 - 6 SR) → Gempa menengah  
- 🟡 **Kuning** (4 - 5 SR) → Gempa ringan  
- 🟢 **Hijau Muda** (3 - 4 SR) → Gempa sangat ringan  
- 🟢 **Hijau** (< 3 SR) → Gempa minor  

---

## 🔑 Fungsi Utama

- `loadGempa()` → Memuat data gempa dari API BMKG  
- `getColor(mag)` → Menentukan warna marker berdasarkan magnitudo  
- `showNotification(gempa)` → Menampilkan notifikasi gempa baru  
- `getNotificationClass(mag)` → Menentukan kelas notifikasi berdasarkan magnitudo  

---

## 🌐 API yang Digunakan

Aplikasi mengambil data dari endpoint BMKG:

```
https://data.bmkg.go.id/DataMKG/TEWS/gempaterkini.json
```
