# 🧰✨ AI Repo Checkup Kit

> **General Check-Up Kit untuk Git repository**: audit repo, cari bug 🐞, cek security 🔐, rapikan dokumentasi 📚, susun roadmap 🗺️, update changelog 📝, dan siapkan deployment 🚀 dengan bantuan AI Agent seperti ChatGPT, Cursor, Cline, Codex, atau agent coding lainnya.

![Status](https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge)
![Made for AI Agents](https://img.shields.io/badge/AI_Agent-ready-blueviolet?style=for-the-badge)
![Markdown First](https://img.shields.io/badge/Markdown-first-111111?style=for-the-badge)
![Security Mindset](https://img.shields.io/badge/security-checkup-red?style=for-the-badge)

---

## 🌟 About This Repo

**AI Repo Checkup Kit** adalah kumpulan prompt, template, dan workflow Markdown untuk membantu kamu melakukan **General Check-Up** pada repository Git apa pun.

Repo ini cocok untuk:

- 🔍 Audit struktur project
- 🐞 Cari bug dan error build
- 🧪 Cek test, lint, dan quality gate
- 🔐 Review security issue dan bad practice
- 🧹 Bersih-bersih dokumentasi
- 🗺️ Susun roadmap fitur berikutnya
- 📝 Catat changelog dan development notes
- 🚀 Siapkan launch ke Vercel / hosting lain
- 🤖 Memberi instruksi yang jelas ke AI Agent

Bayangkan repo ini seperti **kotak P3K untuk project Git**: tinggal buka, ambil prompt yang tepat, tempel ke agent, lalu agent punya peta kerja yang rapi. 🧭✨

---

## 🏷️ Suggested GitHub About

Gunakan ini untuk kolom **About / Description** di GitHub:

```text
🧰 AI-powered Git repo checkup kit: prompts, templates, changelog workflow, debugging checklist, security audit, roadmap planning, and deployment notes for any project.
```

### 🧩 Suggested Topics

Tambahkan topics ini di GitHub repo:

```text
ai-agent
chatgpt
repo-audit
git-checkup
prompt-engineering
debugging
security-audit
changelog
roadmap
vercel
development-workflow
markdown-template
```

---

## ⚡ Cara Pakai Cepat

### 1️⃣ Pilih repo target

Contoh:

```text
https://github.com/username/project-name
```

### 2️⃣ Buka file prompt / template dari kit ini

Minimal pakai:

```text
GENERAL_CHECKUP_PROMPT.md
```

Kalau file belum dibuat, kamu bisa pakai **Master Prompt** di bawah. 👇

### 3️⃣ Tempel ke AI Agent

Bisa dipakai di:

- 🤖 ChatGPT
- 🧠 Cursor
- 🐺 Cline
- ⚙️ Codex
- 🧪 GitHub Copilot Workspace
- 🛠️ AI coding agent lain

### 4️⃣ Tambahkan notes kamu

Contoh notes:

```markdown
# Repo Check-Up Notes

## Target Repo
https://github.com/username/project-name

## Goal
Saya ingin audit repo ini, cari bug, rapikan README, cek build error, dan siapkan roadmap fitur.

## Priority
P0: Fix error critical
P1: Siapkan demo / launch
P2: Tambah fitur berikutnya

## Batasan
- Jangan hapus fitur lama tanpa alasan
- Jangan expose API key / token / secret
- Semua perubahan wajib dicatat di CHANGELOG.md
- Semua method wajib dicatat di DEVELOPMENT_NOTES.md
```

### 5️⃣ Biarkan agent kerja bertahap

Agent harus melakukan:

- 🔎 Scan repo
- 🧱 Peta arsitektur
- 🧪 Jalankan lint/test/build
- 🐞 Cari bug
- 🔐 Audit security
- 🛠️ Fix masalah
- 📝 Update docs
- 🚀 Siapkan deploy
- 📦 Beri ringkasan perubahan

---

## 🤖 Master Prompt: General Git Repo Check-Up

Copy prompt ini ke AI Agent:

```markdown
# General Git Repo Check-Up Agent

Kamu adalah Senior Software Engineer, QA Engineer, Security Reviewer, Documentation Writer, Release Manager, dan Deployment Engineer.

Target repository:
[PASTE GITHUB REPO URL DI SINI]

Input notes dari user:
[PASTE NOTES DI SINI]

## 🎯 Misi Utama

Lakukan General Check-Up repository secara menyeluruh:

1. Audit struktur repo
2. Identifikasi framework, bahasa, package manager, dan entry point
3. Jalankan quality gate yang relevan
4. Cari bug, error, warning, dan bad practice
5. Audit security issue
6. Debug masalah yang ditemukan
7. Tambahkan atau lanjutkan fitur berdasarkan notes user
8. Update dokumentasi
9. Update changelog
10. Catat method kerja di development notes
11. Siapkan rekomendasi next sprint
12. Siapkan instruksi deployment bila ada

## 🧪 Quality Gate

Cek command yang relevan berdasarkan stack repo:

- npm install / pnpm install / yarn install / bun install
- npm run lint
- npm run test
- npm run build
- npm run typecheck
- npm run dev
- docker build bila ada Dockerfile
- deployment check bila ada Vercel/Netlify config

Jika command tidak tersedia, jangan paksa. Tulis alasannya dan rekomendasikan script yang perlu ditambahkan.

## 🔐 Security Audit

Cari dan perbaiki masalah seperti:

- Secret/API key hardcoded
- Token/cookie tersimpan di repo
- SSRF
- XSS
- SQL injection
- Command injection
- Path traversal
- Unsafe file upload
- Unsafe redirect
- Missing input validation
- Weak auth / broken access control
- Dependency vulnerable
- Overly permissive CORS
- Exposed debug logs
- Unsafe environment variable handling

Jangan pernah mencetak secret asli di output. Gunakan format `REDACTED`.

## 🐞 Bug & Debug Checklist

Cek:

- Build error
- Runtime crash
- TypeScript error
- ESLint warning
- Missing import
- Broken route
- Broken API endpoint
- Broken state management
- Broken async flow
- Race condition
- Memory leak
- Error handling kosong
- Loading state tidak jelas
- Empty state tidak ada
- Mobile responsive issue
- Bad UX copywriting

## 🧭 Development Method

Kerjakan secara bertahap:

### Step 1: Repo Mapping
Tulis ringkasan:
- Tech stack
- Folder penting
- Entry point
- API route
- Database / storage bila ada
- Deployment target

### Step 2: Risk Scan
Tulis daftar masalah:
- Critical
- High
- Medium
- Low

### Step 3: Fix Plan
Untuk tiap masalah, tulis:
- File terdampak
- Root cause
- Solusi
- Risiko perubahan
- Test plan

### Step 4: Implementation
Lakukan patch kecil dan aman.

### Step 5: Validation
Jalankan command validasi dan catat hasilnya.

### Step 6: Documentation
Update:
- README.md
- CHANGELOG.md
- DEVELOPMENT_NOTES.md
- ROADMAP.md bila perlu

## 📝 Output Wajib

Setelah selesai, berikan laporan:

1. Executive summary
2. Tech stack yang terdeteksi
3. Struktur repo
4. Bug ditemukan
5. Security issue ditemukan
6. Perubahan kode
7. File yang diubah
8. Test yang dijalankan
9. Hasil validasi
10. Changelog entry
11. Development method
12. Risiko tersisa
13. Next sprint recommendation
14. Deployment instruction
15. Commit message rekomendasi

## 🚦 Priority System

Gunakan prioritas berikut:

- P0 🔥 Critical: build gagal, app crash, security blocker
- P1 🚀 Launch: deploy, docs, demo, UX dasar
- P2 ✨ Product: fitur baru, dashboard, polish
- P3 🧱 Scale: database, queue, observability, CI/CD lanjutan

## 📦 Commit Message Format

Gunakan conventional commit:

```text
feat: add new feature
fix: resolve bug
security: patch security issue
docs: update documentation
test: add or update tests
refactor: improve structure without changing behavior
chore: update tooling/config
ci: update pipeline/deployment
```

## ⚠️ Rules

- Jangan hapus fitur lama tanpa alasan kuat
- Jangan expose secret/token/API key
- Jangan membuat perubahan besar tanpa catatan risiko
- Jangan mengabaikan test/build failure
- Jangan menebak hasil command, jalankan atau tulis bahwa command belum dijalankan
- Semua asumsi harus ditulis
- Semua perubahan harus bisa dijelaskan

Mulai sekarang dari audit repo, lalu lanjutkan berdasarkan notes user.
```

---

## 📁 Struktur File yang Disarankan

Repo kit ini idealnya berkembang menjadi:

```text
AI-Repo-Checkup-Kit/
├─ README.md                         # 🌟 Halaman utama
├─ GENERAL_CHECKUP_PROMPT.md          # 🤖 Prompt audit umum
├─ DEBUG_PROMPT.md                    # 🐞 Prompt debug bertahap
├─ SECURITY_AUDIT_PROMPT.md           # 🔐 Prompt audit security
├─ FEATURE_DEVELOPMENT_PROMPT.md      # ✨ Prompt lanjut fitur
├─ VERCEL_DEPLOY_PROMPT.md            # 🚀 Prompt deploy Vercel
├─ CHANGELOG_TEMPLATE.md              # 📝 Template changelog
├─ DEVELOPMENT_NOTES_TEMPLATE.md      # 📓 Template catatan method
├─ ROADMAP_TEMPLATE.md                # 🗺️ Template roadmap
└─ repo-notes/
   ├─ example-nextjs.md               # ⚛️ Contoh notes Next.js
   ├─ example-python.md               # 🐍 Contoh notes Python
   └─ example-general.md              # 🧰 Contoh notes umum
```

---

## 🧾 Template Notes Harian

Pakai ini setiap mau menyuruh agent kerja:

```markdown
# Daily Repo Check-Up Notes

## 📌 Target Repo
[URL repo]

## 🎯 Goal Hari Ini
- [ ] Audit repo
- [ ] Fix bug
- [ ] Tambah fitur
- [ ] Update docs
- [ ] Siapkan deploy

## 🐞 Masalah yang Terlihat
- ...

## ✨ Fitur yang Diinginkan
- ...

## 🔐 Security Concern
- ...

## 🚀 Deployment Target
- Vercel / Netlify / Railway / VPS / Docker / lainnya

## 📦 Output yang Saya Mau
- Ringkasan bug
- Patch/fix
- Changelog
- Development notes
- Commit message

## ⚠️ Batasan
- Jangan expose secret
- Jangan hapus fitur lama sembarangan
- Jangan refactor besar tanpa alasan
```

---

## 📝 Template CHANGELOG.md

```markdown
# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added
- ✨ ...

### Changed
- 🔁 ...

### Fixed
- 🐞 ...

### Security
- 🔐 ...

### Docs
- 📚 ...

### Removed
- 🗑️ ...
```

---

## 📓 Template DEVELOPMENT_NOTES.md

```markdown
# Development Notes

## Session: YYYY-MM-DD HH:mm

### 🎯 Goal
- ...

### 🧠 Assumptions
- ...

### 🔍 Findings
- ...

### 🛠️ Method
- ...

### 📁 Files Changed
- ...

### 🧪 Validation
- ...

### ✅ Result
- ...

### ⚠️ Remaining Risks
- ...

### 🚀 Next Steps
- ...
```

---

## 🗺️ Template ROADMAP.md

```markdown
# Roadmap

## P0 🔥 Critical Stability
- [ ] Fix build error
- [ ] Fix runtime crash
- [ ] Fix security blocker

## P1 🚀 Launch Ready
- [ ] Improve README
- [ ] Add deployment guide
- [ ] Add health check
- [ ] Add env example

## P2 ✨ Product Features
- [ ] Add dashboard
- [ ] Add export feature
- [ ] Add settings page

## P3 🧱 Scale & Automation
- [ ] Add CI/CD
- [ ] Add monitoring
- [ ] Add database adapter
- [ ] Add Docker support
```

---

## 🚀 Deployment Check-Up Prompt

Gunakan saat mau launch:

```markdown
Audit repo ini untuk deployment.

Target deployment:
[Vercel / Netlify / Railway / VPS / Docker]

Cek:
- Build command
- Output directory
- Env vars
- Runtime compatibility
- Filesystem limitation
- API route limitation
- Serverless timeout
- Logging
- Error page
- Health endpoint
- Security headers
- README deployment guide

Setelah audit, update dokumentasi dan berikan step deploy yang aman.
```

---

## 🔐 Secret Safety Rules

Jangan simpan ini di Markdown publik:

- ❌ API key asli
- ❌ GitHub token
- ❌ Vercel token
- ❌ Cookie/session
- ❌ Database password
- ❌ Private key
- ❌ OAuth client secret

Gunakan contoh aman:

```env
OPENAI_API_KEY=REDACTED
DATABASE_URL=REDACTED
VERCEL_TOKEN=REDACTED
```

Atau buat `.env.example`:

```env
OPENAI_API_KEY=
DATABASE_URL=
NEXT_PUBLIC_APP_URL=
```

---

## 🧠 Best Workflow

```text
1. Tulis notes 📝
2. Tempel Master Prompt 🤖
3. Agent scan repo 🔎
4. Agent fix batch kecil 🛠️
5. Agent run test/build 🧪
6. Agent update changelog 📚
7. Review hasil 👀
8. Commit + deploy 🚀
```

---

## ✅ Definition of Done

Satu sesi check-up dianggap selesai kalau:

- [ ] Repo sudah dipetakan 🧭
- [ ] Bug utama ditemukan 🐞
- [ ] Security issue dicatat 🔐
- [ ] Fix sudah dibuat 🛠️
- [ ] Test/build sudah dicoba 🧪
- [ ] README diperbarui 📚
- [ ] CHANGELOG diperbarui 📝
- [ ] DEVELOPMENT_NOTES diperbarui 📓
- [ ] Next steps jelas 🚀
- [ ] Commit message disiapkan 📦

---

## 💡 Contoh Perintah ke ChatGPT / AI Agent

```markdown
Gunakan AI Repo Checkup Kit ini.

Target repo:
https://github.com/username/project-name

Goal:
General check-up repo, cari bug, audit security, update README, dan siapkan roadmap.

Gunakan format output dari README kit ini.
Jangan expose secret.
Update CHANGELOG dan DEVELOPMENT_NOTES.
```

---

## 🧰 Maintainer Notes

Repo ini dibuat untuk workflow personal dan bisa dipakai ulang di banyak project. Tambahkan template baru sesuai kebutuhan:

- ⚛️ Next.js
- 🐍 Python
- 🦀 Rust
- 🐳 Docker
- 🚀 Vercel
- 🔐 Security audit
- 📱 Mobile app
- 🧪 Testing workflow

---

## 📜 License

Gunakan bebas untuk workflow pribadi. Kalau nanti mau dibuat lebih formal, tambahkan file `LICENSE` seperti MIT License. ⚖️

---

## 🌈 Final Words

Build repo itu bukan cuma nulis kode. Repo yang sehat butuh catatan, peta, alarm kebakaran, kotak perkakas, dan sedikit confetti. 🎉

**AI Repo Checkup Kit** hadir supaya setiap project punya co-pilot kecil yang rapi, cerewet secukupnya, dan siap bantu sebelum bug berubah jadi naga produksi. 🐉🛡️
