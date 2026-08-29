# 🚀 Server Penyimpanan Kata Sandi Aman Mandiri Vaultwarden

[![Lisensi: Open Source](https://img.shields.io/badge/Lisensi-Open%20Source-blue.svg)](#)
[![Deployment: Docker Compose](https://img.shields.io/badge/Deploy-Docker%20Compose-2496ED.svg?logo=docker&logoColor=white)](#)
[![Status: Siap Pakai](https://img.shields.io/badge/Status-Produksi%20Siap%20Pakai-brightgreen.svg)](#)
[![Developer: Muhammad Fikri](https://img.shields.io/badge/Developer-Muhammad%20Fikri-blue.svg)](#)

Server brankas kata sandi privat berbasis Vaultwarden (kompatibel penuh dengan aplikasi Bitwarden) dengan enkripsi end-to-end Zero-Knowledge dan backup otomatis berkala.

---

## ⚡ Fitur Utama & Keunggulan Arsitektur
- **Instalasi Sekali Klik:** Dilengkapi skrip otomasi interaktif `install.sh` untuk deployment instan.
- **Konfigurasi Produksi Aman:** Template `.env.example` dengan variabel lingkungan terisolasi dan izin file yang aman.
- **Manajemen Siklus Hidup Layanan:** Termasuk skrip pemeliharaan mandiri (`scripts/backup.sh`, `scripts/restore.sh`, dan update berkala).
- **Kepatuhan Lisensi Open-Source:** Mengikuti lisensi resmi pengembang hulu (*upstream license compliant*).

---

## 🚀 Panduan Instalasi & Penggunaan Cepat

### 1. Kloning Repositori
```bash
git clone https://github.com/muhammadfikri-dev/vaultwarden-secure-password-vault.git
cd vaultwarden-secure-password-vault
```

### 2. Konfigurasi Lingkungan
Salin file template konfigurasi dan sesuaikan variabel yang diperlukan:
```bash
cp .env.example .env
nano .env
```

### 3. Menjalankan Layanan
Jalankan skrip instalasi otomatis atau gunakan Docker Compose secara langsung:
```bash
chmod +x install.sh
./install.sh
# Atau eksekusi langsung via docker compose:
docker compose up -d
```

---

## 🛠️ Manajemen & Pemeliharaan Kontainer

- **Melihat Status Layanan:** `docker compose ps`
- **Melihat Log Real-time:** `docker compose logs -f`
- **Mematikan Layanan:** `docker compose down`
- **Membuat Backup Data:** `./scripts/backup.sh`

---

## 📄 Lisensi
Didistribusikan di bawah lisensi resmi open-source. Dikembangkan dan dikonfigurasi untuk standar industri oleh **Muhammad Fikri**.
