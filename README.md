# Meus Links

Página simples para reunir todos os seus links de afiliado em um só lugar,
hospedada gratuitamente no GitHub Pages.

## Estrutura

- `index.html` + `style.css` — a página pública que as pessoas vão ver.
- `data.json` — seu nome, bio e a lista de links. É o único arquivo que você
  precisa editar para atualizar o site.
- `admin.html` — uma ferramenta **para uso local**, que te ajuda a editar
  `data.json` sem mexer em código (abrir, não publicar o acesso a ela para outras pessoas).

## Como publicar no GitHub Pages

1. No repositório `GerenciadorLink` no GitHub, vá em **Settings → Pages**.
2. Em "Build and deployment", escolha **Source: Deploy from a branch**.
3. Em "Branch", escolha `main` e pasta `/ (root)`, depois **Save**.
4. Em alguns minutos o site fica disponível em:
   `https://arii19.github.io/GerenciadorLink/`

## Como atualizar seus links (sem programar)

1. Abra o arquivo `admin.html` **no seu computador** (dois cliques nele, abre
   no navegador).
2. Clique em **"Carregar data.json atual"** e selecione o `data.json` que
   está na pasta do projeto (ou baixado do GitHub).
3. Edite seu perfil, adicione/remova/reordene links.
4. Clique em **"Baixar data.json atualizado"**.
5. No GitHub, abra o arquivo `data.json` do repositório, clique no ícone de
   lápis (editar), apague o conteúdo antigo, cole o novo conteúdo e clique em
   **Commit changes**. O site atualiza sozinho em 1–2 minutos.

   (Alternativa, se preferir usar o Git: substitua o arquivo local, depois
   `git add data.json`, `git commit -m "atualiza links"`, `git push`.)

## Segurança

- O repositório é **público** (necessário para o GitHub Pages gratuito) —
  nunca coloque senhas, tokens de API ou dados pessoais sensíveis em nenhum
  arquivo aqui, só os links em si.
- Ative a **verificação em duas etapas (2FA)** na sua conta do GitHub
  (Settings → Password and authentication).
- Cada link de afiliado já abre em nova aba com `rel="sponsored noopener noreferrer"`,
  que é a prática recomendada pelo Google e evita que a página de destino
  manipule a aba original.
- O site já inclui um aviso de que há links de afiliado — isso é importante
  por transparência com quem visita a página.
- Antes de publicar, confira se cada URL aponta mesmo para o site oficial do
  programa de afiliados (evita links errados ou de phishing).
