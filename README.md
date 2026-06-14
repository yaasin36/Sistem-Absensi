# SPACE - Sistem Presensi Digital (Face Detection & Geolocation)

![SPACE App Banner](https://via.placeholder.com/1000x400.png?text=SPACE+-+Sistem+Presensi+Digital) **SPACE** adalah aplikasi absensi berbasis web (Single Page Application) yang dirancang khusus untuk PT Garuda Karya Solution. Dibangun dengan pendekatan *Mobile-First*, aplikasi ini mengintegrasikan teknologi **Face Detection** (menggunakan `face-api.js`), pelacakan **Geolocation**, dan penyimpanan *serverless* menggunakan **Google Apps Script (GAS)**.

---

## ✨ Fitur Utama

### Akses Pengguna (User/Karyawan)
* **Kamera Absensi Cerdas:** Presensi Masuk dan Pulang yang dilengkapi deteksi wajah *real-time*. Tombol jepret hanya akan aktif jika wajah terdeteksi.
* **Live Watermark & Geolocation:** Setiap foto absensi otomatis dicetak dengan nama karyawan, waktu (waktu nyata), dan titik koordinat GPS.
* **Dashboard Interaktif:** Menampilkan jam *real-time*, status absensi hari ini, ringkasan aktivitas terakhir, dan *glass-morphism weekly calendar*.
* **Pengajuan Izin/Cuti:** Formulir digital untuk mengajukan izin, sakit, atau cuti, lengkap dengan fitur unggah dokumen/surat dokter.
* **Riwayat Kalender:** Tampilan kalender bulanan dengan indikator warna (*dot*) untuk melacak status kehadiran (Lengkap, Sebagian, Izin, Alpa).
* **Manajemen Profil:** Pengguna dapat mengubah foto profil dan memperbarui kata sandi secara mandiri.
* **Notifikasi:** Sistem pengingat harian untuk absensi masuk/pulang.

### Akses Administrator (SuperAdmin/Admin)
* **Rekap Data Absensi:** Tabel pemantauan kehadiran seluruh tim, dilengkapi filter berdasarkan Tanggal, Posisi, dan Divisi. Tautan langsung untuk melihat bukti foto absensi.
* **Manajemen Karyawan (CRUD):** Menambah, mengedit, dan menghapus data karyawan beserta hak akses (*role*) mereka langsung dari antarmuka aplikasi.

---

## 🛠️ Teknologi yang Digunakan

**Frontend:**
* HTML5, CSS3, Vanilla JavaScript
* [Bootstrap 5.3](https://getbootstrap.com/) & Bootstrap Icons (UI Framework & Styling)
* [face-api.js](https://github.com/justadudewhohacks/face-api.js) (Machine Learning Model untuk Face Detection di browser)

**Backend & Database:**
* [Google Apps Script (GAS)](https://developers.google.com/apps-script) sebagai REST API.
* Google Sheets (sebagai Database terpusat).
* Google Drive (sebagai penyimpanan foto absensi dan surat dokter).

---

## 🚀 Cara Instalasi & Penggunaan

### 1. Kloning Repositori
Clone repositori ini ke dalam mesin lokal Anda:
```bash
git clone [https://github.com/yaasin36/space-absensi.git](https://github.com/yaasin36/space-absensi.git)
cd space-absensi