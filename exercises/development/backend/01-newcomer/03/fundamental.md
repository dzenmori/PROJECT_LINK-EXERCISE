# 🌐 FUNDAMENTAL – Routing Manual & File System di Node.js

Selamat datang di dunia routing dan file system! Di sini kamu akan belajar bagaimana server "menyambut tamu" (request) dan "menyimpan catatan" (data) di file, seperti resepsionis kantor yang mencatat setiap tamu yang datang.

---

## 📖 Cerita/Analogi Awal

> **Bayangkan kamu jadi resepsionis kantor.**
> Setiap tamu datang, kamu tanya nama dan tujuan, lalu catat di buku tamu. Routing adalah proses mengarahkan tamu ke ruangan yang tepat, file system adalah buku catatan tamu.

---

## 🎯 Tujuan Belajar

Setelah mempelajari materi ini, kamu akan:
- Memahami konsep routing manual di Node.js
- Bisa mengelola data sederhana dengan file JSON
- Membuat server yang bisa menerima dan menampilkan data
- Siap membangun backend tanpa framework

---

## 🗂️ Glossary & Fungsi Penting

| Istilah/Fungsi | Penjelasan Sederhana | Analogi/Contoh |
|---------------|----------------------|----------------|
| Routing       | Mengarahkan request ke handler | Resepsionis kantor |
| Endpoint      | Alamat tujuan request | Ruangan kantor |
| fs            | Modul untuk baca/tulis file | Buku catatan tamu |
| JSON          | Format data sederhana | Daftar tamu di buku |
| Status code   | Kode hasil request    | Stempel di buku tamu |
| Handler       | Fungsi penjawab request | Petugas di ruangan |

---

## 🔀 Apa Itu Routing?

**Routing** adalah proses menangani permintaan HTTP berdasarkan URL dan method-nya. Tujuannya agar server bisa membedakan:
- Permintaan `GET /users`
- vs `POST /users`
- vs `GET /users/123`

> 📬 Anggap routing seperti resepsionis yang menyaring setiap tamu (request) untuk diarahkan ke ruangan (handler) yang sesuai.

---

## 🏷️ Tabel Fungsi Routing & File System

| Fungsi/Method         | Kegunaan & Contoh |
|----------------------|-------------------|
| `req.url`/`req.method` | Cek alamat dan jenis request. <br> `if (req.url === '/users' && req.method === 'GET')` |
| `fs.readFileSync()`  | Baca isi file. <br> `fs.readFileSync('data.json')` |
| `fs.writeFileSync()` | Simpan data ke file. <br> `fs.writeFileSync('data.json', data)` |
| `JSON.parse()`       | Ubah string ke array/object. <br> `JSON.parse(data)` |
| `JSON.stringify()`   | Ubah array/object ke string. <br> `JSON.stringify(data)` |

---

## 📞 Contoh Step-by-Step Routing & File

### 1. Routing Manual
```js
if (req.url === '/users' && req.method === 'GET') {
  // logic baca file & kirim data
}
```

### 2. Menangani JSON Body (POST)
```js
let body = '';
req.on('data', chunk => (body += chunk));
req.on('end', () => {
  const data = JSON.parse(body);
  // lanjut simpan ke file
});
```

### 3. Baca & Simpan Data ke File
```js
const fs = require('fs');
const users = JSON.parse(fs.readFileSync('data.json'));
users.push({ name: 'Raka', hobby: 'Backend' });
fs.writeFileSync('data.json', JSON.stringify(users));
```

---

## 💡 Tips Pro & Troubleshooting
- Jika data tidak tersimpan, cek path dan format JSON
- Gunakan try-catch untuk error handling file
- Cek status code di response
- Gunakan Postman/curl untuk test endpoint
- Jika file tidak ada, buat default `[]`

---

## 📦 Preview Output

**Contoh data di `data.json`:**
```json
[
  { "id": 1, "name": "Raka", "hobby": "Backend" }
]
```
**Tampilan di terminal:**
```
User baru: Raka (Backend)
```

---

## 🔗 Referensi Routing & File System
- [Node.js File System](https://nodejs.org/api/fs.html)
- [MDN JSON](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
- [HTTP Request Handling in Node.js](https://www.digitalocean.com/community/tutorials/)

---

> "Routing itu seperti resepsionis kantor: setiap permintaan diarahkan ke ruangan yang tepat. Data di file = catatan tamu yang selalu bisa dibuka kembali!"

