# 📝 Exercise 02: Asisten Pendaftaran CLI – Belajar Input/Output dari Nol

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

---

## ✅ Checklist Goal Exercise

- [ ] Program CLI menyapa pengguna di terminal
- [ ] Menerima input nama, umur, minat (readline)
- [ ] Validasi input (nama tidak kosong, umur angka)
- [ ] Menampilkan resume pendaftaran di terminal
- [ ] (Bonus) Simpan hasil ke file `result.txt`
- [ ] (Bonus) Argumen `--lang` untuk bahasa

---

## 📖 Studi Kasus: Asisten Pendaftaran Acara Keluarga

Bayangkan kamu membuat **asisten pendaftaran digital** yang berjalan di terminal (CLI) untuk acara keluarga. Asisten ini akan menanyakan nama, umur, dan minat peserta, lalu menampilkan resume pendaftaran di layar. Seperti panitia yang mencatat tamu satu per satu, tapi serba otomatis!

---

## 🎯 Goal Latihan

Setelah latihan ini, kamu akan:
- Memahami cara kerja CLI dan input/output di Node.js
- Bisa membuat program yang menerima input dari pengguna
- Menampilkan output yang rapi dan informatif di terminal
- Siap membangun tool CLI sederhana untuk kebutuhan apapun

---

## 📋 Checklist Langkah

1. **Buat folder project dan file utama:**
   ```bash
   mkdir asisten-pendaftaran-cli
   cd asisten-pendaftaran-cli
   npm init -y
   touch form-wizard.js
   ```
2. **Tampilkan sapaan awal di terminal**
3. **Tanyakan nama, umur, dan minat peserta (gunakan readline)**
4. **Setelah semua terisi, tampilkan resume pendaftaran di terminal**
5. **Validasi:**
   - Nama tidak boleh kosong
   - Umur harus angka
6. **(Bonus) Simpan hasil ke file `result.txt`**
7. **(Bonus) Tambahkan argumen `--lang` untuk bahasa**

---

## 🗂️ Struktur File Disarankan

```
asisten-pendaftaran-cli/
├── form-wizard.js
├── README.md
└── fundamental.md
```

---

## 🧪 Contoh Output CLI

```
📋 Resume Pendaftaran:
Nama   : Raka Pratama
Umur   : 21
Minat  : Backend
Terima kasih sudah mengisi form!
```

---

## 💡 Tips Pro & Troubleshooting
- Jika CLI tidak jalan, cek penulisan kode dan jalankan dengan `node form-wizard.js`
- Gunakan `console.log()` untuk debug
- Cek hasil file dengan `cat result.txt`
- Untuk argumen, cek dengan `process.argv`

---

## 🔗 Referensi
- [Node.js readline module](https://nodejs.org/api/readline.html)
- [Command Line Arguments – Node.js Docs](https://nodejs.org/en/learn/getting-started/how-to-parse-command-line-arguments/)
- [Zellwk CLI tutorial](https://zellwk.com/blog/cli/)

---

> "CLI itu seperti ngobrol langsung dengan komputer. Semakin sering latihan, semakin luwes kamu mengendalikan sistem!"

