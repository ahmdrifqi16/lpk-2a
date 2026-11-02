# LKP 2A — Halaman Profil Pribadi dengan HTML5 & CSS

Praktikum **Pertemuan 2: HTML5 & CSS Dasar** (Pemrograman Base Platform).
Proyek ini adalah halaman profil statis. Tidak perlu instal apa pun, cukup browser.

## 1. Isi Folder

```
lpk-2a/
├── index.html          -> struktur halaman (HTML5 semantik)
├── style.css           -> seluruh styling (CSS eksternal)
├── assets/
│   └── foto.png        -> foto profil
├── screenshot/
│   ├── screenshot-desktop.png
│   └── screenshot-mobile.png
└── README.md           -> dokumen ini
```

## 2. Cara Menjalankan (Langkah demi Langkah)

1. Buka folder `lpk-2a`.
2. Klik dua kali file `index.html`. Halaman akan terbuka di browser.
3. Selesai. Tidak perlu server atau internet.

Opsional, kalau memakai VS Code: klik kanan `index.html` lalu pilih **Open with Live Server**.

## 3. Penjelasan Singkat Kode

### HTML (index.html)

| Elemen      | Fungsi                              |
| ----------- | ----------------------------------- |
| `<header>`  | Bagian atas: foto, nama, keterangan |
| `<nav>`     | Menu link ke bagian halaman         |
| `<main>`    | Konten utama                        |
| `<section>` | Bagian Tentang, Keahlian, Kontak    |
| `<footer>`  | Hak cipta                           |

### CSS (style.css)

- **Flexbox** dipakai pada menu `nav` (`display: flex`, `justify-content: center`, `gap`).
- **CSS Grid** dipakai pada `.cards` (`repeat(auto-fit, minmax(180px, 1fr))`), sehingga kartu otomatis turun baris di layar kecil.
- **Box model**: `* { box-sizing: border-box; }` agar ukuran elemen sudah termasuk padding dan border.
- **Efek hover** pada link menu dan kartu.
