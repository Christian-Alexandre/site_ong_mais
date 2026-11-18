# Site ONG Mais

Página de apresentação do app ONG Mais com botão de download do APK.

## Estrutura
- `index.html` – a página (HTML + CSS + JS num arquivo só)
- `downloads/ONG_Mais.apk` – o APK do app
- `logo.png` / `favicon.png` – logo do app (mesma do ícone Android)
- `vercel.json` – força o download do .apk com o tipo certo

## Publicar no Vercel
1. Gere o APK: `flutter build apk --release` na pasta `app/`
2. Copie `build/app/outputs/flutter-apk/app-release.apk` para `downloads/ONG_Mais.apk`
3. Suba esta pasta num repositório GitHub (ou use `npx vercel` aqui dentro)
4. No Vercel: New Project → importe o repo → Framework Preset: **Other** → Deploy
   (não precisa de build command nem output directory)
