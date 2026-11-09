# VIVA — site estático

Site responsivo em HTML, CSS e JavaScript puro. Não precisa de npm, compilação ou servidor próprio para a primeira versão.

## Arquivos
- `index.html` — estrutura da página.
- `styles.css` — identidade visual preta e vermelha, responsiva.
- `app.js` — desafios, XP, níveis, conquistas, ferramentas e armazenamento local.

## Executar localmente
Abra `index.html` no navegador. Para testar como site, também pode usar a extensão Live Server no VS Code.

## Publicar no Cloudflare Pages pelo GitHub
1. Crie um repositório no GitHub chamado `viva-site`.
2. Envie os três arquivos (`index.html`, `styles.css`, `app.js`) e este README para a raiz do repositório.
3. No Cloudflare, abra **Workers & Pages → Create → Pages → Connect to Git**.
4. Autorize o GitHub e selecione `viva-site`.
5. Framework preset: **None**.
6. Build command: deixe vazio.
7. Build output directory: `/` (raiz do projeto).
8. Clique em **Save and Deploy**.

## O que funciona nesta versão
- Desafio diário baseado na data local.
- XP, níveis, sequência de dias e conquistas.
- Calculadora, temporizador de foco, gerador de ideias.
- Lista de tarefas, bloco de notas e ajuda rápida.
- Perfil local e mural local.
- Persistência com `localStorage`.

## Limites importantes desta primeira versão
Os dados ficam no navegador/dispositivo. O mural não é público e não existe login sincronizado entre aparelhos. Para uma comunidade real, contas, moderação e dados compartilhados, a próxima etapa é adicionar uma API (Cloudflare Workers) e banco D1. Não coloque segredos ou chaves privadas no JavaScript do navegador.

## Personalização
- Desafios: array `challenges` em `app.js`.
- Cores: variáveis CSS no início de `styles.css`.
- Nome e descrição: `index.html`.