# 🌐 FUNDAMENTAL – Pengenalan HTTP & API untuk Semua Kalangan

Selamat datang di dunia backend! Di sini kamu akan belajar pondasi utama: bagaimana komputer saling "berkirim surat" lewat internet, dan bagaimana kamu bisa membuat "pelayan digital" (API) yang siap membantu siapa saja.

---

## 📖 Cerita/Analogi Awal

> **Bayangkan kamu mengirim surat ke teman.**
> Kamu menulis alamat, isi pesan, dan menunggu balasan. Di dunia web, browser (kamu) mengirim “surat” ke server (teman) lewat “pak pos” bernama HTTP. API adalah pelayan yang memastikan suratmu sampai ke dapur yang tepat dan membawakan balasan ke meja kamu.

---

## 🎯 Tujuan Belajar

Setelah mempelajari materi ini, kamu akan:
- Memahami cara kerja HTTP & API dengan analogi surat menyurat
- Tahu apa itu request, response, endpoint, dan status code
- Bisa membaca dan membuat contoh request/response sederhana
- Siap membangun server kecil yang bisa membalas “surat” dari client

---

## 🗂️ Glossary & Fungsi Penting

| Istilah/Fungsi | Penjelasan Sederhana | Analogi/Contoh |
|----------------|----------------------|----------------|
| HTTP           | Protokol kirim pesan | Pak pos        |
| API            | Jembatan komunikasi  | Pelayan restoran|
| Endpoint       | Alamat tujuan surat  | Meja di restoran|
| Request        | Surat yang dikirim   | Surat ke teman  |
| Response       | Balasan surat        | Balasan teman   |
| Status Code    | Kode pos hasil surat | 200 = sukses, 404 = alamat tidak ditemukan |
| Header         | Sampul surat         | Tulis “Rahasia” di amplop |
| Body           | Isi surat/data       | Isi pesan      |

---

## 🧠 Apa Itu HTTP?

**HTTP (Hypertext Transfer Protocol)** adalah aturan standar agar komputer bisa saling mengirim dan menerima pesan lewat internet.

Setiap kali kamu:
- Membuka halaman website
- Login ke aplikasi
- Submit form
... kamu sedang menggunakan HTTP.

### Struktur HTTP (Surat Digital)

| Komponen | Deskripsi                                    | Analogi                  |
| -------- | -------------------------------------------- |--------------------------|
| Request  | Permintaan yang dikirim client ke server     | Surat yang kamu kirim    |
| Response | Balasan dari server untuk client             | Surat balasan dari teman |
| Method   | Jenis aksi yang diminta (`GET`, `POST`, dll) | Jenis permintaan: ambil info, kirim data |
| Header   | Metadata (format, status, izin, dll)         | Sampul surat, catatan di amplop |
| Body     | Isi data yang dikirim (biasanya JSON)        | Isi pesan di dalam surat |

---

## 🧩 Apa Itu API?

**API (Application Programming Interface)** adalah pelayan digital yang menghubungkan aplikasi satu dengan lainnya. API menerima permintaan (request), meneruskan ke dapur (server), lalu mengantarkan hasilnya (response) ke pemesan (client).

> 🔁 **Analogi:** API = pelayan restoran. Kamu (client) minta makanan (data), dapur (server) menyiapkan, lalu pelayan (API) mengantarkan balik ke meja kamu.

---

## 🔧 HTTP Methods (Jenis Permintaan)

| Method | Tujuan Umum        | Contoh                         | Analogi                |
| ------ | ------------------ | ------------------------------ |------------------------|
| GET    | Mengambil data     | `GET /users`                   | Minta daftar menu      |
| POST   | Mengirim data baru | `POST /users` dengan JSON body | Kirim pesanan baru     |
| PUT    | Memperbarui data   | `PUT /users/123`               | Ubah pesanan           |
| DELETE | Menghapus data     | `DELETE /users/123`            | Batalkan pesanan       |

---

## 📬 Contoh Request & Response (Surat Digital)

**Contoh Request:**
```json
POST /data HTTP/1.1
Content-Type: application/json

{
  "name": "Raka",
  "email": "raka@link.id"
}
```

**Contoh Response:**
```json
{
  "message": "Data berhasil diterima!"
}
```

---

## 🧪 Apa Itu Status Code?

Status code = kode pos hasil surat. Memberi tahu apakah permintaanmu sukses, gagal, atau salah alamat.

| Kode | Arti         | Penjelasan Singkat               | Analogi                  |
| ---- | ------------ | -------------------------------- |--------------------------|
| 200  | OK           | Permintaan berhasil              | Surat dibalas dengan baik|
| 201  | Created      | Data baru berhasil dibuat        | Pesanan baru diterima    |
| 400  | Bad Request  | Format data salah / tidak valid  | Suratmu tidak jelas      |
| 404  | Not Found    | Endpoint tidak ditemukan         | Alamat surat tidak ada   |
| 500  | Server Error | Terjadi kesalahan di sisi server | Dapur restoran error     |

---

## 🔧 Node.js HTTP Module (Membuat Pelayan Digital)

Node.js punya module bawaan (`http`) untuk membuat server dasar. Ini seperti membuat pelayan digital yang siap menerima dan membalas surat:

```js
const http = require('http');

const server = http.createServer((req, res) => {
  if (req.url === '/hello' && req.method === 'GET') {
    res.writeHead(200, { 'Content-Type': 'application/json' });
    res.end(JSON.stringify({ message: 'Hello World' }));
  }
});

server.listen(3000, () => {
  console.log('Server aktif di http://localhost:3000');
});
```

---

## 🛠️ Tips Pro & Troubleshooting
- Jika request gagal, cek URL dan method (GET/POST).
- Selalu cek status code di response.
- Gunakan `console.log()` untuk melihat data yang masuk ke server.
- Jika server tidak jalan, pastikan port belum dipakai aplikasi lain.
- Coba kirim request pakai Postman (simulasi mengirim surat).

---

## 📦 Preview Output

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

## 🔗 Referensi Belajar
- [MDN - HTTP Basics](https://developer.mozilla.org/en-US/docs/Web/HTTP)
- [Node.js HTTP Module](https://nodejs.org/api/http.html)
- [Postman API Testing](https://learning.postman.com/)

---

> “Belajar backend itu seperti belajar mengirim surat: mulai dari menulis alamat, isi pesan, sampai memastikan balasan diterima. Nikmati prosesnya, jangan takut salah alamat!”

