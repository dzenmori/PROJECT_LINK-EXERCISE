# 🧪 Exercise 03: JavaScript Basic Interaction

## 📖 Cerita: Kartu Profil Interaktif

Bayangkan halaman profilmu bisa menyapa pengunjung atau berubah warna saat tombol ditekan, seperti kartu ucapan digital yang bisa "hidup"! Di latihan ini, kamu akan belajar membuat halaman web yang bisa merespon aksi pengguna dengan JavaScript.

## 🎯 Tujuan

Setelah latihan ini, kamu akan:
- Menghubungkan file JavaScript ke HTML
- Membuat tombol yang bisa mengubah tampilan halaman
- Membuat halaman web yang bisa menyapa pengunjung secara interaktif

## 📚 Prasyarat

- Sudah menyelesaikan HTML dan CSS dasar

## 🛠 Tools

- Browser
- CodePen / JSFiddle / Replit
- (Opsional) VS Code + Live Server

## 📦 File yang Harus Dibuat

- `index.html`
- `style.css`
- `script.js`

## 📋 Instruksi Langkah demi Langkah

1. **Gunakan kembali file HTML dan CSS dari latihan sebelumnya.**
2. **Tambahkan tombol di bawah deskripsi pada HTML:**
   ```html
   <button id="changeColorBtn">Ubah Warna Background</button>
   ```
3. **Buat file baru bernama `script.js` di folder yang sama.**
4. **Hubungkan file JavaScript ke HTML, letakkan sebelum tag `</body>`:**
   ```html
   <script src="script.js"></script>
   ```
5. **Salin kode berikut ke dalam `script.js`:**
   ```js
   document.getElementById("changeColorBtn").onclick = function() {
     const colors = ["#f4f4f4", "#e0f7fa", "#ffebee", "#f3e5f5"];
     const chosen = colors[Math.floor(Math.random() * colors.length)];
     document.body.style.backgroundColor = chosen;
     alert("Background diubah!");
   };
   ```
6. **Tambahkan input nama dan tombol submit di HTML:**
   ```html
   <input type="text" id="namaInput" placeholder="Masukkan namamu" />
   <button id="greetBtn">Sapa Saya!</button>
   <div id="greetResult"></div>
   ```
7. **Tambahkan kode berikut ke `script.js` untuk menyapa pengguna:**
   ```js
   document.getElementById("greetBtn").onclick = function() {
     const nama = document.getElementById("namaInput").value;
     document.getElementById("greetResult").innerText = "Halo, " + nama + "!";
   };
   ```
8. **Simpan semua file, lalu buka `index.html` di browser dan coba fitur interaktifnya!**

## 💡 Bonus Challenge (Opsional)

- Tambahkan jam digital yang real-time (`setInterval` + `Date()`)
- Buat toggle antara light/dark mode

## ✅ Checklist

- [ ] File `script.js` sudah dibuat
- [ ] Tombol "Ubah Warna Background" berfungsi
- [ ] Input nama dan tombol "Sapa Saya!" berfungsi
- [ ] Hasil sapaan muncul di halaman
- [ ] Semua file sudah terhubung dan dicoba di browser

## 📌 Contoh Preview

*(Tampilkan preview sederhana, misal:)*

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

## 📥 Penyerahan

Folder: `submissions/frontend/newcomer/[namamu]-js-interaction/`

## 🙋 Tips & Troubleshooting

- Jika tombol tidak berfungsi, pastikan file `script.js` sudah terhubung di HTML.
- Jika muncul error, cek penulisan `id` pada elemen HTML dan di JavaScript.
- Gunakan `console.log()` di `script.js` untuk membantu debugging (buka Console di browser: Ctrl+Shift+I).
- Jangan ragu bertanya jika bingung!

---

> "JavaScript memberi nyawa pada halaman webmu. Mulai dari interaksi sederhana, lalu eksplor tanpa batas!" ⚡

