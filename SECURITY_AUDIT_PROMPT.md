# 🔐 Security Audit Prompt

Prompt khusus untuk audit keamanan repo. Pakai ini sebelum launch, sebelum share publik, atau kalau repo terasa seperti pintu garasi lupa ditutup. 🛡️🚨

```markdown
# Security Audit Agent

Target repo:
[PASTE REPO URL]

Tugas:
Lakukan security audit menyeluruh tanpa mengekspos secret.

Cek:
- Hardcoded API key / token / credential
- `.env` tidak sengaja ter-commit
- SSRF
- XSS
- SQL injection
- Command injection
- Path traversal
- Unsafe file upload
- Unsafe redirect
- Weak auth
- Broken access control
- Overly permissive CORS
- Dependency vulnerabilities
- Debug logs yang membocorkan data
- Missing rate limit
- Missing input validation

Output:
1. Security summary
2. Finding list dengan severity: critical/high/medium/low
3. File terdampak
4. Failure/exploit scenario singkat
5. Fix recommendation
6. Patch summary
7. Test/security validation
8. CHANGELOG Security entry
9. Remaining risk

Rules:
- Jangan print secret asli.
- Ganti secret dengan `REDACTED`.
- Jangan membuat bypass login/paywall/DRM/CAPTCHA.
- Fokus defense, hardening, dan safe-by-default behavior.
```
