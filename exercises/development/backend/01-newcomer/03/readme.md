# 📝 Exercise 03: Buku Tamu Komunitas – Routing & File System Sederhana

> **Track**: Development  
> **Specialty**: Backend  
> **Level**: 🌱 Newcomer  
> **Estimated Time**: 1.5–2.5 jam  
> **Last Updated**: Juni 2025

---

## 🧰 Tools yang Digunakan

| Alat      | Keterangan                                 |
|-----------|--------------------------------------------|
| Node.js   | Menjalankan kode JavaScript di backend     |
| VS Code   | Editor kode dengan integrasi terminal      |
| Terminal  | Menjalankan perintah CLI & server          |
| Postman   | Menguji dan mengirim request ke API        |
| curl      | Alternatif Postman untuk test API di CLI   |

---

## ✅ Checklist Goal Exercise

- [ ] Membuat server dengan Node.js (tanpa framework)
- [ ] Endpoint `GET /users` membaca dan menampilkan data dari file JSON
- [ ] Endpoint `POST /users` menerima data dan menyimpan ke file JSON
- [ ] Validasi data (harus lengkap)
- [ ] Menggunakan status code yang sesuai (201, 400)
- [ ] (Bonus) ID unik untuk setiap user
- [ ] (Bonus) Log request ke `log.txt`

---

## 📖 Studi Kasus: Buku Tamu Digital Komunitas

Kamu membuat **buku tamu digital** untuk komunitas. Setiap tamu bisa dilihat (GET /users) dan ditambah (POST /users). Data disimpan di file `data.json`. Seperti resepsionis yang mencatat dan menampilkan daftar tamu!

---

## 🎯 Goal Latihan

Setelah latihan ini, kamu akan:
- Memahami konsep routing manual di Node.js
- Bisa mengelola data sederhana dengan file JSON
- Membuat server yang bisa menerima dan menampilkan data
- Siap membangun backend tanpa framework

---

## 📋 Checklist Langkah

1. **Buat folder project dan file utama:**
   ```bash
   mkdir buku-tamu-komunitas
   cd buku-tamu-komunitas
   npm init -y
   touch server.js data.json
   ```
2. **Buat server dengan Node.js (tanpa framework)**
3. **Endpoint `GET /users`**
   - Baca dan tampilkan isi `data.json` sebagai JSON
4. **Endpoint `POST /users`**
   - Terima data `{ name, hobby }`, simpan ke `data.json`
   - Validasi: data harus lengkap
   - Balas dengan status code yang sesuai (201 untuk sukses, 400 untuk error)
5. **(Bonus) Tambahkan ID unik untuk setiap user**
6. **(Bonus) Tambahkan log request ke `log.txt`**

---

## 🗂️ Struktur File Disarankan

```
buku-tamu-komunitas/
├── server.js
├── data.json
├── log.txt         ← (bonus)
├── README.md
└── fundamental.md
```

---

## 🧪 Contoh Output & Data

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

## 💡 Tips Pro & Troubleshooting
- Jika data tidak tersimpan, cek path dan format JSON
- Gunakan try-catch untuk error handling file
- Cek status code di response
- Gunakan Postman/curl untuk test endpoint

---

## 🔗 Referensi
- [Node.js File System](https://nodejs.org/api/fs.html)
- [MDN JSON](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
- [HTTP Request Handling in Node.js](https://www.digitalocean.com/community/tutorials/)

---

> "Routing itu seperti resepsionis kantor: setiap permintaan diarahkan ke ruangan yang tepat. Data di file = catatan tamu yang selalu bisa dibuka kembali!"

