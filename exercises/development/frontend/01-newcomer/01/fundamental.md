# 📚 FUNDAMENTAL: Pengenalan HTML untuk Kadet

Selamat datang di dunia pemrograman web! Sebagai langkah pertama dalam perjalananmu sebagai Frontend Developer, kamu akan mempelajari **HTML** — bahasa markup dasar yang menjadi pondasi dari semua halaman web di internet.

---

## 🔍 Apa Itu HTML?

**HTML (HyperText Markup Language)** adalah bahasa yang digunakan untuk menyusun struktur dan isi dari sebuah halaman web. HTML bukanlah bahasa pemrograman seperti JavaScript, melainkan bahasa *markup* — yaitu bahasa yang digunakan untuk “menandai” elemen-elemen di dalam sebuah dokumen.

### Analogi Sederhana:

Bayangkan kamu sedang membangun rumah:

- HTML adalah rangka dan struktur bangunannya
- CSS adalah cat, dekorasi, dan interior desain
- JavaScript adalah listrik dan perangkat yang membuat rumahmu "hidup"

---

## 🏗 Struktur Dasar Halaman HTML

Setiap dokumen HTML dimulai dengan struktur seperti ini:

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <title>Judul Halaman</title>
  </head>
  <body>
    <!-- Isi halaman di sini -->
  </body>
</html>
```

### Penjelasan Tag Dasar:

| Tag          | Fungsi                                                             | Contoh Penggunaan                |
| ------------ | ------------------------------------------------------------------ |----------------------------------|
| `<!DOCTYPE>` | Mendeklarasikan bahwa ini adalah dokumen HTML5                     | `<!DOCTYPE html>`                |
| `<html>`     | Elemen utama yang membungkus seluruh isi dokumen HTML              | `<html lang="id"> ... </html>`  |
| `<head>`     | Berisi informasi meta seperti judul, karakter encoding, stylesheet | `<head> ... </head>`             |
| `<title>`    | Judul halaman (muncul di tab browser)                              | `<title>Profil Saya</title>`     |
| `<body>`     | Tempat di mana konten utama website diletakkan                     | `<body> ... </body>`             |

---

## 📑 Tabel Tag HTML Populer & Fungsinya

| Tag         | Fungsi/Deskripsi                                      | Contoh Penggunaan                                  |
|-------------|-------------------------------------------------------|----------------------------------------------------|
| `<h1>`-`<h6>` | Judul utama hingga subjudul kecil                    | `<h1>Judul</h1>`, `<h2>Subjudul</h2>`              |
| `<p>`       | Paragraf teks                                         | `<p>Ini paragraf.</p>`                             |
| `<a>`       | Tautan ke halaman lain atau website                   | `<a href="https://github.com">GitHub</a>`         |
| `<img>`     | Menampilkan gambar                                    | `<img src="foto.jpg" alt="Foto">`               |
| `<ul>`      | Membuat daftar tak berurutan (bullets)                | `<ul><li>Item</li></ul>`                           |
| `<ol>`      | Membuat daftar berurutan (angka)                      | `<ol><li>Item</li></ol>`                           |
| `<li>`      | Item di dalam list                                    | `<li>Belajar HTML</li>`                            |
| `<div>`     | Pembungkus umum, untuk layout atau grup elemen        | `<div class="container">...</div>`                |
| `<span>`    | Pembungkus inline, untuk styling sebagian teks        | `<span style="color:red">merah</span>`            |
| `<br>`      | Baris baru                                            | `Teks<br>Baris Baru`                               |
| `<hr>`      | Garis pemisah horizontal                              | `<hr>`                                             |
| `<form>`    | Formulir input data                                   | `<form>...</form>`                                 |
| `<input>`   | Kolom input (teks, email, password, dsb)              | `<input type="text">`                             |
| `<button>`  | Tombol aksi                                           | `<button>Kirim</button>`                           |
| `<label>`   | Label untuk input/form                                | `<label for="nama">Nama</label>`                  |
| `<section>` | Bagian/area khusus di halaman                         | `<section>...</section>`                            |
| `<nav>`     | Navigasi/menu                                         | `<nav>...</nav>`                                   |
| `<footer>`  | Bagian bawah halaman                                  | `<footer>Copyright</footer>`                       |
| `<header>`  | Bagian atas halaman                                   | `<header>Logo</header>`                            |

---

## 🧩 Elemen-Elemen Dasar HTML (dengan Fungsi Praktis)

### 📌 Heading
Digunakan untuk judul:
```html
<h1>Judul Besar</h1>
<h2>Subjudul</h2>
```

### 📌 Paragraf
Untuk menuliskan teks:
```html
<p>Ini adalah paragraf teks.</p>
```

### 📌 Gambar
Menampilkan gambar:
```html
<img src="https://example.com/gambar.jpg" alt="Deskripsi gambar" />
```

### 📌 Tautan (Link)
Mengarahkan ke halaman lain:
```html
<a href="https://github.com">Kunjungi GitHub</a>
```

### 📌 List
Untuk membuat daftar:
```html
<ul>
  <li>Hobi 1</li>
  <li>Hobi 2</li>
</ul>
```

### 📌 Formulir Sederhana
Untuk input data:
```html
<form>
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama">
  <button type="submit">Kirim</button>
</form>
```

---

## 📖 Kenapa Ini Penting?
- Semua web developer, tanpa terkecuali, harus memahami HTML.
- Kamu tidak bisa membuat website tanpa mengetahui struktur dan isi yang benar.
- HTML adalah titik awal untuk belajar CSS dan JavaScript.

---

## 🧠 Insight Tambahan
- HTML adalah **declarative**, artinya kamu memberitahu browser apa fungsinya ("ini heading", "ini gambar") bukan bagaimana tampilannya.
- HTML tidak sensitif terhadap spasi atau enter, tapi **case-sensitive untuk atribut** (contoh: `alt`, `src`, dll).
- `<div>` dan `<span>` sering dipakai untuk layout dan styling, walau tidak punya makna semantik khusus.
- `<form>`, `<input>`, `<button>` sangat penting untuk interaksi (misal: login, pencarian, dsb).

---

## 🔗 Referensi Tambahan

### Dokumentasi Resmi & Interaktif:
- [MDN Web Docs – HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
- [W3Schools – HTML Tutorial](https://www.w3schools.com/html/)
- [FreeCodeCamp – Responsive Web Design Certification (HTML/CSS)](https://www.freecodecamp.org/learn/)

### Video Interaktif:
- [HTML Crash Course – Traversy Media (YouTube)](https://www.youtube.com/watch?v=UB1O30fR-EE)

---

## ✅ Tips untuk Kadet
- Selalu *preview* hasil HTML kamu di browser.
- Biasakan menulis HTML dengan rapi dan indentasi.
- Jangan hafal semua tag, cukup pahami pola dasarnya.
- Gunakan validator: [https://validator.w3.org](https://validator.w3.org) untuk mengecek apakah HTML-mu valid.
- Jika error, cek urutan tag dan penulisan atribut.

---

> "HTML adalah alfabet dari dunia web. Kamu bisa menulis puisi, artikel, bahkan aplikasi, setelah kamu memahaminya." 🌐

