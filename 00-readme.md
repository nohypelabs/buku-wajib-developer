FILE 00-README.md (UNIVERSAL)
markdown
# Panduan Arsitektur — Universal Design Patterns

> **Pola:** Decoupled Architecture (Hexagonal DDD + Modular Component-Based)  
> **Prinsip:** Pragmatis, Scalable, Maintainable, Anti-Over-Engineering  
> **Universal:** Dapat diimplementasikan di STACK APAPUN (React, Vue, Next.js, Express, Django, Laravel, dll.)

---

## 📁 Struktur Root (Generik)
src/
├── server/ # 🔴 BACKEND ONLY
│ └── modules/[module]/
├── client/ # 🔵 FRONTEND ONLY
│ ├── (admin)/
│ ├── (dashboard)/
│ └── (public)/
└── shared/ # Shared components / utils

text

> **Catatan:** Nama folder bisa disesuaikan dengan stack (contoh: `app/` untuk Next.js, `src/` untuk React, `routes/` untuk Express).

---

## 🎯 Panduan Cepat (Universal)

| **Yang Ingin Dibuat** | **Baca File** | **Lokasi (Generik)** |
|---|---|---|
| Backend module baru (CRUD) | `01-BACKEND.md` §2 | `src/server/modules/[feature]/` |
| Backend module kompleks | `01-BACKEND.md` §3 | `src/server/modules/[feature]/` |
| Halaman frontend baru | `02-FRONTEND.md` §3 | `src/client/(group)/[route]/page.tsx` |
| Komponen UI baru | `02-FRONTEND.md` §3.2 | `src/client/(group)/[route]/_components/` |
| Error handling & observability | `03-ADVANCED.md` | `src/server/shared/errors/` |
| Environment variables | `03-ADVANCED.md` §2 | `src/env.ts` atau `.env` |
| Database migration | `03-ADVANCED.md` §3 | `prisma/` atau `migrations/` |
| Monorepo scaling | `03-ADVANCED.md` §4 | `apps/` + `packages/` |
| Implementasi per stack | `04-STACK-SPECIFIC.md` | Contoh: Next.js, Express, Django |

---

## 📚 Panduan Lengkap

- **Backend:** Baca `01-BACKEND.md`
- **Frontend:** Baca `02-FRONTEND.md`
- **Advanced Topics:** Baca `03-ADVANCED.md`
- **Stack-Specific:** Baca `04-STACK-SPECIFIC.md`

---

**Dokumen ini adalah kitab wajib bagi seluruh developer dan AI Agent. Gunakan di project APAPUN. 🚀**
