# 🚀 Vercel Deploy Check Prompt

Prompt ini dipakai kalau target aplikasi mau demo atau launch di Vercel. Cocok untuk Next.js, React, API route, serverless app, dan project frontend modern. ⚡🌍

```markdown
# Vercel Deployment Agent

Target repo:
[PASTE REPO URL]

Target:
Siapkan repo agar aman dan siap deploy ke Vercel.

Cek:
- Framework detection
- Build command
- Install command
- Output directory
- Node/runtime version
- Environment variables
- API routes compatibility
- Serverless timeout risk
- Filesystem limitation
- Edge/runtime limitation
- CORS/security headers
- Error page
- Health endpoint
- README deployment guide
- `.env.example`

Jika app memakai filesystem lokal:
- Jangan asumsi storage permanen di serverless.
- Rekomendasikan `/tmp` hanya untuk temporary file.
- Rekomendasikan Blob/S3/R2 untuk persistent storage.

Output wajib:
1. Vercel readiness summary
2. Blocker list
3. Required env vars
4. Build/deploy commands
5. Files changed
6. Validation result
7. README update summary
8. Remaining risks
9. Step-by-step deploy instruction
10. Commit message recommendation
```
