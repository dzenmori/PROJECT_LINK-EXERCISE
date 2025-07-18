# 📚 FUNDAMENTAL: Dasar-Dasar CSS & Layout Web

Selamat datang di dunia styling web! Di sini kamu akan belajar mempercantik dan menata halaman HTML-mu agar tampil menarik, rapi, dan nyaman digunakan siapa saja.

---

## 🗂️ Glossary Umum & Fungsi Tagline

| Istilah/Tagline         | Fungsi/Deskripsi                                                                                 | Contoh/Analogi                                    |
|------------------------|--------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Mendekorasi Profil     | Tema exercise: memperindah tampilan profil HTML dengan CSS dasar                                 | Seperti mendekorasi kamar atau buku harian        |
| Styling                | Proses mengatur tampilan (warna, font, layout) pada halaman web                                 | Mengecat dan menata ruangan                       |
| Selector               | Bagian CSS yang memilih elemen HTML untuk di-style                                              | Alamat rumah yang dituju tukang pos               |
| Responsive             | Tampilan web tetap bagus di HP & laptop                                                         | Baju yang muat di semua ukuran                    |
| Class                  | Nama kelompok elemen untuk styling bersama                                                      | Seragam kelompok                                 |
| ID                     | Identitas unik satu elemen                                                                      | Nomor induk siswa                                 |
| Property               | Sifat yang diatur di CSS (warna, ukuran, dsb)                                                   | Warna cat, ukuran meja                            |
| Value                  | Nilai dari property                                                                             | Biru, 16px, center                                |
| Layout                 | Cara menata posisi elemen di halaman                                                            | Menyusun furnitur di ruangan                      |

---

## 🎨 Apa Itu CSS?

**CSS (Cascading Style Sheets)** adalah bahasa yang digunakan untuk mendesain dan mengatur tampilan (style) elemen HTML di halaman web. CSS mengontrol warna, ukuran font, posisi elemen, jarak antar elemen, dan bahkan animasi!

### Analogi Sederhana:
- Kalau HTML adalah *tulang dan organ tubuh*, maka CSS adalah *pakaian dan gaya rambut*. Fungsinya tetap sama, tapi tampilannya bisa sangat berbeda.

---

## 🏷️ Tabel Property & Selector CSS Populer

| Property/Selector | Fungsi/Deskripsi                                      | Contoh Penggunaan                                  |
|------------------|-------------------------------------------------------|----------------------------------------------------|
| `color`          | Mengatur warna teks                                   | `color: blue;`                                     |
| `background`/`background-color` | Mengatur warna/ gambar latar belakang     | `background: #f4f4f4;`                             |
| `font-size`      | Ukuran huruf                                          | `font-size: 18px;`                                 |
| `font-family`    | Jenis huruf                                           | `font-family: Arial, sans-serif;`                  |
| `text-align`     | Perataan teks (kiri, kanan, tengah)                   | `text-align: center;`                              |
| `margin`         | Jarak luar elemen                                     | `margin: 20px;`                                    |
| `padding`        | Jarak dalam elemen                                    | `padding: 10px;`                                   |
| `border`         | Garis tepi elemen                                     | `border: 1px solid #ccc;`                          |
| `width`/`height` | Lebar/tinggi elemen                                  | `width: 100px; height: 50px;`                      |
| `display`        | Cara elemen ditampilkan (block, inline, flex, grid)   | `display: flex;`                                   |
| `flex`/`flex-direction`/`gap` | Layout fleksibel (Flexbox)                 | `display: flex; gap: 20px;`                        |
| `max-width`      | Lebar maksimum elemen                                 | `max-width: 600px;`                                |
| `box-shadow`     | Efek bayangan                                         | `box-shadow: 0 2px 8px #aaa;`                      |
| `:hover`         | Efek saat mouse diarahkan ke elemen                   | `a:hover { color: red; }`                          |
| `.class`         | Selector untuk elemen dengan class tertentu           | `.container { ... }`                               |
| `#id`            | Selector untuk elemen dengan id tertentu              | `#main-title { ... }`                              |

---

## 🧩 Fungsi CSS Populer di Exercise
- Membuat tampilan lebih menarik dan mudah dibaca
- Menata layout agar rapi (Flexbox, Grid)
- Membuat halaman responsive (bisa dibuka di HP/laptop)
- Memberi efek interaktif (hover, transisi warna)
- Menyembunyikan/menampilkan elemen

---

## 📐 Contoh Penggunaan CSS Praktis

### Mengubah warna dan font
```css
body {
  background: #f4f4f4;
  font-family: sans-serif;
}
```

### Menata judul dan paragraf
```css
h1 {
  color: #1976d2;
  text-align: center;
}
p {
  font-size: 16px;
  text-align: justify;
}
```

### Layout Flexbox
```css
.container {
  display: flex;
  gap: 20px;
}
```

### Responsive dengan max-width
```css
.container {
  max-width: 600px;
  margin: auto;
}
```

---

## 📖 Kenapa Ini Penting?
- CSS membuat web jadi menarik, mudah dibaca, dan nyaman digunakan
- Tanpa CSS, semua website akan terlihat polos dan membosankan
- CSS membantu web tampil baik di berbagai perangkat

---

## 🧠 Insight Tambahan
- Gunakan DevTools di browser untuk eksperimen styling secara langsung
- Flexbox dan Grid sangat membantu untuk layout modern
- Class bisa dipakai berkali-kali, id hanya untuk satu elemen unik
- Responsive = web tetap enak dilihat di HP, tablet, laptop

---

## 🔗 Referensi Tambahan
- [MDN – CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
- [CSS Tricks – Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [W3Schools – CSS Tutorial](https://www.w3schools.com/css/)
- [FreeCodeCamp – Responsive Web Design](https://www.freecodecamp.org/learn/responsive-web-design/)

### Video:
- [Traversy Media – CSS Crash Course](https://www.youtube.com/watch?v=yfoY53QXEnI)

---

## ✅ Tips untuk Kadet
- Jika warna tidak berubah, cek koneksi CSS di `<head>`
- Gunakan DevTools (klik kanan > Inspect) untuk eksperimen
- Mulai dari gaya minimalis, lalu eksplorasi
- Konsisten dalam penggunaan indentasi dan nama class
- Cek hasil di HP dan laptop

---

> "CSS bukan tentang menjadi cantik — tapi membuat web bisa dibaca, nyaman, dan bermakna." 💅

