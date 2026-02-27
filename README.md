# 🎯 CGMagic - Kompresi Gambar Ajaib di Browser

![CGMagic Preview](https://via.placeholder.com/1200x630/0a0c10/00ffff?text=CGMagic+Preview)

> 🚀 **Kompres gambar seperti sulap!** Ukuran file turun drastis, kualitas visual tetap tajam. 100% bekerja di browser, tanpa backend.

[![Live Demo](https://img.shields.io/badge/demo-live-00ffff?style=for-the-badge&logo=netlify)](https://caggyid.github.io/CGMagic/)
[![GitHub license](https://img.shields.io/github/license/caggyid/CGMagic?style=for-the-badge&color=7c3aed)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge&color=c084fc)](http://makeapullrequest.com)

## ✨ Fitur Ajaib

| Fitur | Deskripsi |
|-------|-----------|
| 🎯 **Kompresi Ekstrem** | Turun hingga 80%+ ukuran file dengan kualitas terjaga |
| 🖼️ **Multi Upload** | Drag & drop banyak gambar sekaligus (JPG, PNG, WEBP) |
| 👁️ **Slider Before/After** | Geser untuk melihat perbedaan kualitas secara real-time |
| 📊 **Live Info** | Tampilkan ukuran before/after + persentase penghematan |
| 🎚️ **Level Kompresi** | Low, Medium, High, atau Custom dengan slider |
| 📦 **Download All** | Simpan semua hasil kompresi dalam satu file ZIP |
| ⚡ **100% Client-side** | Privasi terjaga, tidak ada upload ke server |
| 📱 **Responsive** | Tampilan sempurna di desktop & mobile |

## 🎨 Tampilan Futuristik

- Tema gelap dengan aksen **neon gradient** (cyan & ungu)
- Efek glassmorphism dan glow yang halus
- Animasi loading modern dengan pulse effect
- Desain profesional ala produk SaaS premium

## 🚀 Demo Online

🔗 **Live Demo:** [https://caggyid.github.io/CGMagic](https://caggyid.github.io/CGMagic/)

## 📦 Instalasi & Penggunaan

### 1. Clone repository
```bash
git clone https://github.com/caggyid/CGMagic.git
cd CGMagic
```

### 2. Buka di browser
```bash
# Cukup buka index.html di browser favorit Anda
# Atau gunakan live server:
npx live-server
```

### 3. Mulai kompresi!
- Drag & drop gambar atau klik area upload
- Pilih level kompresi
- Klik "Kompres semua"
- Download hasil (satu-satu atau ZIP)

## 🛠️ Teknologi

- **HTML5** - Struktur semantik
- **CSS3** - Flexbox, Grid, Animasi, Glassmorphism
- **JavaScript (Vanilla)** - Logika kompresi tanpa framework
- **Canvas API** - Proses kompresi gambar
- **JSZip** - Membuat file ZIP untuk download all
- **Font Awesome 6** - Ikon-ikon keren

## 📁 Struktur Proyek

```
CGMagic/
├── index.html          # File utama (HTML, CSS, JS)
├── README.md           # Dokumentasi
├── LICENSE             # MIT License
└── assets/             # (opsional) Gambar preview
```

## ⚙️ Cara Kerja

1. **Upload** - Gambar dibaca via FileReader API
2. **Kompresi** - Canvas menggambar ulang dengan kualitas yang diatur
3. **Preview** - Menampilkan before/after dengan slider interaktif
4. **Download** - Blob hasil kompresi siap diunduh

```javascript
// Inti kompresi: cukup 5 baris!
const canvas = document.createElement('canvas');
canvas.width = img.width;
canvas.height = img.height;
canvas.getContext('2d').drawImage(img, 0, 0);
canvas.toBlob(callback, file.type, quality);
```

## 🎯 Level Kompresi

| Level | Kualitas | Cocok Untuk |
|-------|----------|-------------|
| **Low** | 90% | Foto penting, butuh kualitas maksimal |
| **Medium** | 70% | Keseimbangan size & kualitas |
| **High** | 40% | Web, hemat bandwidth maksimal |
| **Custom** | 0-100% | Kontrol penuh sesuai kebutuhan |

## 🌐 Browser Support

| Chrome | Firefox | Safari | Edge | Opera |
|--------|---------|--------|------|-------|
| ✅ 90+ | ✅ 88+ | ✅ 14+ | ✅ 90+ | ✅ 76+ |

## 📝 To Do / Roadmap

- [ ] Tambahkan opsi resize dimensi gambar
- [ ] Support format AVIF & JPEG XL
- [ ] Batch processing dengan progress bar
- [ ] Dark/light mode toggle
- [ ] PWA untuk installable app

## 🤝 Kontribusi

Kontribusi selalu diterima dengan tangan terbuka!

1. Fork repository
2. Buat branch fitur (`git checkout -b fitur-keren`)
3. Commit perubahan (`git commit -m 'Add fitur keren'`)
4. Push ke branch (`git push origin fitur-keren`)
5. Buka Pull Request

## 📄 Lisensi

MIT License © 2024 [Caggy ID](https://github.com/caggyid)

## 🙏 Credits

- Icons by [Font Awesome](https://fontawesome.com)
- ZIP compression by [Stuk/jszip](https://github.com/Stuk/jszip)
- Inspirasi desain dari TinyPNG & SaaS modern

---

## 💬 FAQ

**Q: Apakah gambar saya terkirim ke server?**  
A: **Tidak!** Semua proses 100% di browser Anda. Privasi terjaga.

**Q: Ada batasan ukuran file?**  
A: Disarankan maksimal 20MB per file (keterbatasan browser). File lebih besar mungkin lambat.

**Q: Format apa saja yang didukung?**  
A: JPG, PNG, dan WEBP. Output sesuai format asli.

**Q: Kok bisa gratis?**  
A: Karena semua proses menggunakan device Anda sendiri, tidak perlu server mahal 😉

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/caggyid">Caggy ID</a>
  <br>
  ⭐️ Star us on GitHub — it helps!
</p>
```
