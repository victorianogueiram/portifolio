# Portfólio · Vic Nogueira

Site estático (HTML + CSS), bilíngue.

- Português na raiz (versão principal): `index.html`, `sobre.html`, `voluntariado.html`, `cases/app-pep.html`, `cases/portal-do-estabelecimento.html`
- Inglês em `en/`: `en/index.html`, `en/about.html`, `en/volunteering.html`, `en/cases/pep-app.html`, `en/cases/establishment-portal.html`
- URLs limpas (sem `.html`), configuradas no `vercel.json`: `/sobre`, `/en`, `/en/about` etc.
- Os links internos começam com `/`, então para ver no computador rode um servidor local na pasta (`npx serve .`) em vez de abrir o arquivo com duplo clique.
- Estilos em `assets/css/style.css`, imagens em `assets/img/`

## Pendências
- Link do currículo: procurar por `href="#"` nos links "resume" / "currículo" (header e footer de todas as páginas) e trocar pela URL.

## Subir no GitHub + Vercel
1. Crie um repositório no GitHub e suba esta pasta:
   ```
   git init
   git add .
   git commit -m "Portfólio v1"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/portfolio.git
   git push -u origin main
   ```
2. Na Vercel: Add New → Project → importe o repositório.
   Framework preset: **Other**. Sem build command, output directory em branco.
3. Cada `git push` na `main` publica uma nova versão.
