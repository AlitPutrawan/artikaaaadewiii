# 🍃 Bijak Sampah - Website Edukasi Pengelolaan Sampah

> **Proyek Ujian Tengah Semester (UTS) Pemrograman Web**  
> Website Edukasi Masyarakat Bertema SDGs (SDG 11 & SDG 12)

---

## 👥 Anggota Kelompok & Pembagian Tugas

| No | Nama Anggota | NIM | Pembagian Tugas / Kontribusi |
| :---: | :--- | :---: | :--- |
| **1** | **I Komang Yogi Sai Rama Putra** | 2515091127 | Perancangan Struktur Semantik HTML5, Penataan Beranda & Edukasi |
| **2** | **Gede Alit Putrawan** | 2515091081 | Penyusunan Layout CSS (Flexbox/Grid) & Skema Warna |
| **3** | **Gede Juniarta** | 2515091102 | Penerapan *Responsive Web Design* (Media Queries Tablet & Mobile) |
| **4** | **Gusti Agung Widhyamerta** | 2515091085 | Pembuatan Fitur Interaktif Navigasi & Integrasi JavaScript (`script.js`) |
| **5** | **Putu Angga Agusta Parama Sandhi** | 2515091115 | Riset Konten Edukasi SDGs, Pengumpulan Aset & Dokumentasi `README.md` |

---

## 📌 Deskripsi Website

- **Tema Utama SDGs**: `SDG 11` (Kota dan Komunitas yang Berkelanjutan) dan `SDG 12` (Konsumsi dan Produksi yang Bertanggung Jawab).
- **Sasaran Pengguna**: Masyarakat umum, khususnya skala rumah tangga, pelajar, dan komunitas peduli lingkungan.
- **Tujuan**: Meningkatkan kesadaran masyarakat untuk memilah sampah dari rumah, mengurangi penggunaan limbah plastik sekali pakai, mengolah sampah organik secara mandiri, serta memberikan pemahaman mengenai fasilitas pengolahan sampah seperti TPS3R dan Bank Sampah.
- **Manfaat**: Membantu mengurangi volume sampah yang bermuara di Tempat Pemrosesan Akhir (TPA), mencegah banjir, serta mengurangi pencemaran tanah dan air akibat limbah berbahaya.

---

## 📑 Halaman Website

Website **Bijak Sampah** dirancang secara responsif dengan menyajikan 6 bagian utama yang terinterkoneksi secara mulus melalui navigasi *smooth scrolling*:

1. **Beranda (`#halaman1`)**: Menampilkan *Hero Section* dengan latar belakang visual menarik, judul utama, slogan, dan pengantar pesan pengelolaan sampah.
2. **Edukasi (`#halaman2`)**: Menjelaskan 4 kategori utama sampah rumah tangga (Organik, Anorganik, B3, dan Residu) beserta deskripsi, contoh, dan estimasi waktu terurai.
3. **Dampak (`#halaman3`)**: Menggambarkan bahaya nyata jika sampah tidak dikelola, seperti banjir, sarang penyakit, pencemaran tanah, dan kerusakan ekosistem laut.
4. **Solusi (`#halaman4`)**: Menyediakan panduan praktis pengelolaan mandiri melalui metode Komposting, 3R & Upcycling, penanganan B3, residu, dan link tutorial daur ulang.
5. **Artikel (`#halaman5`)**: Mengedukasi masyarakat tentang alur pengolahan sampah, peran fasilitas **TPS3R**, dan nilai luhur **Gotong Royong**.
6. **Tentang (`#halaman6`)**: Menyajikan latar belakang tujuan platform, profil anggota kelompok pengembang, serta daftar rujukan ilmiah.

---

## 🛠️ Teknologi yang Digunakan

- **HTML5**: Menggunakan tag semantik modern (`<header>`, `<nav>`, `<section>`, `<article>`, `<main>`, `<footer>`).
- **CSS3**: Menggunakan *CSS Custom Properties*, *Flexbox*, *CSS Grid*, dan *Media Queries*.
- **FontAwesome (v6.7.2)**: Penyedia ikon vektor responsif untuk antarmuka pengguna (UI).
- **Google Fonts**: Menggunakan *font family* `'Poppins'` untuk keterbacaan tipografi.
- **JavaScript (Vanilla JS)**: Mengontrol interaktivitas menu navigasi *hamburger* pada perangkat *mobile*.

---

## 🔍 Penjelasan Implementasi

### 1. Navigasi

Navbar memakai tag `<nav>` dan berada di bagian atas header. Tombol *hamburger* disiapkan untuk tampilan *mobile*, dan navigasi berpindah section menggunakan *anchor link* (`#halamanX`).

```html
<header class="site-bar">
  <nav class="nav-bar">
    <img src="Photos/Logo Sampah.png" alt="logo" class="logo" />
    <div class="hamburger" id="hamburger-btn">
      <i class="fa-solid fa-bars"></i>
    </div>
    <div class="nav-menu" id="nav-menu">
      <div id="icon">
        <i class="fa-solid fa-xmark"></i>
      </div>
      <div id="menu">
        <a href="#halaman1" class="brand">Beranda</a>
        <a href="#halaman2">Edukasi</a>
        <a href="#halaman3">Dampak</a>
        <a href="#halaman4">Solusi</a>
        <a href="#halaman5">Artikel</a>
        <a href="#halaman6">Tentang</a>
      </div>
    </div>
  </nav>
</header>
```
**FUNGSI**
- `<a href="#halamanX">` memindahkan pengunjung langsung ke bagian section tertentu tanpa perlu reload, memanfaatkan smooth scroll.

- `<div class="hamburger" id="hamburger-btn">` berfungsi sebagai tombol pembuka menu saat website dibuka dari layar HP/smartphone.

- `<div id="icon">` berisi ikon silang (fa-xmark) yang digunakan untuk menutup kembali menu mobile yang sedang terbuka.
