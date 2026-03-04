# 🩺 SehatKu — Platform Konsultasi Kesehatan Online

Website jasa konsultasi kesehatan digital yang siap deploy ke Vercel. Dibangun dengan HTML, CSS, dan JavaScript murni tanpa framework — ringan, cepat, dan mudah dikustomisasi.

---

## 📁 Struktur File

```
sehatku/
├── index.html      # Seluruh halaman website (HTML + CSS + JS)
├── vercel.json     # Konfigurasi deployment Vercel
└── README.md       # Dokumentasi ini
```

---

## ✨ Fitur

- **Hero Section** — Tagline, statistik, CTA, dan animasi floating card dokter
- **Layanan** — 6 jenis layanan dengan harga (Chat, Video Call, Klinik, Lab, Resep, Konseling)
- **Direktori Dokter** — 8 dokter dengan filter Semua / Umum / Spesialis / Online
- **Form Booking** — Validasi input + modal konfirmasi sukses
- **Artikel Kesehatan** — Layout featured artikel edukasi
- **Testimoni** — Review pasien berbintang
- **FAQ** — Accordion interaktif 6 pertanyaan
- **Footer** — Navigasi lengkap + info legalitas
- **Responsive** — Mobile-friendly dengan hamburger menu
- **Animasi** — Scroll fade-in, floating cards, hover effects, toast notification

---

## 🎨 Cara Kustomisasi

### Ganti Nama & Branding
Cari teks `SehatKu` di `index.html` dan ganti dengan nama brand kamu.

### Ganti Warna
Edit CSS variables di bagian `:root` di dalam `index.html`:
```css
:root {
  --sage:    #6bbf9a;   /* warna aksen hijau */
  --forest:  #1a4d3a;   /* warna utama gelap */
  --cream:   #f9f5ee;   /* background utama */
  --coral:   #e07060;   /* warna aksen merah */
}
```

### Tambah/Edit Dokter
Cari array `dokters` di bagian `<script>` dan tambahkan objek baru:
```js
{ nama: 'dr. Nama Dokter', spesialis: 'Spesialisasi', emoji: '👨‍⚕️', rating: 4.9, ulasan: 100, kategori: 'spesialis', online: true }
```

### Tambah/Edit FAQ
Cari array `faqs` di bagian `<script>` dan tambahkan:
```js
{ q: 'Pertanyaan kamu?', a: 'Jawaban lengkapnya di sini.' }
```

### Ganti Harga
Cari teks `Mulai Rp` di `index.html` dan sesuaikan dengan tarif kamu.

---

## 🛠 Teknologi

| Teknologi | Keterangan |
|-----------|-----------|
| HTML5 | Struktur halaman |
| CSS3 | Styling + animasi (tanpa library) |
| Vanilla JS | Interaktivitas (tanpa framework) |
| Google Fonts | Font Fraunces + DM Sans |
| Vercel | Hosting & deployment |

---

## 📋 Lisensi

Bebas digunakan dan dimodifikasi untuk keperluan pribadi maupun komersial.