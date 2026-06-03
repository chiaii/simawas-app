# Panduan Kontribusi SIMAWAS

Terima kasih telah meluangkan waktu untuk berkontribusi! 🎉  
Setiap kontribusi — sekecil apapun — sangat berarti bagi pengembangan SIMAWAS.

---

## 📋 Daftar Isi

- [Kode Etik](#kode-etik)
- [Cara Berkontribusi](#cara-berkontribusi)
- [Melaporkan Bug](#melaporkan-bug)
- [Mengusulkan Fitur](#mengusulkan-fitur)
- [Kontribusi Kode](#kontribusi-kode)
- [Kontribusi Dokumentasi](#kontribusi-dokumentasi)
- [Standar Penulisan Kode](#standar-penulisan-kode)
- [Proses Review](#proses-review)
- [Kontak](#kontak)

---

## 🤝 Kode Etik

Proyek ini berkomitmen untuk menjadi ruang yang ramah dan inklusif bagi semua kontributor.  
Kami mengharapkan semua peserta untuk:

- Menggunakan bahasa yang ramah dan sopan
- Menghormati perbedaan sudut pandang dan pengalaman
- Menerima kritik membangun dengan lapang dada
- Mengutamakan kepentingan komunitas dan pengguna akhir

Perilaku yang tidak dapat diterima akan dilaporkan kepada maintainer di **[anasu1997@gmail.com]**.

---

## 🚀 Cara Berkontribusi

Ada banyak cara untuk berkontribusi tanpa harus menulis kode:

| Jenis Kontribusi | Cara |
|------------------|------|
| 🐛 Menemukan bug | Buka Issue baru |
| 💡 Ide fitur baru | Buka Issue dengan label `enhancement` |
| 📖 Perbaiki dokumentasi | Buat Pull Request |
| 💻 Kerjakan Issue | Lihat Issues berlabel `good first issue` |
| 🏛️ Pilot project pemda | Hubungi maintainer langsung |
| 🌐 Terjemahan | Bantu terjemahkan dokumentasi |

---

## 🐛 Melaporkan Bug

Sebelum membuat laporan bug, pastikan kamu sudah:
- [ ] Memeriksa apakah bug yang sama sudah pernah dilaporkan di tab **Issues**
- [ ] Mencoba mereproduksi bug di versi terbaru

### Format Laporan Bug

Buat Issue baru dengan judul: `[BUG] Deskripsi singkat masalah`

Isi dengan template berikut:

```
## Deskripsi Bug
Jelaskan bug secara singkat dan jelas.

## Langkah Reproduksi
1. Buka halaman '...'
2. Klik tombol '...'
3. Lihat error di '...'

## Perilaku yang Diharapkan
Jelaskan apa yang seharusnya terjadi.

## Perilaku Aktual
Jelaskan apa yang benar-benar terjadi.

## Screenshot (jika ada)
Tambahkan screenshot untuk membantu menjelaskan masalah.

## Lingkungan
- OS: [contoh: Windows 11, Ubuntu 22.04]
- Browser: [contoh: Chrome 120, Firefox 121]
- Versi SIMAWAS: [contoh: v0.1.0]
```

---

## 💡 Mengusulkan Fitur

Punya ide untuk meningkatkan SIMAWAS? Kami sangat terbuka!

Buat Issue baru dengan judul: `[FEAT] Nama fitur yang diusulkan`

Isi dengan template berikut:

```
## Latar Belakang
Jelaskan masalah atau kebutuhan yang mendorong usulan ini.

## Solusi yang Diusulkan
Jelaskan fitur yang kamu usulkan secara detail.

## Alternatif yang Dipertimbangkan
Apakah ada pendekatan lain yang sudah kamu pertimbangkan?

## Konteks Tambahan
Apakah ada contoh dari sistem lain? Siapa yang akan paling terbantu?
```

---

## 💻 Kontribusi Kode

### 1. Fork & Clone Repositori

```bash
# Fork dulu via GitHub UI, lalu clone fork kamu
git clone [https://github.com/chiaii/simawas-app]
cd simawas
```

### 2. Buat Branch Baru

Gunakan konvensi penamaan berikut:

```bash
# Untuk fitur baru
git checkout -b feat/nama-fitur

# Untuk perbaikan bug
git checkout -b fix/nama-bug

# Untuk dokumentasi
git checkout -b docs/nama-dokumentasi
```

Contoh:
```bash
git checkout -b feat/google-drive-integration
git checkout -b fix/login-redirect-error
git checkout -b docs/panduan-instalasi
```

### 3. Kerjakan Perubahanmu

- Pastikan kode kamu mengikuti [standar penulisan kode](#standar-penulisan-kode)
- Tulis atau perbarui tes jika diperlukan
- Pastikan semua tes berjalan dengan baik sebelum commit

### 4. Commit dengan Pesan yang Jelas

Kami menggunakan konvensi **Conventional Commits**:

```
<type>: <deskripsi singkat>

[isi opsional]

[footer opsional]
```

**Tipe yang tersedia:**

| Tipe | Digunakan untuk |
|------|----------------|
| `feat` | Fitur baru |
| `fix` | Perbaikan bug |
| `docs` | Perubahan dokumentasi |
| `style` | Perubahan format/style (bukan logika) |
| `refactor` | Refaktor kode |
| `test` | Menambah atau memperbaiki tes |
| `chore` | Perubahan build, dependency, dsb |

Contoh pesan commit yang baik:
```bash
git commit -m "feat: tambah integrasi Google Drive untuk upload dokumen"
git commit -m "fix: perbaiki redirect setelah login role inspektorat"
git commit -m "docs: tambah langkah konfigurasi Google OAuth di README"
```

### 5. Push dan Buat Pull Request

```bash
git push origin feat/nama-fitur
```

Lalu buka repositori di GitHub dan klik **"Compare & pull request"**.

### Format Pull Request

Gunakan judul yang deskriptif dan isi template berikut:

```
## Ringkasan
Jelaskan perubahan yang kamu buat secara singkat.

## Jenis Perubahan
- [ ] Bug fix
- [ ] Fitur baru
- [ ] Breaking change
- [ ] Pembaruan dokumentasi

## Issue Terkait
Closes #[nomor issue]

## Cara Pengujian
Jelaskan langkah-langkah untuk menguji perubahan ini.

## Checklist
- [ ] Kode mengikuti standar penulisan proyek ini
- [ ] Saya sudah melakukan self-review terhadap kode saya
- [ ] Saya sudah menambahkan komentar pada bagian yang sulit dipahami
- [ ] Dokumentasi sudah diperbarui jika diperlukan
- [ ] Tidak ada error atau warning baru yang muncul
```

---

## 📖 Kontribusi Dokumentasi

Dokumentasi yang baik sama pentingnya dengan kode yang baik.  
Kamu bisa berkontribusi di:

- `README.md` — Deskripsi utama proyek
- `docs/` — Panduan instalasi, konfigurasi, dan penggunaan
- Komentar dalam kode — Penjelasan fungsi dan logika

Untuk dokumentasi dalam Bahasa Indonesia, pastikan menggunakan ejaan yang benar sesuai KBBI.  
Untuk dokumentasi dalam Bahasa Inggris, gunakan bahasa yang sederhana dan mudah dipahami.

---

## 📐 Standar Penulisan Kode

- **Indentasi:** 4 spasi (bukan tab)
- **Encoding:** UTF-8
- **Line ending:** LF (Unix-style)
- **Panjang baris:** Maksimal 120 karakter
- **Komentar:** Tulis dalam Bahasa Indonesia atau Inggris, konsisten dalam satu file
- **Penamaan variabel:** gunakan `camelCase` untuk variabel dan fungsi, `PascalCase` untuk class
- **Penamaan file:** gunakan `kebab-case` untuk nama file

> Standar tambahan spesifik per bahasa/framework akan ditambahkan setelah stack teknologi diputuskan.

---

## 🔍 Proses Review

Setelah kamu membuat Pull Request:

1. **Maintainer akan merespons dalam 3–5 hari kerja**
2. Mungkin ada permintaan perubahan — ini normal dan bukan penolakan
3. Setelah disetujui, PR akan di-merge ke branch `main`
4. Nama kamu akan ditambahkan ke daftar kontributor 🎉

### Tips agar PR cepat di-review:
- Buat PR yang fokus — satu PR untuk satu perubahan
- Tulis deskripsi yang jelas
- Pastikan tidak ada konflik dengan branch `main`
- Hubungkan PR ke Issue yang relevan

---

## 🏛️ Untuk Pemerintah Daerah

Apakah kamu bekerja di instansi pemerintah daerah dan tertarik mengadopsi SIMAWAS?

Kami membuka kesempatan **pilot project** dengan:
- Dukungan instalasi dan konfigurasi awal
- Pendampingan onboarding pengguna
- Prioritas penanganan isu dan permintaan fitur

Hubungi maintainer di **[anasu1997@gmail.com]** dengan subjek: `[PILOT] Nama Instansi - Kabupaten/Kota`

---

## 📬 Kontak

Punya pertanyaan yang tidak tercakup di sini?

- **Email:** [anasu1997@gmail.com]
- **GitHub Discussions:** [github.com/chiaii/simawas-app/discussions/6]
- **Issue:** Buka Issue baru dengan label `question`

---

<div align="center">
  <i>Bersama kita wujudkan pemerintahan daerah yang lebih transparan dan akuntabel. 🇮🇩</i>
</div>
