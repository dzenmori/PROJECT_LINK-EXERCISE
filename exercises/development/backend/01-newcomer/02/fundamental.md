# 🌐 FUNDAMENTAL – CLI & Input/Output (I/O) dengan Node.js

Selamat datang di dunia Command Line Interface (CLI)! Di sini kamu akan belajar bagaimana "ngobrol langsung dengan komputer" lewat terminal, seperti panitia acara yang mencatat tamu satu per satu dengan cepat dan efisien.

---

## 📖 Cerita/Analogi Awal

> **Bayangkan kamu jadi panitia pendaftaran acara keluarga.**
> Kamu bertanya nama, umur, dan minat setiap tamu, lalu mencatatnya di buku. CLI adalah cara komputer melakukan hal yang sama—tapi lewat teks di terminal!

---

## 🎯 Tujuan Belajar

Setelah mempelajari materi ini, kamu akan:
- Memahami konsep CLI dan input/output di Node.js
- Bisa membuat program yang menerima input dari pengguna
- Menyimpan dan menampilkan data di terminal
- Siap membangun tool CLI sederhana untuk kebutuhan apapun

---

## 🗂️ Glossary & Fungsi Penting

| Istilah/Fungsi | Penjelasan Sederhana | Analogi/Contoh |
|---------------|----------------------|----------------|
| CLI           | Antarmuka teks untuk perintah | Ngobrol langsung dengan komputer |
| Argumen       | Data tambahan saat menjalankan program | Catatan di kertas pendaftaran |
| process.argv  | Array argumen di Node.js | Daftar jawaban dari peserta |
| readline      | Modul untuk tanya-jawab interaktif | Panitia bertanya langsung |
| fs            | Modul untuk baca/tulis file | Buku catatan tamu |
| Output        | Hasil yang ditampilkan | Resume pendaftaran di papan |

---

## 🧠 Apa Itu CLI?

**CLI (Command Line Interface)** adalah antarmuka berbasis teks di mana pengguna mengetik perintah untuk menjalankan program.

> 💬 CLI ≈ ngobrol langsung dengan komputer pakai teks, bukan klik tombol.

### Contoh CLI tools di dunia nyata:
- `npm` → mengelola package
- `git` → version control
- `node` → menjalankan file JavaScript

---

## 📥 Jenis Input di CLI

| Jenis Input                | Contoh                  | Modul Node.js yang Digunakan |
| -------------------------- | ----------------------- | ---------------------------- |
| **Argumen baris perintah** | `node app.js --lang=id` | `process.argv`               |
| **Input interaktif**       | Prompt: "Nama Anda?"    | `readline`                   |

---

## ✍️ Tabel Fungsi Penting CLI Node.js

| Fungsi/Method         | Kegunaan & Contoh |
|----------------------|-------------------|
| `process.argv`       | Ambil argumen dari command line. <br> `node app.js --lang=id` → `process.argv[2]` = '--lang=id' |
| `readline.question()`| Tanya pengguna di terminal. <br> `rl.question('Nama?', cb)` |
| `fs.writeFileSync()` | Simpan data ke file. <br> `fs.writeFileSync('hasil.txt', data)` |
| `console.log()`      | Tampilkan output ke terminal. <br> `console.log('Halo!')` |

---

## 📞 Contoh Step-by-Step CLI

### 1. Menangkap Argumen
```js
const args = process.argv.slice(2);
console.log('Argumen:', args);
```

### 2. Input Interaktif
```js
const readline = require('readline');
const rl = readline.createInterface({ input: process.stdin, output: process.stdout });
rl.question('Nama kamu siapa? ', (jawaban) => {
  console.log(`Halo, ${jawaban}!`);
  rl.close();
});
```

### 3. Menyimpan ke File
```js
const fs = require('fs');
fs.writeFileSync('output.txt', 'Isi yang ingin disimpan');
```

---

## 💡 Tips Pro & Troubleshooting
- Jika CLI tidak jalan, cek penulisan kode dan jalankan dengan `node namafile.js`
- Gunakan `console.log()` untuk debug
- Untuk argumen, cek dengan `process.argv`
- Jika file tidak tersimpan, cek path dan permission
- Cek hasil file dengan `cat result.txt` atau buka di editor

---

## 📦 Preview Output

```
📋 Resume:
Nama  : Raka
Umur  : 22
Minat : Backend
```

---

## 🔗 Referensi CLI Node.js
- [Node.js readline module](https://nodejs.org/api/readline.html)
- [Command Line Arguments – Node.js Docs](https://nodejs.org/en/learn/getting-started/how-to-parse-command-line-arguments/)
- [Zellwk CLI tutorial](https://zellwk.com/blog/cli/)

---

> "CLI itu seperti ngobrol langsung dengan komputer. Semakin sering latihan, semakin luwes kamu mengendalikan sistem!"

