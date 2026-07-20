# 📒 Pencatat Progres Mandor (BA)

Aplikasi web **Single-File HTML** murni untuk mencatat progres pekerjaan mandor, akumulasi termin Berita Acara (BA), dan mencegah kesalahan perhitungan akibat perubahan adendum. Berjalan **100% Offline** tanpa dependency, tanpa server, dan tanpa proses build.

---

## 🌟 Keunggulan Utama

* ⚡ **100% Offline & Serverless**: Data tersimpan aman di browser lokal Anda (`localStorage`). Dapat dijalankan di mana saja tanpa butuh koneksi internet.
* 🎯 **Mencegah Salah Hitung Adendum**: Perhitungan termin otomatis ($\text{Termin} = \text{Kumulatif} - \text{Sebelumnya}$). Dilengkapi deteksi dini saat nilai kontrak berubah (*Adendum Warning*).
* 🔍 **Parsing Baris Otomatis**: Cukup *copy-paste* baris teks BA / Excel, parser akan mengekstrak Nama Mandor, Jenis Pekerjaan, Persen Progres, Nilai Kontrak, dan Nilai Kumulatif secara presisi.
* 🔗 **Linked Auto-Suggestion Input**: Kolom input Mandor dan Pekerjaan saling terhubung. Mengetik nama Mandor akan langsung menyaring daftar pekerjaan yang relevan dengannya.
* 🎨 **Epic Animation Pack (Silky 60FPS)**:
  * 🌊 **Staggered Entrance**: Animasi kemunculan kartu UI yang halus.
  * 🔢 **Odometer Number Counter**: Efek penghitung naik untuk *Grand Total* rupiah dengan efek *glow pulse*.
  * ⚡ **Parse Sequence**: Animasi sorot (*scanning highlight*) berurutan saat data BA di-parse.
  * 💥 **Particle Burst (Confetti)**: Ledakan partikel offline saat data berhasil disimpan.
  * 🪄 **Ripple & Magnetic Buttons**: Efek riak air saat tombol diklik dan efek terangkat (*hover*).
  * 🍞 **Glassmorphism Toast**: Notifikasi mengambang kaca buram (*backdrop-filter*) yang responsif.
* 📂 **Urutan Dinamis & Collapsible Cards**: Kartu kelompok mandor dengan aktivitas progres terbaru akan otomatis naik ke **posisi paling atas**. Tabel rincian dapat diciutkan (*collapsed*) untuk menjaga tampilan tetap ringkas.
* 📊 **Multi Rekap Real-time**: Rekapitulasi termin otomatis per **Pekerjaan**, per **Mandor**, dan per **Tempat** (Dapur, Gedung, Ruko, dll.).
* 💾 **Backup & Migration**: Fitur Export & Import data berbasis JSON untuk pencadangan atau pemindahan data antar perangkat.

---

## 🚀 Cara Penggunaan

1. Unduh atau *clone* repository ini:
   ```bash
   git clone https://github.com/maulinul/rekapmandor.git
   ```
2. Buka file [`index.html`](file:///d:/FIle%20Kerja/AI/Antigravity%20IDE/index.html) langsung dengan mengklik dua kali pada file tersebut atau membukanya melalui browser favorit Anda (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari, dll.).
3. Tidak memerlukan instalasi Node.js, `npm`, web server, maupun koneksi internet!

---

## 🛠️ Fitur & Pengaturan (⚙️ Setting)

* **Tema Tampilan**: Mendukung tema **☀️ Terang**, **🌙 Gelap**, dan **🖥 Otomatis** mengikuti preferensi sistem perangkat.
* **Format Angka**: Pilihan format angka otomatis untuk bahasa Indonesia (pemisah ribuan titik `.`, desimal koma `,`) atau Inggris.
* **Kata Kunci Tempat**: Kustomisasi kata kunci pencarian lokasi/tempat (default: `Dapur`, `Gedung`, `Blok`, `Gudang`, `Ruko`, `Lantai`, `LT`) untuk pengelompokan rekap lokasi.
* **Regex Kustom**: Mendukung penyesuaian pola parsing teks BA tingkat lanjut untuk format laporan kustom.

---

## 📄 Lisensi

Proyek ini bersifat Open Source di bawah lisensi [MIT License](LICENSE). Bebas digunakan dan dikembangkan untuk keperluan pribadi maupun profesional.
