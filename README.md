# Ratoglota (鼠) — Ecossistema Comunitário de Idiomas

Aplicativo Web Progressivo (PWA) de código único para estudo de **9 idiomas** integrado à pasta `10. Idiomas` do Google Drive:
- **Zero emojis**, com identidade visual **Ratoglota** (cabeça de rato vermelho + sinograma `鼠`).
- **Inicia 100% seco (sem perfis pré-prontos e sem dias marcados)**: cada participante cria ou acessa seu próprio `@identificador` para iniciar e manter sua ofensiva (streak).
- **Todos os 6 Regimes de Tempo do Guia `04.1`**: `20 min`, `30 min`, `45 min`, `60 min (1h)`, `120 min (2h em 2 turnos)` e `180 min (3h em 3 turnos)`.
- **Flashcards SRS Integrados (padrão Anki SM-2)** direto no navegador com áudio nativo (`speechSynthesis`) + exportação e importação `.tsv` para qualquer um dos 9 idiomas.
- **Comunidade + Mural de Check-ins (estilo GymRats) + Chat em Grupo**.

## Como Publicar Gratuitamente no GitHub Pages (Sem Vercel)
1. Crie um repositório público no GitHub (ex: `ratoglota`).
2. Envie os arquivos deste `.zip` (`index.html`, `manifest.json`, `sw.js` e os arquivos `.tsv`).
3. No repositório do GitHub, clique em **Settings** -> **Pages** -> em **Branch**, selecione `main` e salve.
4. O site ficará no ar em `https://seu-usuario.github.io/ratoglota/`.

## Como Ativar o Chat, Perfis e Streaks em Tempo Real entre Todos os Amigos
Como o GitHub Pages hospeda arquivos estáticos gratuitos, para que o celular de todos os amigos veja os perfis, ofensivas, check-ins e mensagens do chat ao vivo automaticamente:
1. Acesse [console.firebase.google.com](https://console.firebase.google.com/) com sua conta Google e clique em **Adicionar projeto** (100% gratuito no plano Spark).
2. No menu lateral, clique em **Criação** -> **Realtime Database** -> **Criar banco de dados** -> escolha **Iniciar no modo de teste** (ou defina `.read: true` e `.write: true`).
3. Copie a URL gerada (ex: `https://ratoglota-turma-default-rtdb.firebaseio.com`).
4. No topo do site **Ratoglota**, clique em **Sincronizar Nuvem**, cole essa URL e clique em **Salvar e Sincronizar Agora**. Mande essa mesma URL para seus amigos colarem uma única vez!
