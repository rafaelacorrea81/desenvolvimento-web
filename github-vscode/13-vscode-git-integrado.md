---
title: Unidade 13 â€” VS Code + Git Integrados
parent: GitHub e VS Code
nav_order: 13
---
# Unidade 13 â€” VS Code + Git Integrados

**Objetivo:** Utilizar o painel Source Control do VS Code para fazer stage, commit e push sem sair do editor, e conectar sua conta GitHub Ã  interface.

## Conectando sua conta GitHub ao VS Code

1. Clique no Ã­cone de perfil no canto **inferior esquerdo** da janela do VS Code (ou vÃ¡ em **Arquivo â†’ PreferÃªncias â†’ Contas**)
2. Escolha **"Sign in with GitHub"**
3. Uma aba do navegador abre pedindo autorizaÃ§Ã£o â€” clique em **Authorize**
4. Volte ao VS Code: o Ã­cone de perfil agora mostra sua foto/usuÃ¡rio do GitHub

A partir daqui, toda operaÃ§Ã£o de push/pull feita pela interface do VS Code se autentica sozinha, sem pedir usuÃ¡rio/senha depois.

## O painel Source Control

Abra com o Ã­cone de ramificaÃ§Ã£o na barra lateral, ou `Ctrl+Shift+G` (Windows/Linux) / `Cmd+Shift+G` (Mac).

| Elemento | O que mostra |
|---|---|
| Lista de arquivos modificados | Cada arquivo alterado aparece com uma letra: `M` (modified), `A` (added), `D` (deleted) |
| BotÃ£o `+` ao lado de cada arquivo | Equivalente a `git add` naquele arquivo especÃ­fico, sem digitar comando nenhum |
| Caixa de texto no topo do painel | Onde vocÃª escreve a mensagem do commit |
| Ãcone de check (âœ“) ou `Ctrl+Enter` | Confirma o commit dos arquivos em stage |

## Publicando um projeto novo direto pela interface

Se vocÃª abriu uma pasta que **ainda nÃ£o Ã©** um repositÃ³rio Git:

1. VÃ¡ no painel Source Control (`Ctrl+Shift+G`)
2. Clique em **"Publish to GitHub"** (o VS Code detecta que a pasta nÃ£o estÃ¡ versionada e sugere isso)
3. Escolha se o repositÃ³rio serÃ¡ pÃºblico ou privado
4. O VS Code cria o repositÃ³rio no GitHub **e jÃ¡ faz o primeiro push sozinho** â€” sem precisar digitar `git init`, `git remote add origin` ou `git push` manualmente

## Fluxo do dia a dia pela interface

1. Modifique um arquivo e salve
2. Ele aparece na lista de modificados no painel Source Control
3. Clique no `+` ao lado do arquivo (stage) â€” ou passe o mouse sobre "Changes" e clique no `+` para dar stage em tudo de uma vez
4. Escreva a mensagem na caixa de texto
5. Aperte `Ctrl+Enter` (ou clique no âœ“) para commitar
6. Clique em **"Sync Changes"** (ou nos Ã­cones de seta, no rodapÃ©) para fazer `pull` e `push` juntos

## GitLens â€” indo alÃ©m

Com a extensÃ£o GitLens instalada (Unidade 10), cada linha de cÃ³digo passa a mostrar, discretamente ao final da linha, quem foi o autor da Ãºltima alteraÃ§Ã£o e quando ela ocorreu â€” Ãºtil para entender o histÃ³rico de um arquivo sem sair do editor nem digitar `git log`.

## Por que aprender o terminal mesmo tendo a interface grÃ¡fica

A interface Ã© Ã³tima para o dia a dia, mas os comandos de terminal (Unidades 2 a 6) funcionam em **qualquer** editor e em servidores sem interface grÃ¡fica â€” e entender o que cada comando faz ajuda a entender o que a interface estÃ¡ fazendo por trÃ¡s dos botÃµes, principalmente quando algo dÃ¡ errado e a mensagem de erro aparece sÃ³ no terminal.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Conecte sua conta GitHub ao VS Code, seguindo os 4 passos da primeira seÃ§Ã£o.
2. No projeto que vocÃª jÃ¡ versionou (Unidades 3 e 5), modifique um arquivo e faÃ§a o commit **inteiramente** pelo painel Source Control (sem digitar nenhum comando `git` no terminal).
3. Envie ao GitHub tambÃ©m pela interface, clicando em "Sync Changes" ou no botÃ£o de push.
4. Confirme no site do GitHub que o commit feito pela interface aparece no histÃ³rico, com a mensagem que vocÃª escreveu.

