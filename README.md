# Zeik Digital — Site oficial

Site institucional da **Zeik Digital**: site profissional, Instagram e tráfego pago
para negócios da Zona Sul de São Paulo.

🔗 Contato: [WhatsApp (11) 99014-7836](https://wa.me/5511990147836) · zeikdigital@gmail.com · [@zeikdigital](https://www.instagram.com/zeikdigital)

## Como funciona

O site é **um único arquivo** (`index.html`) com HTML, CSS e JavaScript embutidos.
As imagens (logo, assinatura e logos dos clientes) estão em base64 dentro do próprio arquivo.

- Sem build, sem npm, sem dependência externa
- Abre direto no navegador (clicar duas vezes no `index.html` já funciona)
- Funciona offline

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `zeik-site`)
2. Suba os arquivos desta pasta
3. No GitHub: **Settings → Pages → Source: Deploy from a branch → `main` / `root`** → Save
4. Em ~1 minuto o site fica no ar em `https://SEUUSUARIO.github.io/zeik-site/`

### Comandos

```bash
git init
git add .
git commit -m "Site da Zeik Digital"
git branch -M main
git remote add origin https://github.com/SEUUSUARIO/zeik-site.git
git push -u origin main
```

### Domínio próprio (opcional)

Se comprar um domínio (ex.: `zeikdigital.com.br`), crie um arquivo chamado `CNAME`
com o domínio dentro e aponte o DNS para o GitHub Pages.

## Publicar sem Git (mais rápido)

- **Netlify Drop**: https://app.netlify.com/drop — arrasta a pasta e já está no ar
- **Vercel**: importa o repositório e publica sem configurar nada

## Onde editar as coisas

| O que | Onde procurar no `index.html` |
|---|---|
| WhatsApp | `5511990147836` |
| E-mail | `zeikdigital@gmail.com` |
| Instagram | `zeikdigital` |
| Preços | seção `id="precos"` e a caixa `.f-price` |
| Empresas do portfólio | seção `id="empresas"` |
| Perguntas do formulário | seção `id="contato"` (`#leadForm`) |
| Cores da marca | `:root` → `--a1` (ciano `#00ccdd`) |

O formulário **não usa servidor**: ele monta a mensagem e abre o WhatsApp do Ezequiel.
