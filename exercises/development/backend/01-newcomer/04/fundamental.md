# 🌐 FUNDAMENTAL – Modularisasi Server Node.js

Selamat datang di dunia modularisasi backend! Di sini kamu akan belajar bagaimana membagi kode menjadi bagian-bagian kecil yang jelas tugasnya, seperti dapur restoran yang punya chef spesialis di setiap bagian.

---

## 📖 Cerita/Analogi Awal

> **Bayangkan kamu bekerja di dapur restoran besar.**
> Setiap chef punya tugas: ada yang khusus masak, ada yang khusus plating, ada yang khusus cuci piring. Modularisasi di backend = membagi kode sesuai keahlian, supaya dapur (server) tetap rapi dan efisien.

---

## 🎯 Tujuan Belajar

Setelah mempelajari materi ini, kamu akan:
- Memahami pentingnya modularisasi di backend
- Bisa memecah kode menjadi bagian-bagian kecil yang jelas tugasnya
- Membuat server yang mudah dikembangkan dan di-maintain
- Siap berkolaborasi di tim backend

---

## 🗂️ Glossary & Fungsi Penting

| Istilah/Fungsi | Penjelasan Sederhana | Analogi/Contoh |
|---------------|----------------------|----------------|
| Modularisasi  | Membagi kode jadi bagian kecil | Chef spesialis di dapur |
| Module        | File/fungsi terpisah yang bisa dipakai ulang | Resep masakan |
| require()     | Memanggil module lain | Meminta chef lain bantu |
| module.exports| Mengekspor fungsi/module | Membagikan resep ke chef lain |
| Controller    | Tempat logic utama    | Chef kepala |
| Route         | Tempat pemetaan URL   | Buku pesanan |
| Utils         | Fungsi bantu          | Alat dapur |
| Data          | Tempat simpan data    | Lemari bahan makanan |

---

## 🧱 Prinsip Dasar Modularisasi di Node.js

### 🔹 1. Entry Point
File utama tempat server dijalankan: `server.js`

### 🔹 2. Routes
Menangani pemetaan URL ke handler: `routes/notes.js`

### 🔹 3. Controllers
Berisi logic utama atau "business logic": `controllers/notesController.js`

### 🔹 4. Utils / Helpers
Fungsi bantu seperti membaca file, validasi: `utils/file.js`

### 🔹 5. Data
Penyimpanan (sementara): `data/notes.json`

---

## 🏷️ Tabel Fungsi Modularisasi Node.js

| Fungsi/Method         | Kegunaan & Contoh |
|----------------------|-------------------|
| `require()`          | Memanggil module lain. <br> `const notes = require('./routes/notes')` |
| `module.exports`     | Mengekspor fungsi/module. <br> `module.exports = notesRouter` |
| Struktur folder      | Memisahkan file sesuai tugas. <br> `routes/`, `controllers/`, `utils/`, `data/` |

---

## 📞 Contoh Step-by-Step Modularisasi

### 1. Membuat Struktur Modular
```
server-modular/
├── server.js
├── routes/
│   └── notes.js
├── controllers/
│   └── notesController.js
├── utils/
│   └── file.js
├── data/
│   └── notes.json
```

### 2. Contoh Routing Modular
```js
// routes/notes.js
const { getNotes, addNote } = require('../controllers/notesController');
function notesRouter(req, res) {
  if (req.url === '/notes' && req.method === 'GET') return getNotes(req, res);
  if (req.url === '/notes' && req.method === 'POST') return addNote(req, res);
}
module.exports = notesRouter;
```

### 3. Menggunakan di server.js
```js
const http = require('http');
const notesRouter = require('./routes/notes');
const server = http.createServer((req, res) => {
  notesRouter(req, res);
});
server.listen(3000);
```

---

## 💡 Tips Pro & Troubleshooting
- Jika ada error “module not found”, cek path require
- Pisahkan fungsi sesuai tanggung jawab, jangan semua di satu file
- Gunakan nama folder yang konsisten (`routes`, `controllers`, `utils`)
- Dokumentasikan fungsi jika perlu (`README.md`, komentar)
- Cek hasil di Postman/curl

---

## 📦 Preview Output & Struktur

- **GET /notes** → tampilkan semua catatan dari notes.json
- **POST /notes** → tambah catatan baru

**Struktur folder:**
```
├── server.js
├── routes/
├── controllers/
├── utils/
├── data/
```

---

## 🔗 Referensi Modularisasi
- [Node.js Modules](https://nodejs.org/api/modules.html)
- [Zellwk - Structure for Beginners](https://zellwk.com/blog/structure-node-js/)
- [Modular Node.js Project Pattern](https://dev.to/)

---

> "Server modular itu seperti dapur restoran: setiap chef punya tugas jelas, hasilnya rapi dan mudah dikembangkan bersama!"

