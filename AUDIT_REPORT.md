# Audit Report — Evaluasi Pekan 3

## 1) Peta Struktur

- Lampiran: `structure.txt` (di commit ini)

## 2) Aset Salah Tempat

- Ditemukan file gambar di root:
  ./24-7-support.png
  ./arrow-down.png
  ./arrow-left.png
  ./arrow-right.png
  ./arrow-up.png
  ./background.jpg
  ./banner-old.jpg
  ./banner.jpg
  ./bg.jpg
  ./cart-icon.png
  ./check-icon.png
  ./close-icon.png
  ./customer-service.jpg
  ./delivery-truck.jpg
  ./email-icon.png
  ./error-icon.png
  ./facebook-icon.png
  ./fast-delivery.png
  ./hero-bg.jpg
  ./hero-image.jpg
  ./info-icon.png
  ./instagram-icon.png
  ./linkedin-icon.png
  ./location-icon.png
  ./logo-backup.png
  ./logo-copy.png
  ./logo.png
  ./logo_old.png
  ./menu-icon.png
  ./money-back.png
  ./office-photo.jpg
  ./payment-methods.jpg
  ./phone-icon.png
  ./product1-thumb.png
  ./product1.jpg
  ./product2-thumb.png
  ./product2.jpg
  ./product3-thumb.png
  ./product3.jpg
  ./quality-guarantee.png
  ./search-icon.png
  ./security-badge.png
  ./slide1-mobile.jpg
  ./slide1.jpg
  ./slide2-mobile.jpg
  ./slide2.jpg
  ./slide3-mobile.jpg
  ./slide3.jpg
  ./star-empty.png
  ./star-filled.png
  ./team-member1.jpg
  ./team-member2.jpg
  ./team-member3.jpg
  ./testimonial1.jpg
  ./testimonial2.jpg
  ./testimonial3.jpg
  ./twitter-icon.png
  ./user-icon.png
  ./warehouse-photo.jpg
  ./warning-icon.png
  ./whatsapp-icon.png
  ./youtube-icon.png

  → rekomendasi pindah ke `assets/images/`.

## 3) Bug CSS (Tidak Ter-render)

- File: `index.html`
- Temuan: `href="style.css"` → **seharusnya** `href="assets/css/style.css"`
- Dampak: CSS tidak termuat → tampilan berantakan.
- Rekomendasi: perbaiki path & satukan CSS ke `assets/css/`.

## 4) Forensik Git — debug.log

- Commit pertama menambahkan `semua project yang berantakan ini 🗿`: main 2025-08-21 18:17:26 +0700 iqbaljlldn`
- Baris sensitif:
  - Baris 12: `API_KEY=xA-tOpSecReT-12345`

## 5) Rekomendasi Perbaikan Terukur (untuk Orang 2)

- [ ] Pindah aset ke `assets/images/`
- [ ] Perbaiki semua path CSS → `assets/css/style.css`
- [ ] Tambahkan `.gitignore` untuk `*.log`

---

_Disiapkan oleh: Orang 1 (Auditor & Repo Manager)_
