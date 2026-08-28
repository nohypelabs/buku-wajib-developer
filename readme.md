# 📚 Buku Wajib Developer — Universal Architecture Guide

> **Pola:** Decoupled Architecture (Hexagonal DDD + Modular Component-Based)  
> **Prinsip:** Pragmatis, Scalable, Maintainable, Anti-Over-Engineering  
> **Universal:** Dapat diimplementasikan di STACK APAPUN (React, Vue, Next.js, Express, Django, Laravel, Go, dll.)

---

## 📖 Dokumentasi Lengkap

Repo ini berisi **17 file panduan** yang mencakup semua aspek pengembangan software — dari arsitektur, setup environment, testing, deployment, sampai keamanan.

| **File** | **Fungsi** |
|----------|------------|
| [`01-backend.md`](01-backend.md) | Backend architecture (Hexagonal DDD) — Level 1 (CRUD) & Level 2 (State Machine) |
| [`02-frontend.md`](02-frontend.md) | Frontend architecture — Feature-based folder, composition root, component rules |
| [`03-advanced.md`](03-advanced.md) | Advanced topics — error handling, environment validation, monitoring, monorepo |
| [`04-stack-specific.md`](04-stack-specific.md) | Implementasi di 7 stack populer (Next.js, Express, Django, Laravel, Flask, Vue, dll.) |
| [`05-create-Newrepo.md`](05-create-Newrepo.md) | Git workflow + GitHub CLI (`gh`) cheat sheet |
| [`ARCHITECTURE.md`](ARCHITECTURE.md) | High-level architecture overview (ringkasan cepat) |
| [`PROJECT-STRUCTURE.md`](project-structure.md) | Penjelasan detail struktur folder dan kapan pindah ke shared |
| [`DEVELOPMENT.md`](development.md) | Panduan setup environment lokal (clone, install, run, migrate) |
| [`DEPLOYMENT.md`](deployment.md) | Panduan deploy ke production/staging (manual, CI/CD, rollback) |
| [`TESTING.md`](testing.md) | Strategi testing (unit, integration, E2E) dan coverage target |
| [`CONTRIBUTING.md`](contributing.md) | Panduan kontribusi — branch strategy, commit convention, PR process |
| [`API.md`](API.md) | Dokumentasi endpoint API (contoh untuk REST) |
| [`FAQ.md`](FAQ.md) | Pertanyaan umum seputar setup, arsitektur, dan troubleshooting |
| [`SECURITY.md`](SECURITY.md) | Kebijakan keamanan & cara melaporkan vulnerability |
| [`CHANGELOG.md`](CHANGELOG.md) | Catatan perubahan versi (ikuti Keep a Changelog) |
| [`LICENSE`](LICENSE) | Lisensi MIT — open source, bebas digunakan dan dimodifikasi |
| [`README.md`](README.md) | **Halaman ini** — pintu masuk ke semua dokumentasi |

---

## 🎯 Panduan Cepat (Berdasarkan Kebutuhan)

| **Yang Ingin Dibuat** | **Baca File** | **Lokasi (Generik)** |
|---|---|---|
| Backend module baru (CRUD) | `01-backend.md` §2 | `src/server/modules/[feature]/` |
| Backend module kompleks (state machine) | `01-backend.md` §3 | `src/server/modules/[feature]/` |
| Halaman frontend baru | `02-frontend.md` §3 | `src/client/(group)/[route]/page.tsx` |
| Komponen UI baru | `02-frontend.md` §3.2 | `src/client/(group)/[route]/_components/` |
| Error handling & observability | `03-advanced.md` | `src/server/shared/errors/` |
| Environment variables | `03-advanced.md` §2 | `src/env.ts` atau `.env` |
| Database migration | `03-advanced.md` §3 | `prisma/` atau `migrations/` |
| Monorepo scaling | `03-advanced.md` §4 | `apps/` + `packages/` |
| Setup lokal & menjalankan project | `development.md` | — |
| Deploy ke production | `deployment.md` | — |
| Testing | `testing.md` | — |
| Kontribusi | `contributing.md` | — |
| Lihat daftar API | `API.md` | — |
| Cari jawaban cepat | `FAQ.md` | — |
| Laporkan kerentanan | `SECURITY.md` | — |

---

## 🚀 Cara Mulai (Singkat)

```bash
# Clone repo
git clone git@github.com:nohypelabs/buku-wajib-developer.git
cd buku-wajib-developer

# Setup environment
cp .env.example .env
# Edit .env sesuai konfigurasi lokal

# Install dependencies (sesuai stack)
npm install   # atau pnpm install / yarn

# Jalankan development
npm run dev
Untuk panduan lebih detail, baca DEVELOPMENT.md.

🤝 Kontribusi
Kami sangat terbuka untuk kontribusi! Silakan baca CONTRIBUTING.md sebelum mengirim Pull Request.

📄 Lisensi
Proyek ini dilisensikan di bawah MIT License — bebas digunakan, dimodifikasi, dan didistribusikan.

🙏 Terima Kasih
Dokumen ini adalah kitab wajib bagi seluruh developer dan AI Agent. Gunakan di project APAPUN. 🚀

Happy coding!


