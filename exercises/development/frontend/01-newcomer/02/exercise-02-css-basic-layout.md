# 🧪 Exercise 02: CSS Basic Layout

## 📖 Cerita: Mendekorasi Kartu Profilmu

Setelah membuat kartu nama digital, sekarang saatnya mendekorasi agar lebih menarik! Bayangkan kamu sedang menata kamar atau mendekorasi buku harianmu. Dengan CSS, kamu bisa mengubah warna, font, dan tata letak halaman profilmu agar lebih keren dan nyaman dilihat.

## 🎯 Tujuan

Setelah latihan ini, kamu akan:
- Menghubungkan file CSS ke HTML
- Mengubah tampilan halaman web (warna, font, layout)
- Mengenal konsep dasar layout dengan Flexbox

## 📚 Prasyarat

- Sudah menyelesaikan Exercise 01 (HTML Introduction)

## 🛠 Tools

- Browser
- CodePen / JSFiddle / Replit
- (Opsional) VS Code + Live Server

## 📦 File yang Harus Dibuat

- `index.html`
- `style.css`

## 📋 Instruksi Langkah demi Langkah

1. **Buka kembali file `index.html` dari latihan sebelumnya.**
2. **Buat file baru bernama `style.css` di folder yang sama.**
3. **Hubungkan file CSS ke HTML dengan menambahkan baris berikut di dalam tag `<head>`:**

```html
<link rel="stylesheet" href="style.css" />
```

4. **Ubah tampilan halaman dengan aturan CSS berikut (tulis di `style.css`):**
   - Ubah font seluruh halaman menjadi sans-serif:
     ```css
     body {
       font-family: sans-serif;
     }
     ```
   - Atur background halaman jadi warna cerah (misal: #f4f4f4):
     ```css
     body {
       background: #f4f4f4;
     }
     ```
   - Heading `<h1>` berwarna biru dan rata tengah:
     ```css
     h1 {
       color: #1976d2;
       text-align: center;
     }
     ```
   - Paragraf `<p>` berukuran 16px dan rata kiri-kanan:
     ```css
     p {
       font-size: 16px;
       text-align: justify;
     }
     ```
   - Buat konten lebih terpusat dengan lebar maksimal 600px dan margin auto:
     ```css
     .container {
       max-width: 600px;
       margin: auto;
     }
     ```

5. **Jika kamu punya gambar dan list hobi, bungkus dengan `<div class="container">` di HTML.**
6. **Gunakan Flexbox untuk menata gambar dan list hobi secara horizontal:**
   ```css
   .container {
     display: flex;
     gap: 20px;
   }
   ```
7. **Eksplorasi padding, margin, dan border untuk elemen utama.**

## 🧠 Bonus Challenge (Opsional)

- Buat dark mode alternatif menggunakan class `.dark`
- Tambahkan efek hover pada link

## ✅ Checklist

- [ ] File `style.css` sudah dibuat
- [ ] File CSS sudah terhubung ke HTML
- [ ] Warna background berubah
- [ ] Heading `<h1>` berwarna biru dan center
- [ ] Paragraf `<p>` berukuran 16px dan justify
- [ ] Konten terpusat dengan max-width
- [ ] Gambar dan list hobi (jika ada) tersusun horizontal dengan Flexbox

## 📌 Contoh Preview

*(Tampilkan preview sederhana, misal:)*

```
+-----------------------------+
|        Nama Kamu            |
|  [Foto]   [List Hobi]       |
|  Saya suka belajar...       |
+-----------------------------+
```

## 📥 Penyerahan

Fork repositori ini, buat folder `frontend/newcomer/[namamu]-css-layout/` dan masukkan `index.html` dan `style.css`

## 🙋 Tips & Troubleshooting

- Jika warna tidak berubah, pastikan file `style.css` sudah terhubung dengan benar di `<head>`.
- Jika layout Flexbox tidak berfungsi, cek penulisan class dan pastikan elemen dibungkus dengan `<div class="container">`.
- Gunakan DevTools di browser (klik kanan > Inspect) untuk eksperimen styling.
- Tanya mentor jika layout-nya kacau atau bingung!

---

> "CSS bukan hanya tentang estetika, tapi komunikasi visual yang efisien. Mulai dari yang sederhana, lalu eksplorasi!"

