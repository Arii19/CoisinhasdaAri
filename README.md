# Meus Links

Página simples para reunir todos os seus links de afiliado em um só lugar,
hospedada gratuitamente no GitHub Pages.

## Estrutura

- `index.html` + `style.css` — a página pública que as pessoas vão ver.
- `data.json` — seu nome, bio e a lista de links. É o único arquivo que você
  precisa editar para atualizar o site.
- `admin.html` — o editor do site. Abre pelo navegador, do celular ou do
  computador, em `https://arii19.github.io/CoisinhasdaAri/admin.html`, e
  salva direto no GitHub (precisa da sua chave de acesso, veja abaixo).

## Como publicar no GitHub Pages

1. No repositório `CoisinhasdaAri` no GitHub, vá em **Settings → Pages**.
2. Em "Build and deployment", escolha **Source: Deploy from a branch**.
3. Em "Branch", escolha `main` e pasta `/ (root)`, depois **Save**.
4. Em alguns minutos o site fica disponível em:
   `https://arii19.github.io/CoisinhasdaAri/`

## Como criar sua chave de acesso (uma vez só)

O editor precisa de uma chave para poder salvar alterações no seu repositório.
Essa chave é pessoal, funciona só com esse site e você pode revogar quando
quiser.

1. No GitHub, acesse **Settings → Developer settings → Personal access tokens
   → Fine-grained tokens** (ou direto: `github.com/settings/personal-access-tokens/new`).
2. Em **Repository access**, escolha **Only select repositories** e selecione
   `CoisinhasdaAri`.
3. Em **Permissions → Repository permissions**, defina **Contents** como
   **Read and write**. Deixe todo o resto sem acesso.
4. Escolha uma validade (ex: 90 dias) e clique em **Generate token**.
5. Copie a chave gerada (começa com `github_pat_...`) — ela só aparece uma vez.

## Como editar os links (do celular ou do computador)

1. Abra `https://arii19.github.io/CoisinhasdaAri/admin.html`.
2. Cole sua chave de acesso em **"Chave de acesso"** e clique em **"Conectar
   e carregar"**. O navegador guarda a chave só nesse aparelho — não precisa
   colar de novo da próxima vez.
3. Edite o perfil, adicione, edite, reordene ou remova links (pode enviar a
   foto do produto direto da galeria do celular).
4. Clique em **"Salvar no site"**. Em 1–2 minutos a mudança aparece no ar.

Se trocar de aparelho ou perder o acesso a algum deles, gere uma chave nova
pelo GitHub e revogue a antiga em **Settings → Developer settings → Personal
access tokens**.

## Segurança

- O repositório é **público** (necessário para o GitHub Pages gratuito) —
  nunca coloque senhas, tokens de API ou dados pessoais sensíveis em nenhum
  arquivo aqui, só os links em si.
- Sua chave de acesso **nunca** fica no código do site: ela só é guardada no
  navegador do seu próprio aparelho (localStorage) e enviada direto para a
  API do GitHub. Mesmo que alguém abra `admin.html`, não consegue editar nada
  sem a sua chave.
- Use sempre uma chave **fine-grained**, restrita só ao repositório
  `CoisinhasdaAri` e só com permissão de "Contents" — assim, mesmo se
  vazar, ninguém acessa o resto da sua conta GitHub.
- Ative a **verificação em duas etapas (2FA)** na sua conta do GitHub
  (Settings → Password and authentication).
- Cada link de afiliado já abre em nova aba com `rel="sponsored noopener noreferrer"`,
  que é a prática recomendada pelo Google e evita que a página de destino
  manipule a aba original.
- O site já inclui um aviso de que há links de afiliado — isso é importante
  por transparência com quem visita a página.
- Antes de publicar, confira se cada URL aponta mesmo para o site oficial do
  programa de afiliados (evita links errados ou de phishing).
