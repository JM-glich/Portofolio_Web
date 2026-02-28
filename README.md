# Portofolio_Web
Nama: Jemis Movid (2409116070).
\
# 🎵 Music Portfolio Website - Movid

## Deskripsi Project
Website portofolio statis bertema Music Producer dengan desain dark neon.
Website ini dibuat menggunakan HTML, CSS, dan Bootstrap 5 untuk memenuhi tugas Praktikum Pemrograman Berbasis Web.
```
music-portfolio-bootstrap/
│
├── index.html
├── style.css
├── README.md
└── screenshots/
    ├── hero.png
    ├── about.png
    ├── certificates.png
```
---

# Tampilan Setiap Section

## 1. Navbar
<img width="765" height="207" alt="image" src="https://github.com/user-attachments/assets/7821a650-815e-4a81-85ea-f3f7730fd2f4" />

Navbar dibuat menggunakan Bootstrap 5 dengan fitur:
- Responsive collapse menu
- Navigation link ke setiap section
- Fixed top position
- Border neon hijau

```html
<nav class="navbar navbar-expand-lg navbar-dark fixed-top">
  <div class="container">
    <a class="navbar-brand glow-text" href="#">MOVID</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
        <li class="nav-item"><a class="nav-link" href="#certificates">Certificates</a></li>
      </ul>
    </div>
  </div>
</nav>
```

Navbar dibuat menggunakan komponen bawaan Bootstrap 5 agar responsif dan mudah diatur. Class navbar-expand-lg memungkinkan menu berubah menjadi toggle pada layar kecil, sedangkan fixed-top membuat navbar tetap berada di bagian atas saat halaman di-scroll. Sistem collapse bekerja melalui atribut data-bs-toggle dan data-bs-target yang terhubung dengan id navbarNav. Class ms-auto digunakan untuk meratakan menu ke sisi kanan. Warna dan border disesuaikan dengan tema dark neon menggunakan bg-black dan border-success.
---

## 2. Hero Section (Home)
<img width="768" height="896" alt="image" src="https://github.com/user-attachments/assets/5d8df0c2-1024-40f1-919f-84aa2625f71f" />

Hero section berisi:
- Nama brand (MOVID)
- Deskripsi singkat
- Background image (music studio)
- Tombol navigasi ke About section

Fitur:
- Fullscreen height (100vh)
- Background overlay gradient
- Neon glow text effect

```html
<section id="home" class="hero d-flex align-items-center justify-content-center text-center">
  <div class="container">
    <h1 class="display-3 text-success fw-bold">MOVID.</h1>
    <p class="lead">Music Producer • Sound Designer • Creative Technologist</p>
    <a href="#about" class="btn btn-success">Explore More</a>
  </div>
</section>
```
Hero section berfungsi sebagai halaman utama yang menampilkan identitas dan deskripsi singkat. Utility class Bootstrap seperti d-flex, align-items-center, dan justify-content-center digunakan untuk memposisikan konten tepat di tengah layar. Class display-3 memperbesar ukuran judul agar lebih menonjol, sedangkan btn btn-success digunakan untuk membuat tombol dengan warna hijau sesuai tema.
---

## 3. About Me Section
<img width="747" height="743" alt="image" src="https://github.com/user-attachments/assets/95f9a1e6-bc48-4504-8f1d-37fc1f155d60" />

Berisi:
- Deskripsi diri
- Music Skills menggunakan Bootstrap Progress Bar
- Experience list

Progress bar menggunakan html dengan class:
```html
    <p>FL Studio</p>
    <div class="progress mb-3">
    <div class="progress-bar bg-success" style="width: 90%"></div>
    </div>

    <p>Mixing & Mastering</p>
    <div class="progress mb-3">
    <div class="progress-bar bg-success" style="width: 85%"></div>
    </div>

    <p>Sound Design</p>
    <div class="progress mb-4">
    <div class="progress-bar bg-success" style="width: 80%"></div>
    </div>
```
Skill ditampilkan menggunakan komponen progress dan progress-bar dari Bootstrap 5. Nilai kemampuan ditentukan melalui atribut style="width: 90%", yang secara visual merepresentasikan tingkat keahlian. Class bg-success digunakan untuk memberikan warna hijau yang konsisten dengan tema website. Pengalaman ditampilkan dalam bentuk unordered list agar informasi tersusun rapi dan mudah dibaca.

## 4. Certificates Section
<img width="750" height="588" alt="image" src="https://github.com/user-attachments/assets/be1aa27a-f4fa-4c33-87c6-1dde6570ffb1" />

Menampilkan daftar sertifikat menggunakan:
- Bootstrap Grid System (row, col-md-4)
- Bootstrap Card
- Custom neon hover effect

```html
<div class="col-md-4">
  <div class="card bg-black border-success h-100">
    <div class="card-body text-light">
      <h5 class="card-title text-success">Digital Audio Production</h5>
      <p class="card-text">Certified Music Production Course</p>
    </div>
  </div>
</div>
```
Section Certificates menggunakan sistem grid Bootstrap dengan row dan col-md-4 sehingga pada layar sedang ke atas akan menampilkan tiga kolom, dan pada layar kecil otomatis menjadi satu kolom. Komponen card digunakan untuk membungkus setiap sertifikat agar terlihat terstruktur dan modern. Class h-100 memastikan tinggi setiap card sama rata.

Hover Effect menggunakan CSS:
```css
.card:hover {
transform: translateY(-5px);
box-shadow: 0 0 15px #00ff88;
}
```
Properti transform membuat card sedikit terangkat saat hover, sedangkan box-shadow menciptakan efek glow neon untuk memperkuat konsep desain dark futuristic.

# Teknologi yang Digunakan:
- HTML5
- CSS3
- Bootstrap 5
- Unsplash Image (Background)
