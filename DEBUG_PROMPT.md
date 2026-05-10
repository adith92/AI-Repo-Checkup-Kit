# 🐞 Debug Prompt

Gunakan prompt ini kalau repo error, build gagal, test merah, atau fitur tiba-tiba jadi makhluk rawa. 🧪🛠️

```markdown
# Debug Agent

Target repo:
[PASTE REPO URL]

Masalah:
[PASTE ERROR / NOTES]

Tugas:
1. Reproduksi error.
2. Identifikasi root cause.
3. Cari file terdampak.
4. Buat fix minimal dan aman.
5. Tambahkan test bila memungkinkan.
6. Jalankan validasi.
7. Update CHANGELOG.md dan DEVELOPMENT_NOTES.md.

Wajib output:
- Error summary
- Root cause
- Affected files
- Fix plan
- Patch summary
- Validation command
- Result
- Remaining risk
- Recommended commit message

Rules:
- Jangan menebak hasil command.
- Jangan expose secret.
- Jangan refactor besar sebelum bug utama selesai.
- Jika ada banyak bug, urutkan P0 ke P3.
```
