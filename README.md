# CarnaTiller 2027 — Landing Page & Simulador de Alta Conversão

Repositório autossuficiente pronto para publicação no **GitHub Pages** da campanha **CarnaTiller 2027 — Tiller Confecções**.

## O que está incluso nesta pasta
- `index.html` — Página principal de alta conversão (Hero com ancoragem de preço, Prova Social real, 4 passos, Catálogo Top 10 + 183 modelos com busca, 4 Tipos de Sublimação 2027 conectados ao simulador, Simulador com Retirada em Natal/RN ou Envio p/ fora do RN, FAQ, barra sticky mobile, GA4 `G-ZHPX185Q6Q` e **Meta Pixel pronto para conversão `Lead`**).
- `imagens/` — Todos os ativos já otimizados para 4G:
  - `campanha/alegria-neon-2027.jpg`
  - `prova-social/` (fotos reais otimizadas)
  - `estampas/` (4 artes 2027 corrigidas)
  - `categoria-1/` a `categoria-4/` (todos os 183 modelos prontos)
  - `og-carnatiller-2027.jpg` (capa para compartilhamento no WhatsApp/Instagram)
- `m/001.html` a `m/193.html` — Páginas de compartilhamento direto de cada modelo para grupos de WhatsApp.
- `favicon.svg` · `.nojekyll` · `.gitignore`

---

## Passo 1 — Inserir seu ID do Meta Pixel (1 linha)

Antes de subir (ou a qualquer momento), abra `index.html` e localize no `<head>`:

```js
const META_PIXEL_ID = "COLE_SEU_PIXEL_ID_AQUI";
```

Substitua `COLE_SEU_PIXEL_ID_AQUI` pelo número do seu Pixel do Meta Ads (ex.: `"123456789012345"`).

**Eventos disparados automaticamente assim que o ID for preenchido:**
- `PageView` — ao carregar a página.
- `ViewContent` — ao trocar coleção ou ampliar qualquer modelo.
- `InitiateCheckout` — ao escolher um modelo para simular.
- `Lead` *(com `value`, `currency: "BRL"`, modelo e quantidade)* — em todo clique para pedir orçamento ou Arte Grátis no WhatsApp `(84) 2133-8804`.

---

## Passo 2 — Subir para um Novo Repositório no GitHub

1. Crie um repositório novo e vazio no GitHub (ex.: `carnatiller2027`).
2. Abra o terminal dentro desta pasta `site-carnatiller-2027-github` e rode:

```bash
git init
git branch -M main
git add .
git commit -m "Publicacao inicial CarnaTiller 2027 alta conversao"
git remote add origin https://github.com/SEU_USUARIO/SEU_NOVO_REPO.git
git push -u origin main
```

3. No GitHub, acesse **Settings → Pages**:
   - Em **Build and deployment / Source**, selecione **Deploy from a branch**.
   - Em **Branch**, escolha `main` e pasta `/ (root)`, depois clique em **Save**.
4. Em cerca de 1 a 2 minutos, o novo site estará no ar em:
   `https://SEU_USUARIO.github.io/SEU_NOVO_REPO/`
