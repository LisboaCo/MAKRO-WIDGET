# Makro WhatsApp (LP em formato de conversa)

Site estatico. Tudo que sobe para a Cloudflare esta em `public/`.

## Opcao A - Deploy pelo terminal (mais rapido)
```
npx wrangler login
npx wrangler pages deploy public --project-name makro-whatsapp
```
URL: https://makro-whatsapp.pages.dev  (/ abre a conversa; /whatsapp tambem)

## Opcao B - Upload manual
Cloudflare > Workers & Pages > Create > Pages > Upload assets
Envie a PASTA `public/` (ou um zip do conteudo dela).

## Opcao C - Git
Cloudflare > Pages > Connect to Git. Build command: (vazio). Build output directory: `public`.

## Dominio proprio
Pages > projeto > Custom domains > Set up a domain.

## Antes de publicar de verdade
- `public/whatsapp.html`: remover `<meta name="robots" content="noindex, nofollow">`
- `CONFIG.PHONE`: trocar pelo WhatsApp oficial

- Link da Politica de Privacidade e rodape regulatorio (CRO) ainda pendentes
