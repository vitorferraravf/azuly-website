# azuly-website

Site institucional da **Azuly** — `https://azuly.app`.

Hospeda:
- Página inicial
- Política de Privacidade (`/privacy`)
- Termos de Uso (`/terms`)
- Página intermediária do Cloudflare Turnstile (`/turnstile.html`) — consumida pelo WebView do app via captcha invisible

## Deploy

Push pra `main` → GitHub Pages serve automaticamente em `azuly.app` (via custom domain).

## Editar conteúdo legal

Source-of-truth fica no repo do app: `Therapy/legal/*.md`.
Quando atualizar, espelhar:
1. `Therapy/legal/{privacy-policy,terms-of-service}.md`
2. `Therapy/legal/content.ts` (versão bundled in-app)
3. `Therapy/legal/site/{privacy,terms}.html` → copiar pra cá
