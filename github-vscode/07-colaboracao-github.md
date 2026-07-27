---
title: Unidade 7 â€” ColaboraÃ§Ã£o no GitHub
parent: GitHub e VS Code
nav_order: 7
---
# Unidade 7 â€” ColaboraÃ§Ã£o no GitHub

**Objetivo:** Reconhecer os conceitos de Issues, Pull Requests e Fork usados na colaboraÃ§Ã£o em projetos no GitHub, e praticar cada um.

## Os trÃªs conceitos

| Conceito | O que Ã© |
|---|---|
| **Issues** | Um quadro de tarefas, bugs e ideias do projeto. Qualquer pessoa pode abrir uma Issue descrevendo um problema ou sugestÃ£o |
| **Fork** | Uma cÃ³pia completa de um repositÃ³rio de outra pessoa, feita na **sua prÃ³pria conta**, para vocÃª poder modificar sem afetar o original |
| **Pull Request (PR)** | Um pedido formal para que suas mudanÃ§as (de uma branch ou de um fork) sejam incorporadas ao repositÃ³rio original, com espaÃ§o para revisÃ£o e comentÃ¡rios antes de aceitar |

## Abrindo uma Issue

1. No repositÃ³rio de alguÃ©m (ou no seu prÃ³prio), clique na aba **Issues**
2. Clique em **New issue**
3. Escreva um tÃ­tulo curto e, no corpo, descreva o problema ou a sugestÃ£o com detalhes (o que vocÃª esperava que acontecesse x o que de fato acontece, se for um bug)
4. Clique em **Submit new issue**

## Fluxo tÃ­pico de contribuiÃ§Ã£o em projeto de terceiros

1. FaÃ§a um **fork** do repositÃ³rio para a sua conta (botÃ£o **Fork**, no canto superior direito do repositÃ³rio)
2. Clone o fork para sua mÃ¡quina: `git clone https://github.com/seu-usuario/nome-do-fork.git`
3. Crie uma branch para a sua mudanÃ§a: `git checkout -b minha-correcao`
4. FaÃ§a as alteraÃ§Ãµes, `git add .`, `git commit -m "..."` e `git push origin minha-correcao`
5. No GitHub, na pÃ¡gina do seu fork, clique em **Compare & pull request**
6. Escreva um tÃ­tulo e uma descriÃ§Ã£o explicando o que a mudanÃ§a faz, e clique em **Create pull request**

> ðŸ’¡ Em projetos prÃ³prios ou de equipe pequena, geralmente **nÃ£o Ã© preciso fork**: basta criar uma branch direto no repositÃ³rio original e abrir o Pull Request de branch para branch.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Escolha um repositÃ³rio pÃºblico simples no GitHub (pode ser um projeto de exemplo de um colega de turma) e abra uma **Issue** nele descrevendo uma sugestÃ£o de melhoria â€” sem necessariamente implementÃ¡-la.
2. Se possÃ­vel, faÃ§a um fork desse mesmo repositÃ³rio, clone-o, crie uma branch, faÃ§a uma pequena alteraÃ§Ã£o (por exemplo, corrigir um erro de digitaÃ§Ã£o no README) e abra um Pull Request seguindo o fluxo acima.

