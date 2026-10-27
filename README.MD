# 🍃 Bijak Sampah - Pengelolaan Sampah Rumah Tangga

> **Website Edukasi Pengelolaan Sampah Rumah Tangga Bertema SDGs (SDG 11 & SDG 12)**  
> Proyek Ujian Tengah Semester (UTS) Mata Kuliah Pemrograman Web

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

* **Tema Utama SDGs**:
  * **SDG 11**: *Sustainable Cities and Communities* (Kota dan Komunitas yang Berkelanjutan)[cite: 2].
  * **SDG 12**: *Responsible Consumption and Production* (Konsumsi dan Produksi yang Bertanggung Jawab)[cite: 2].
* **Sasaran Pengguna**: Masyarakat umum, khususnya skala rumah tangga, pelajar, dan komunitas peduli lingkungan.
* **Tujuan**: Tujuan utama dari pembuatan sistem ini adalah mengintegrasikan seluruh proses bisnis ke dalam satu platform sentral melalui sembilan modul fungsional. Untuk mendukung pengambilan keputusan yang strategis, aplikasi ini menyediakan dasbor eksekutif interaktif yang menampilkan Key Performance Indicators (KPI), tren okupansi, dan peringatan otomatis secara seketika.
* **Manfaat**: Membantu mengurangi volume sampah yang bermuara di Tempat Pemrosesan Akhir (TPA), mencegah banjir, serta mengurangi pencemaran tanah dan air akibat limbah berbahaya.

---

## 📑 Struktur Bagian / Halaman Website

Website **Bijak Sampah** dirancang secara responsif dengan menyajikan 6 bagian utama yang terinterkoneksi secara mulus melalui navigasi *smooth scrolling*:

1. **Beranda (`#halaman1`)**: Menampilkan *Hero Section* dengan latar belakang visual menarik, judul utama, slogan, dan pengantar pesan pentingnya mengelola sampah demi bumi.
2. **Edukasi (`#halaman2`)**: Menjelaskan 4 kategori utama sampah rumah tangga (Organik, Anorganik, B3, dan Residu) lengkap dengan deskripsi, contoh material, rentang waktu terurai secara alami, serta visual pendukung.
3. **Dampak (`#halaman3`)**: Menggambarkan bahaya nyata jika sampah tidak dikelola dengan baik, seperti timbulnya banjir, sarang penyakit (DBD, diare), pencemaran tanah, dan kerusakan ekosistem laut akibat mikroplastik[cite: 3].
4. **Solusi (`#halaman4`)**: Menyediakan panduan praktis pengelolaan mandiri melalui metode Komposting (Organik), 3R & Upcycling (Anorganik), penanganan khusus limbah B3, pengolahan residu, serta tautan tutorial daur ulang kreatif berbentuk video[cite: 3].
5. **Artikel (`#halaman5`)**: Mengedukasi masyarakat tentang peran komunitas, alur pengelolaan sampah dari rumah tangga, pengertian fasilitas pengolahan **TPS3R**, dan nilai luhur **Gotong Royong**[cite: 3].
6. **Tentang (`#halaman6`)**: Menyajikan latar belakang tujuan pengembangan platform, profil anggota kelompok pengembang, serta rujukan/referensi ilmiah dan kredibel[cite: 3].

---

## 🛠️ Teknologi yang Digunakan

* **HTML5**: Menggunakan tag semantik modern (`<header>`, `<nav>`, `<section>`, `<article>`, `<main>`, `<footer>`)[cite: 3].
* **CSS3**: Menggunakan *CSS Custom Properties* (Variables), *Flexbox*, *CSS Grid*, dan *Media Queries*[cite: 3].
* **FontAwesome (v6.7.2)**: Penyedia ikon vektor responsif untuk memperjelas visual antarmuka pengguna (UI).
* **Google Fonts**: Menggunakan *font family* `'Poppins'` untuk keterbacaan tipografi yang optimal.
* **JavaScript (Vanilla JS)**: Mengontrol interaktivitas menu navigasi *hamburger* pada perangkat *mobile* (layar kecil).

---

## 1. NAVIGASI YANG DIGUNAKAN 
Navbar memakai tag <nav> dan berada di bagian atas header. Tombol hamburger disiapkan untuk tampilan mobile, dan navigasi berpindah section menggunakan anchor link (#halamanX)
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
## FUNGSI 
1. Setiap <a href="#halamanX"> memindahkan pengunjung langsung ke bagian section tertentu pada halaman tanpa perlu reload, memanfaatkan smooth scroll.  
2. Tag <div class="hamburger" id="hamburger-btn"> berfungsi sebagai tombol pembuka menu saat website dibuka dari layar HP/smartphone.   
3. Tag <div id="icon"> berisi ikon silang (fa-xmark) yang digunakan untuk menutup kembali menu mobile yang sedang terbuka.   
