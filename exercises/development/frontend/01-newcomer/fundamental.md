# 📚 FUNDAMENTAL: Panduan Awal Frontend Web untuk Semua Kalangan

Selamat datang di dunia pengembangan web! Di level Newcomer ini, kamu akan belajar membangun halaman web pertamamu dari NOL, tanpa perlu pengalaman teknis sebelumnya. Setiap bagian disusun dengan cerita, langkah-langkah jelas, dan tips praktis agar mudah diikuti siapa saja.

---

## 1️⃣ HTML – Kartu Nama Digitalmu

**Fungsi Tagline/Fiksi:**
Kita menggunakan cerita “kartu nama digital” agar kamu bisa langsung membayangkan hasil nyata dari belajar HTML. Dengan membuat profil sederhana, kamu belajar pondasi semua halaman web.

**Fungsi HTML di Dunia Nyata:**
HTML adalah “kerangka” atau “tulang” dari semua website. Semua konten (teks, gambar, link) di internet diatur dengan HTML. Tanpa HTML, halaman web tidak punya struktur.

### Cerita
Bayangkan kamu ingin memperkenalkan dirimu di dunia maya, seperti membuat kartu nama digital yang bisa dilihat siapa saja. HTML adalah pondasi semua halaman web.

### Langkah-Langkah Dasar
1. Buka Notepad/VS Code/CodePen.
2. Buat file baru: `index.html`.
3. Salin struktur berikut:
   ```html
   <!DOCTYPE html>
   <html lang="id">
     <head>
       <meta charset="UTF-8" />
       <title>Profil Saya</title>
     </head>
     <body>
       <!-- Konten kamu di sini -->
     </body>
   </html>
   ```
4. Tambahkan:
   - `<h1>` Nama kamu
   - `<p>` Deskripsi singkat
   - `<img>` Foto profil/hobi
   - `<a>` Link ke GitHub
5. Simpan dan buka di browser.

### Checklist
- [ ] File `index.html` sudah dibuat
- [ ] Ada heading, paragraf, gambar, dan link
- [ ] Sudah dicoba di browser

### Preview Hasil
```
+-----------------------------+
|        Nama Kamu            |
|  [Foto]                     |
|  Saya suka belajar...       |
|  GitHub: [link]             |
+-----------------------------+
```

### Tips & Troubleshooting
- Pastikan file berekstensi `.html`
- Link gambar harus valid (http/https)
- Link `<a>` harus benar penulisannya

---

### 🗂️ Glossary Istilah Penting

| Istilah      | Penjelasan Singkat                                                                 |
|--------------|------------------------------------------------------------------------------------|
| HTML         | Bahasa untuk membuat struktur halaman web.                                         |
| Tag          | Tanda khusus di HTML, misal `<h1>`, `<p>`, `<img>`.                               |
| Heading      | Judul di halaman, biasanya `<h1>`, `<h2>`, dst.                                   |
| Paragraf     | Blok teks, ditulis dengan `<p>`.                                                  |
| Link         | Tautan ke halaman lain, ditulis dengan `<a>`.                                     |
| Attribute    | Info tambahan di tag, misal `src` di `<img src="...">`.                         |
| Browser      | Aplikasi untuk membuka web (Chrome, Firefox, Edge, dll).                          |
| Preview      | Melihat hasil kerja di browser.                                                   |

---

## 2️⃣ CSS – Mendekorasi Profilmu

**Fungsi Tagline/Fiksi:**
Cerita “mendekorasi profil” membantu kamu memahami bahwa CSS adalah alat untuk mempercantik dan menata halaman, seperti mendekorasi kamar atau buku harian.

**Fungsi CSS di Dunia Nyata:**
CSS mengatur warna, font, layout, dan keindahan halaman web. Tanpa CSS, semua website akan terlihat polos dan membosankan.

### Cerita
Setelah punya kartu nama digital, saatnya mendekorasi! CSS ibarat pakaian dan gaya rambut halamanmu.

### Langkah-Langkah Dasar
1. Buat file baru: `style.css`.
2. Hubungkan ke HTML di `<head>`:
   ```html
   <link rel="stylesheet" href="style.css" />
   ```
3. Tambahkan aturan CSS:
   ```css
   body { font-family: sans-serif; background: #f4f4f4; }
   h1 { color: #1976d2; text-align: center; }
   p { font-size: 16px; text-align: justify; }
   .container { max-width: 600px; margin: auto; }
   ```
4. Untuk gambar & list hobi, bungkus dengan `<div class="container">` dan tambahkan Flexbox:
   ```css
   .container { display: flex; gap: 20px; }
   ```
5. Simpan dan refresh browser.

### Checklist
- [ ] File `style.css` sudah dibuat & terhubung
- [ ] Warna, font, dan layout berubah
- [ ] Gambar & list hobi tersusun rapi

### Preview Hasil
```
+-----------------------------+
|        Nama Kamu            |
|  [Foto]   [List Hobi]       |
|  Saya suka belajar...       |
+-----------------------------+
```

### Tips & Troubleshooting
- Jika warna tak berubah, cek koneksi CSS di `<head>`
- Gunakan DevTools (klik kanan > Inspect) untuk eksperimen

---

### 🗂️ Glossary Istilah Penting

| Istilah      | Penjelasan Singkat                                                                 |
|--------------|------------------------------------------------------------------------------------|
| CSS          | Bahasa untuk mengatur tampilan halaman web.                                        |
| Selector     | Bagian CSS yang memilih elemen HTML, misal `h1`, `.container`.                     |
| Property     | Sifat yang diatur di CSS, misal `color`, `font-size`.                              |
| Value        | Nilai dari property, misal `blue`, `16px`.                                         |
| Flexbox      | Cara modern untuk mengatur layout elemen secara fleksibel.                         |
| Responsive   | Tampilan web yang tetap bagus di HP dan laptop.                                    |
| Class        | Nama khusus untuk kelompok elemen, ditulis di HTML: `class="container"`.         |
| Margin       | Jarak luar elemen.                                                                 |
| Padding      | Jarak dalam elemen.                                                                |
| DevTools     | Alat di browser untuk cek dan edit tampilan web secara langsung.                   |

---

## 3️⃣ JavaScript – Membuat Profilmu Interaktif

**Fungsi Tagline/Fiksi:**
Dengan “kartu ucapan digital yang hidup”, kamu belajar bahwa JavaScript membuat halaman web bisa merespon pengguna, seperti tombol yang bisa diklik atau sapaan otomatis.

**Fungsi JavaScript di Dunia Nyata:**
JavaScript membuat web jadi interaktif: tombol, animasi, form, popup, dan banyak fitur modern di web berjalan dengan JS.

### Cerita
Profilmu kini bisa menyapa pengunjung atau berubah warna saat tombol ditekan, seperti kartu ucapan digital yang "hidup"!

### Langkah-Langkah Dasar
1. Tambahkan tombol di HTML:
   ```html
   <button id="changeColorBtn">Ubah Warna Background</button>
   ```
2. Buat file baru: `script.js` dan hubungkan sebelum `</body>`:
   ```html
   <script src="script.js"></script>
   ```
3. Tambahkan kode berikut di `script.js`:
   ```js
   document.getElementById("changeColorBtn").onclick = function() {
     const colors = ["#f4f4f4", "#e0f7fa", "#ffebee", "#f3e5f5"];
     const chosen = colors[Math.floor(Math.random() * colors.length)];
     document.body.style.backgroundColor = chosen;
     alert("Background diubah!");
   };
   ```
4. Tambahkan input nama & tombol sapa:
   ```html
   <input type="text" id="namaInput" placeholder="Masukkan namamu" />
   <button id="greetBtn">Sapa Saya!</button>
   <div id="greetResult"></div>
   ```
5. Tambahkan kode berikut di `script.js`:
   ```js
   document.getElementById("greetBtn").onclick = function() {
     const nama = document.getElementById("namaInput").value;
     document.getElementById("greetResult").innerText = "Halo, " + nama + "!";
   };
   ```
6. Simpan dan coba di browser.

### Checklist
- [ ] Tombol ubah warna berfungsi
- [ ] Input nama & sapaan muncul
- [ ] Semua file terhubung & dicoba

### Preview Hasil
```
+-----------------------------+
|        Nama Kamu            |
|  [Foto]                     |
|  Saya suka belajar...       |
|  [Tombol Ubah Warna]        |
|  [Input Nama] [Sapa Saya!]  |
|  Halo, [namamu]!            |
+-----------------------------+
```

### Tips & Troubleshooting
- Jika tombol tak berfungsi, cek koneksi `script.js`
- Gunakan `console.log()` untuk debugging (Ctrl+Shift+I > Console)

---

### 🗂️ Glossary Istilah Penting

| Istilah      | Penjelasan Singkat                                                                 |
|--------------|------------------------------------------------------------------------------------|
| JavaScript   | Bahasa pemrograman untuk membuat web jadi interaktif.                              |
| Script       | Kode program, biasanya di file `.js`.                                              |
| Event        | Aksi pengguna, misal klik, input, scroll.                                          |
| Function     | Blok kode yang bisa dijalankan berulang.                                           |
| Variable     | Tempat menyimpan data sementara.                                                   |
| DOM          | Struktur data yang mewakili isi halaman web.                                       |
| Alert        | Pesan pop-up di browser.                                                           |
| Debugging    | Proses mencari dan memperbaiki error/kesalahan di kode.                            |
| Console      | Tempat melihat pesan/error di browser (Ctrl+Shift+I > Console).                    |

---

## 4️⃣ Mini Project – Poster Digital / Landing Page

**Fungsi Tagline/Fiksi:**
“Poster digital” atau “landing page” adalah latihan menggabungkan semua skill, seperti membuat brosur online yang bisa diakses siapa saja.

**Fungsi Mini Project di Dunia Nyata:**
Landing page banyak dipakai untuk promosi produk, portofolio, atau event. Ini latihan membangun web utuh dari awal.

### Cerita
Saatnya membuat poster digital untuk ide, produk, atau acara kamu! Ini latihan menggabungkan semua skill yang sudah dipelajari.

### Langkah-Langkah Dasar
1. Pilih tema: produk fiktif, portofolio, atau acara komunitas.
2. Buat file: `index.html`, `style.css`, `script.js`.
3. Struktur HTML:
   - Header (logo & navbar)
   - Hero section (judul besar & tombol CTA)
   - Section fitur/deskripsi
   - Footer sederhana
4. Tambahkan class/id untuk styling/interaksi.
5. CSS: Gunakan Flexbox/Grid, warna & font harmonis, responsive.
6. JS: Tombol CTA (popup/scroll), form input dengan validasi sederhana.
7. Simpan & coba semua fitur di browser.

### Checklist
- [ ] Semua file sudah dibuat & terhubung
- [ ] Ada header, hero, fitur, footer
- [ ] Tombol CTA & form berfungsi
- [ ] Responsive di HP & laptop

### Preview Hasil
```
+----------------------------+
| LOGO    | Home | About |  |
+----------------------------+
|     Welcome to [App]      |
|    [CTA Button]           |
+----------------------------+
| Fitur 1 | Fitur 2 | Fitur 3|
+----------------------------+
|   Footer - Contact Info   |
+----------------------------+
```

### Tips & Troubleshooting
- Jika tampilan berantakan, cek struktur HTML & CSS
- Preview di HP & laptop
- Selesaikan fitur utama dulu, baru percantik

---

### 🗂️ Glossary Istilah Penting

| Istilah      | Penjelasan Singkat                                                                 |
|--------------|------------------------------------------------------------------------------------|
| Landing Page | Halaman web utama untuk promosi/tujuan khusus.                                     |
| Header       | Bagian atas halaman, biasanya berisi logo & menu.                                 |
| Hero Section | Bagian utama dengan judul besar & CTA.                                            |
| CTA          | Call To Action, tombol/ajakan untuk aksi utama.                                   |
| Footer       | Bagian bawah halaman, biasanya info kontak/copyright.                             |
| Navbar       | Navigasi/menu di halaman.                                                         |
| Validasi     | Mengecek input agar sesuai aturan.                                                |
| Popup        | Jendela kecil yang muncul di atas halaman.                                        |

---

## 📖 Referensi & Video
- [MDN Web Docs – HTML, CSS, JS](https://developer.mozilla.org/en-US/docs/Learn)
- [W3Schools – HTML, CSS, JS](https://www.w3schools.com/)
- [FreeCodeCamp – Responsive Web Design](https://www.freecodecamp.org/learn/)
- [HTML Crash Course – Traversy Media (YouTube)](https://www.youtube.com/watch?v=UB1O30fR-EE)
- [CSS Crash Course – Traversy Media (YouTube)](https://www.youtube.com/watch?v=yfoY53QXEnI)
- [JavaScript for Beginners – Codevolution (YouTube)](https://www.youtube.com/watch?v=PkZNo7MFNFg)
- [Build a Simple Landing Page – Dev Ed (YouTube)](https://www.youtube.com/watch?v=27JtRAI3QO8)

---

> "Belajar web itu seperti membangun rumah: mulai dari pondasi, dekorasi, lalu menghidupkan suasana. Nikmati prosesnya, dan jangan ragu bertanya!" 🚀 