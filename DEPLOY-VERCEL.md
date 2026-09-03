# 🚀 Publicação do Portal na Vercel

O portal é um site **estático de arquivo único** (`index.html`) — não precisa de
build, framework ou configuração especial. Basta subir os arquivos para a Vercel.

## Opção A — Conectar este repositório GitHub (recomendado, deploy automático)

Com o repositório conectado, **todo push na branch `main` publica automaticamente**
uma nova versão do portal.

1. Acesse [vercel.com](https://vercel.com) e entre com sua conta.
2. Clique em **Add New → Project**.
3. Na lista de repositórios, escolha **`Infraestrutura2026/portal-infraestrutura-cpm`**
   (se o repositório não aparecer, clique em *Adjust GitHub App Permissions* /
   *Add GitHub Account* e autorize a organização `Infraestrutura2026`).
4. Na tela de configuração do projeto:
   - **Framework Preset:** `Other` *(a Vercel detecta sozinha — deixe em branco)*
   - **Build Command:** vazio
   - **Output Directory:** vazio (a raiz do repositório já contém o `index.html`)
   - **Root Directory:** `./`
5. Clique em **Deploy**.
6. Ao terminar, o portal estará publicado em:
   `https://portal-infraestrutura-cpm.vercel.app`

### Próximas atualizações

A partir daí, basta editar os arquivos neste repositório e **enviar para a branch
`main`** (merge de um pull request, por exemplo). A Vercel publica sozinha em
segundos.

---

## Opção B — Publicar sem Git (upload manual / CLI)

Se preferir publicar manualmente os arquivos desta pasta:

- **Via CLI:** `npm i -g vercel && vercel` dentro da pasta do projeto e depois
  `vercel --prod` (o arquivo `index.html` e a pasta `images/` são enviados).
- **Via painel:** Vercel → **Add New → Project → Upload** (`vercel deploy` sem Git)
  e arraste os arquivos.

---

## 🌐 Domínio (opcional)

Se houver um domínio próprio (ex.: `portal.infraestrutura.cpm.sp.gov.br`), em
**Project → Settings → Domains** adicione o domínio e siga as instruções de DNS
apontando para `cname.vercel-dns.com`.

---

## ✏️ Como trocar um link do portal depois

Os endereços dos sistemas ficam nos `href` dos cartões dentro de `index.html`
(busque por `vercel.app`). Exemplo — cartão da frota:

```html
<a class="card" href="https://frotacpm.vercel.app/" ...>
```

Troque o endereço, faça o commit/push na `main` e a Vercel republica sozinha.
