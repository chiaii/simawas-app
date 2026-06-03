# SIMAWAS
### Sistem Manajemen Dokumen Pengawasan Pemerintah Daerah

> **Open-source platform** untuk mempermudah pengiriman dan pengelolaan dokumen evaluasi antara dinas pemerintah daerah dan inspektorat — terintegrasi langsung dengan Google Drive.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/status-in%20development-yellow)]()
[![Platform](https://img.shields.io/badge/platform-web-blue)]()
[![Made for](https://img.shields.io/badge/made%20for-Indonesia%20Local%20Government-red)]()

---

## 🎯 Latar Belakang

Indonesia memiliki **514 kabupaten/kota**, masing-masing dengan puluhan dinas yang wajib menyerahkan dokumen evaluasi dan kepatuhan secara berkala kepada inspektorat daerah.

Kenyataannya, proses ini masih berjalan melalui:
- 💬 Grup WhatsApp yang tidak terstruktur
- 📧 Email tanpa sistem pelacakan
- 📂 Dokumen fisik yang rawan hilang

Akibatnya:
- Dokumen sering tidak terdata dengan baik
- Tidak ada *audit trail* yang jelas
- Beban administratif tinggi bagi ASN
- Evaluasi dan tindak lanjut menjadi lambat

**SIMAWAS hadir sebagai solusi open-source yang bisa di-*deploy* mandiri oleh pemerintah daerah mana pun.**

---

## ✨ Fitur Utama

| Fitur | Deskripsi |
|-------|-----------|
| 📤 **Pengiriman Dokumen Terstruktur** | Dinas dapat mengirim dokumen sesuai kategori dan periode yang ditentukan |
| ☁️ **Integrasi Google Drive** | Dokumen tersimpan otomatis ke folder Google Drive yang terorganisasi |
| ✅ **Manajemen Status** | Inspektorat dapat mengubah status dokumen: *Diterima*, *Revisi*, atau *Ditolak* |
| 📊 **Dashboard Rekapitulasi** | Pantau progres pengiriman semua dinas dalam satu tampilan |
| 🔔 **Notifikasi Deadline** | Pengingat otomatis bagi dinas yang belum mengirimkan dokumen |
| 📋 **Riwayat & Audit Trail** | Setiap aksi tercatat lengkap dengan timestamp dan identitas pengguna |
| 👥 **Multi-role Access** | Peran terpisah untuk Admin, Inspektorat, dan Operator Dinas |

---

## 🗺️ Roadmap

### v0.1 — Foundation *(In Progress)*
- [ ] Setup repositori & struktur proyek
- [ ] Autentikasi multi-role (Admin / Inspektorat / Dinas)
- [ ] Manajemen dinas dan kategori dokumen
- [ ] Upload dokumen dasar

### v0.2 — Google Drive Integration
- [ ] OAuth2 Google Drive
- [ ] Penyimpanan dokumen ke folder terstruktur otomatis
- [ ] Preview dokumen langsung dari aplikasi

### v0.3 — Workflow & Tracking
- [ ] Sistem status dokumen (Diterima / Revisi / Ditolak)
- [ ] Komentar dan catatan dari inspektorat
- [ ] Notifikasi in-app dan email

### v1.0 — Production Ready
- [ ] Dashboard rekapitulasi & laporan
- [ ] Notifikasi deadline otomatis
- [ ] Panduan deployment lengkap
- [ ] Docker support untuk kemudahan instalasi

---

## 🏗️ Arsitektur

```
┌─────────────────────────────────────────┐
│              SIMAWAS Web App            │
├─────────────┬───────────────────────────┤
│   Frontend  │        Backend / API      │
│  (Browser)  │   (REST / Server-side)    │
└─────────────┴──────────┬────────────────┘
                         │
              ┌──────────▼──────────┐
              │    Google Drive API │
              │  (Document Storage) │
              └─────────────────────┘
```

> **Stack:** Belum final — kontribusi dan saran terbuka. Kami memprioritaskan stack yang umum digunakan oleh developer pemerintah daerah Indonesia (PHP/Laravel atau Python/Django).

---

## 🚀 Cara Deploy *(Coming Soon)*

Panduan instalasi lengkap akan tersedia setelah v0.2. Sementara ini, kamu bisa mengikuti perkembangan proyek melalui tab [Issues](../../issues) dan [Discussions](../../discussions).

---

## 🌏 Potensi Adopsi

SIMAWAS dirancang agar bisa diadopsi oleh pemerintah daerah mana pun tanpa perlu kustomisasi besar:

- ✅ **23 kabupaten/kota di Aceh** memiliki struktur inspektorat yang identik
- ✅ **514 kabupaten/kota di Indonesia** menghadapi tantangan yang sama
- ✅ Sejalan dengan agenda digitalisasi pemerintahan dari **BPK** dan **KPK**
- ✅ Bebas lisensi vendor — self-hosted, data tetap milik pemda

---

## 🤝 Kontribusi

Proyek ini terbuka untuk kontribusi! Kami terutama membutuhkan bantuan di:

- 🐛 **Bug reporting** — temukan masalah dan laporkan via Issues
- 🌐 **Dokumentasi** — bantu tulis panduan dalam Bahasa Indonesia dan Inggris
- 💻 **Development** — lihat Issues berlabel `good first issue`
- 🏛️ **Pemerintah Daerah** — tertarik jadi pilot project? Hubungi kami!

Baca [CONTRIBUTING.md](CONTRIBUTING.md) untuk panduan kontribusi.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License** — bebas digunakan, dimodifikasi, dan didistribusikan oleh siapa pun, termasuk instansi pemerintah, tanpa biaya lisensi.

Lihat [LICENSE](LICENSE) untuk detail lengkap.

---

## 📬 Kontak

**Maintainer:** [Muhammad Anas]  
**Lokasi:** Bireuen, Aceh, Indonesia  
**Email:** [anasu1997@gmail.com]  
**Instansi Pilot:** Inspektorat Kabupaten Bireuen, Aceh

---

<div align="center">
  <i>Dibangun untuk transparansi dan akuntabilitas pemerintahan Indonesia. 🇮🇩</i>
</div>
