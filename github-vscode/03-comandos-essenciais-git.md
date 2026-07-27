---
title: Unidade 3 â€” Comandos Essenciais do Git
parent: GitHub e VS Code
nav_order: 3
---
# Unidade 3 â€” Comandos Essenciais do Git

**Objetivo:** Utilizar os comandos bÃ¡sicos do Git para acompanhar o estado de um repositÃ³rio e registrar mudanÃ§as, reconhecendo os trÃªs estados de um arquivo.

## Criando seu primeiro repositÃ³rio de teste

1. Crie uma pasta nova, por exemplo `teste-git`, e abra-a no VS Code (Arquivo â†’ Abrir Pasta)
2. Abra o terminal integrado (`Ctrl+\`` ) e digite:
   ```
   git init
   ```
   **Como saber se deu certo:** aparece a mensagem `Initialized empty Git repository in .../teste-git/.git/`

## Os trÃªs estados de um arquivo

| Estado | O que significa |
|---|---|
| **Modified** | O arquivo foi alterado, mas ainda nÃ£o foi preparado para o commit |
| **Staged** | O arquivo foi adicionado com `git add` e estÃ¡ pronto para entrar no prÃ³ximo commit |
| **Committed** | A mudanÃ§a foi registrada no histÃ³rico do repositÃ³rio com `git commit` |

## Comandos, na ordem em que vocÃª vai usÃ¡-los

```
git status                # mostra o que mudou desde o Ãºltimo commit
git add arquivo.html      # prepara um arquivo especÃ­fico para o commit
git add .                 # prepara todos os arquivos modificados de uma vez
git commit -m "mensagem"  # registra um ponto de salvamento
git log --oneline         # mostra o histÃ³rico de commits, resumido
git diff                  # mostra exatamente o que mudou, linha a linha
```

## Praticando o ciclo completo

1. No terminal, dentro de `teste-git`, digite `git status`. Deve aparecer `No commits yet` e `nothing to commit` (a pasta estÃ¡ vazia).
2. Crie um arquivo `index.html` simples (pode ser sÃ³ `<h1>Teste</h1>`) e salve.
3. Digite `git status` de novo â€” agora o arquivo aparece listado em vermelho, em **"Untracked files"** (nÃ£o rastreado ainda).
4. Digite `git add .` e depois `git status` de novo â€” o arquivo passa para verde, em **"Changes to be committed"** (staged).
5. Digite `git commit -m "Primeiro commit de teste"`.
6. Digite `git status` de novo â€” deve aparecer **"nothing to commit, working tree clean"**, confirmando que tudo foi salvo.
7. Digite `git log --oneline` â€” deve aparecer uma linha com um cÃ³digo curto (hash) e a mensagem "Primeiro commit de teste".

## ðŸŽ¥ VÃ­deo de apoio

- Git e GitHub, tutorial completo (cobre os mesmos comandos na prÃ¡tica): https://www.youtube.com/watch?v=_hZf1teRFNg

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Repita o ciclo dos 7 passos acima em uma pasta de teste sua.
2. Altere o conteÃºdo do `index.html` (mude o texto do `<h1>`), salve, e rode `git diff` **antes** de dar `git add` â€” confirme que aparece, em vermelho, a linha antiga e, em verde, a linha nova.
3. Complete o commit dessa segunda mudanÃ§a e rode `git log --oneline` de novo, confirmando que agora aparecem **duas** linhas de commit.

