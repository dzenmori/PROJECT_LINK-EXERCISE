# 📝 Exercise 04: Server Modular – Backend Rapi & Siap Kolaborasi

> **Track**: Development  
> **Specialty**: Backend  
> **Level**: 🌱 Newcomer  
> **Estimated Time**: 2–3 jam  
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

- [ ] Membuat struktur folder modular (server, routes, controllers, utils, data)
- [ ] Memisahkan logic route, controller, dan helper
- [ ] Endpoint `GET /notes` dan `POST /notes` berjalan
- [ ] Menggunakan module.exports dan require
- [ ] Validasi data dan status code
- [ ] (Bonus) DELETE /notes/:id
- [ ] (Bonus) Logger ke log.txt

---

## 📖 Studi Kasus: Server Kolaborasi Tim

Kamu dan tim ingin membuat server yang mudah dikembangkan bersama. Kode harus dipisah: server utama, route, controller, utils, dan data. Seperti dapur restoran yang punya chef spesialis di setiap bagian!

---

## 🎯 Goal Latihan

Setelah latihan ini, kamu akan:
- Memahami pentingnya modularisasi di backend
- Bisa memecah kode menjadi bagian-bagian kecil yang jelas tugasnya
- Membuat server yang mudah dikembangkan dan di-maintain
- Siap berkolaborasi di tim backend

---

## 📋 Checklist Langkah

1. **Buat struktur folder modular:**
   ```bash
   mkdir server-modular
   cd server-modular
   npm init -y
   mkdir routes controllers utils data
   touch server.js routes/notes.js controllers/notesController.js utils/file.js data/notes.json
   ```
2. **Pisahkan logic route, controller, dan file helper**
3. **Endpoint `GET /notes` dan `POST /notes` (tambah catatan)**
4. **Gunakan module.exports dan require**
5. **Validasi data dan status code**
6. **(Bonus) Tambahkan `DELETE /notes/:id`**
7. **(Bonus) Tambahkan logger ke `log.txt`**

---

## 🗂️ Struktur Folder Disarankan

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
├── log.txt (bonus)
├── README.md
└── fundamental.md
```

---

## 🧪 Contoh Output & Struktur

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

## 💡 Tips Pro & Troubleshooting
- Jika ada error “module not found”, cek path require
- Pisahkan fungsi sesuai tanggung jawab, jangan semua di satu file
- Gunakan nama folder yang konsisten (`routes`, `controllers`, `utils`)
- Cek hasil di Postman/curl

---

## 🔗 Referensi
- [Node.js Modules](https://nodejs.org/api/modules.html)
- [Zellwk - Structure for Beginners](https://zellwk.com/blog/structure-node-js/)
- [Modular Node.js Project Pattern](https://dev.to/)

---

> "Server modular itu seperti dapur restoran: setiap chef punya tugas jelas, hasilnya rapi dan mudah dikembangkan bersama!"

