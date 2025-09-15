# Chá de Bebê — Site estático (GitHub Pages)

Este projeto contém:
- `index.html` — convite + RSVP por WhatsApp + lista (lendo `produtos.xlsx` via SheetJS) + seção PIX com **QR Code** e botão **Copiar chave**.
- `produtos.xlsx` — itens apropriados para chá de bebê.
- `hero.jpeg` — imagem do topo (sua foto enviada).
- `bradesco.png` — QR Code do PIX (mantida a mesma lógica do seu site atual).

## Como usar
1. **Edite o bloco `CONFIG` no `index.html`** e ajuste:
   - `datetime` / `datetimeText` (data/hora)
   - `mapsQuery` (endereço)
   - `pixKey` (sua chave PIX)
   - `whatsapp`, `rsvpText`, `reserveText`
   - `defaultSource`: deixe `xlsx` para ler a planilha.
2. **Edite os produtos** em `produtos.xlsx` (colunas: `nome | detalhe | valor`).

## Publicar no GitHub Pages
```bash
# Crie um repositório novo (substitua NOME_DO_REPO pelo nome desejado)
cd baby-shower-site
git init
git add .
git commit -m "Chá de bebê: convite + lista + PIX"
git branch -M main
# Crie o repo no GitHub e conecte:
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPO.git
git push -u origin main
```
Depois, no GitHub: **Settings → Pages → Source: Deploy from a branch → main / root**.
Abra a URL que o Pages mostrar.

---

Qualquer dúvida, só falar. 💖
