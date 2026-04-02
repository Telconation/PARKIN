<p align="center">
<img src="public\images\icons\icon-x144.png">
</p>
<h1 align="center">PARKIN Landing Page</h1>

Ini adalah repositori khusus untuk antarmuka muka (**Landing Page**) proyek PARKIN. Website ini dibangun untuk melayani fungsi pengenalan produk.
> **PENTING:** Kode dari repositori **PARKIN System** dipublikasikan secara terpisah atau bersifat tertutup (privat).

## 🛠️ Stack Teknologi

- **Framework Builder:** Astro (V5.x)
- **Styling:** Tailwind CSS V4 (Bawaan Astro Integration) + Vanilla CSS (`global.css`)
- **Assets / Icons:** FontAwesome v6 (CDN / SVG rendering)
---

## 🏗️ Struktur Direktori Dasar (Landing Page)

```text
LandingPage/
├── public/                 # File publik tanpa proses
│   ├── images/             # Tangkapan layar, Ikon, Favicon
│   └── fonts/              # Tipehuruf kustom (Inter, dsb)
├── src/
│   ├── components/         # Konfigurasi per-Komponen Astro (Navbar, Hero, FAQ)
│   ├── i18n/               # Kamus translasi Bahasa (ui.ts)
│   ├── layouts/            # Tata Letak Utama (Blok anti-FOIT ada di sini)
│   ├── pages/              # Routing Aplikasi (index.astro, en/index.astro)
│   └── styles/             # Global Tailwind & Root CSS variabel (global.css)
├── astro.config.mjs        # Konfigurasi Astro
└── package.json            # Daftar NPM Script & Dependencies
```

---

## 💻 Panduan Instalasi Lokal (Penyetelan)

Anda bisa menjalankan salinan murni dari repositori situs pemasaran ini untuk dipelajari atau membantu pemecahan masalah:

1. **Pastikan Node.js terinstal** (Versi 18+ sangat disarankan).
2. Tiru (_Clone_) repositori Landing Page ini ke komputer Anda.
3. Masuk ke direktori utama: `cd LandingPage`
4. Lakukan instalasi ketergantungan paket Node:
   ```bash
   npm install
   ```
5. Putar _Development Server_:
   ```bash
   npm run dev
   ```
6. Situs dapat diakses melalui peramban pada alamat lokal (umumnya `http://localhost:4321`).

Untuk menguji kompilasi statis tahap produksi:
```bash
npm run build
npm run preview
```

---

## 🤝 Aturan Kontribusi Khusus (Semi-Open Source)

Kode proyek ini pada dasarnya bersifat bebas akses dan dapat dianalisis secara bebas untuk keperluan edukasi antarmuka. **NAMUN**, Akses Repositori PARKIN System bersifat terbatas. Uuntuk integrasi perubahan (*Pull Request*) harus mematuhi kebijakan verifikasi internal.

Langkah-lagkah jika Anda ingin menyerahkan ide penyempurnaan ke kode dasar ini:

1. **WAJIB:** Buka sebuah diskursus di menu _**Issues**_ pada repositori GitHub ini terlebih dahulu. Paparkan desain proposal atau _bug_ apa yang ingin Anda selesaikan.
2. Tunggu persetujuan (_Approval_) dari (_Owner / Maintainer_).
3. Setelah proposal disetujui (_Owner / Maintainer_) akun anda akan ditambahkan sebagai _Collaborator_, kemudian Anda dapat Fork repositorinya.
4. Setel perubahan di atas repositori kloningan milik Anda sendiri. Periksa kembali standar aksesibilitas tampilan (WCAG) yang ada.
5. Jika telah siap, kirimkan **Pull Request (PR)** sembari menyertakan catatan Referensi #Issue dari langkah pertama.
6. Saya akan mereviu kode baris per-baris sebelum ditarik (*merge*) ke produksi publik.

_Terima kasih atas segala ketertarikan Anda untuk menelisik infrastruktur antarmuka PARKIN System._