# 📝 Exercise 01: Buku Tamu Digital – Belajar HTTP & API dari Nol

> **Track**: Development  
> **Specialty**: Backend  
> **Level**: 🌱 Newcomer  
> **Estimated Time**: 1–2 jam  
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

- [ ] Membuat server dengan module `http` dari Node.js
- [ ] Endpoint `GET /hello` membalas dengan pesan JSON
- [ ] Endpoint `POST /data` menerima data tamu dan tampilkan di terminal
- [ ] Mengirim response JSON dan status code yang sesuai (200, 201, 400)
- [ ] Menggunakan header `Content-Type: application/json`
- [ ] Mengetes endpoint dengan Postman/curl

---

## 📖 Studi Kasus: Buku Tamu Digital Keluarga

Bayangkan kamu diminta membuat **buku tamu digital** untuk acara keluarga. Setiap tamu bisa menyapa lewat endpoint `/hello` dan mengisi data diri lewat endpoint `/data`. Data yang masuk akan tampil di terminal, seperti buku tamu di meja resepsionis.

---

## 🎯 Goal Latihan

Setelah latihan ini, kamu akan:
- Memahami cara kerja HTTP & API dengan analogi surat menyurat
- Bisa membuat server sederhana yang membalas “surat” (request) dengan “pesan” (response)
- Mengenal status code (kode pos surat) dan cara mengirim data
- Siap membangun pondasi backend untuk project apapun

---

## 📋 Checklist Langkah

1. **Buat folder project dan file server:**
   ```bash
   mkdir buku-tamu-digital
   cd buku-tamu-digital
   npm init -y
   touch server.js
   ```
2. **Buat server dengan module `http` dari Node.js**
3. **Buat endpoint `GET /hello`**
   - Jika diakses, balas dengan JSON: `{ "message": "Selamat datang di Buku Tamu Digital!" }`
4. **Buat endpoint `POST /data`**
   - Terima data tamu (nama, email) dalam format JSON
   - Tampilkan data tamu di terminal (pakai `console.log`)
   - Balas dengan JSON: `{ "message": "Data berhasil diterima!" }`
   - Jika data tidak lengkap, balas dengan status 400 dan pesan error
5. **Gunakan header `Content-Type: application/json`**
6. **Gunakan status code yang sesuai:**
   - 200 untuk sukses
   - 201 untuk data baru
   - 400 untuk data salah
7. **Tes endpoint pakai Postman atau curl**

---

## 🗂️ Struktur File Disarankan

```
buku-tamu-digital/
├── server.js
├── README.md
└── fundamental.md
```

---

## 🧪 Contoh Request & Output

**Contoh request:**
```json
POST /data
{
  "name": "Budi",
  "email": "budi@keluarga.id"
}
```
**Contoh response:**
```json
{
  "message": "Data berhasil diterima!"
}
```
**Tampilan di terminal:**
```
Tamu baru: Budi (budi@keluarga.id)
```

---

## 💡 Tips Pro & Troubleshooting
- Jika request gagal, cek URL dan method (GET/POST)
- Selalu cek status code di response
- Gunakan `console.log()` untuk melihat data yang masuk ke server
- Jika server tidak jalan, pastikan port belum dipakai aplikasi lain
- Coba kirim request pakai Postman (simulasi mengirim surat)

---

## 🔗 Referensi
- [Node.js HTTP module](https://nodejs.org/api/http.html)
- [MDN - HTTP Overview](https://developer.mozilla.org/en-US/docs/Web/HTTP)
- [Postman Docs](https://learning.postman.com/)

---

> "REST API itu seperti buku tamu digital: kamu mengisi data, server menyimpan, dan semua orang bisa saling terhubung. Mulai dari sini, kamu siap membangun backend apapun!"

