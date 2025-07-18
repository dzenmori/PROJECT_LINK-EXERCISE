# 📚 FUNDAMENTAL: Dasar Interaksi JavaScript di Halaman Web

Selamat datang di dunia JavaScript! Di sini kamu akan belajar membuat halaman web yang bisa merespon aksi pengguna, seperti tombol yang bisa diklik, sapaan otomatis, dan perubahan tampilan secara dinamis.

---

## 🗂️ Glossary Umum & Fungsi Tagline

| Istilah/Tagline         | Fungsi/Deskripsi                                                                                 | Contoh/Analogi                                    |
|------------------------|--------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Kartu Ucapan Interaktif| Tema exercise: membuat halaman yang bisa merespon pengguna dengan JS                              | Kartu ucapan yang bisa bicara/mengubah warna      |
| Interaksi              | Aksi yang terjadi saat pengguna melakukan sesuatu di halaman web                                 | Menekan tombol lampu, pintu otomatis              |
| Event                  | Kejadian/aksi pengguna yang bisa direspon kode                                                   | Klik, input, scroll, hover                        |
| Function               | Blok kode yang bisa dijalankan berulang kali                                                     | Resep masakan, tombol remote                      |
| Variable               | Tempat menyimpan data sementara                                                                  | Laci penyimpanan                                 |
| DOM                    | Struktur data yang mewakili isi halaman web                                                      | Denah rumah digital                               |
| Debugging              | Proses mencari dan memperbaiki error/kesalahan di kode                                           | Mencari kabel putus di rumah                      |
| Console                | Tempat melihat pesan/error di browser                                                            | Walkie-talkie untuk komunikasi                    |

---

## ⚡ Apa Itu JavaScript?
JavaScript adalah bahasa pemrograman utama di dunia web. Ia memungkinkan kamu untuk:
- Menangani aksi pengguna (klik, input, hover)
- Mengubah isi halaman secara dinamis
- Membuat animasi, form interaktif, validasi, popup, dan banyak lagi

### Analogi Sederhana:
> Jika HTML adalah kerangka dan CSS adalah tampilan, maka JavaScript adalah "otak" dan "otot" dari halamanmu — ia mengatur logika dan interaksi.

---

## 🏷️ Tabel Function/Metode/Objek JS Populer

| Fungsi/Konsep         | Fungsi/Deskripsi                                      | Contoh Penggunaan                                  |
|----------------------|-------------------------------------------------------|----------------------------------------------------|
| `document.getElementById` | Mengambil elemen HTML berdasarkan id           | `document.getElementById("judul")`                |
| `addEventListener`   | Menambahkan event handler ke elemen                   | `btn.addEventListener("click", fn)`               |
| `onclick`            | Event handler untuk klik                              | `btn.onclick = function() { ... }`                 |
| `alert`              | Menampilkan popup pesan                               | `alert("Halo!")`                                  |
| `console.log`        | Menampilkan pesan di console browser                  | `console.log("Cek data")`                         |
| `value`              | Mengambil/menetapkan nilai input                      | `input.value`                                      |
| `innerText`/`textContent` | Mengubah/mengambil isi teks elemen              | `el.innerText = "Hai!"`                           |
| `function`           | Mendefinisikan blok kode yang bisa dipanggil          | `function sapa() { ... }`                          |
| `let`/`const`/`var`  | Membuat variable                                      | `let nama = "Kadet";`                             |
| `if`/`else`          | Percabangan logika                                    | `if (nilai > 80) { ... } else { ... }`             |
| `for`/`while`        | Perulangan                                            | `for (let i=0; i<5; i++) { ... }`                  |
| `setTimeout`/`setInterval` | Menunda/menjadwalkan aksi berulang             | `setTimeout(fn, 1000)`                             |
| `Math.random`        | Menghasilkan angka acak                               | `Math.random()`                                    |

---

## 🧩 Fungsi/Interaksi Populer di Exercise
- Mengubah warna background halaman
- Menyapa pengguna berdasarkan input
- Menangani klik tombol (event handler)
- Mengambil dan menampilkan nilai input
- Menampilkan popup/alert
- Debugging dengan console.log

---

## 📐 Contoh Penggunaan JS Praktis

### Mengubah warna background saat tombol diklik
```js
document.getElementById("btn").onclick = function() {
  document.body.style.backgroundColor = "lightblue";
};
```

### Menyapa pengguna berdasarkan input
```js
document.getElementById("greetBtn").onclick = function() {
  const nama = document.getElementById("namaInput").value;
  document.getElementById("greetResult").innerText = "Halo, " + nama + "!";
};
```

### Menampilkan pesan di console
```js
console.log("Cek data");
```

---

## 📖 Kenapa Ini Penting?
- JavaScript membuat web jadi interaktif dan hidup
- Hampir semua website modern menggunakan JS untuk fitur dinamis
- JS adalah dasar untuk belajar framework modern (React, Vue, dsb)

---

## 🧠 Insight Tambahan
- Gunakan `console.log()` untuk debugging saat error
- Event handler bisa dipasang dengan `.onclick` atau `.addEventListener`
- Semua interaksi di web (klik, input, dsb) bisa di-handle dengan JS
- DOM = cara JS berkomunikasi dengan HTML

---

## 🔗 Referensi Tambahan
- [MDN – JavaScript First Steps](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps)
- [W3Schools – JavaScript](https://www.w3schools.com/js/)
- [JavaScript.info – Modern JS](https://javascript.info/)
- [FreeCodeCamp – JS Course](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)

### Video:
- [Codevolution – JavaScript for Beginners](https://www.youtube.com/watch?v=PkZNo7MFNFg)

---

## ✅ Tips untuk Kadet
- Jika tombol tidak berfungsi, cek id elemen dan koneksi file JS
- Gunakan `console.log()` untuk cek nilai variable
- Mulai dari interaksi sederhana, lalu eksplorasi lebih jauh
- Jangan takut error, debugging itu bagian dari belajar

---

> "JavaScript membuat web bukan hanya tampil, tapi bisa bicara balik padamu." 🧠💻

