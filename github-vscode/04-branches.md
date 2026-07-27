---
title: Unidade 4 â€” Trabalhando com Branches
parent: GitHub e VS Code
nav_order: 4
---
# Unidade 4 â€” Trabalhando com Branches

**Objetivo:** Criar, alternar e mesclar branches para desenvolver funcionalidades sem afetar a versÃ£o principal do projeto.

## O que Ã© uma branch

Uma **branch** (ramo) Ã© uma linha paralela de desenvolvimento. A branch `main` (Ã s vezes chamada `master` em projetos antigos) geralmente representa a versÃ£o estÃ¡vel do projeto. Ao criar uma nova funcionalidade, Ã© comum abrir uma branch separada, testar tudo por lÃ¡, e sÃ³ depois juntar (merge) as mudanÃ§as de volta Ã  `main`.

## Comandos

```
git branch                     # lista as branches existentes (a atual aparece com um *)
git branch nome-da-branch      # cria uma nova branch, sem mudar para ela
git checkout nome-da-branch    # muda para essa branch
git checkout -b nome-da-branch # cria E jÃ¡ muda para a nova branch, em um Ãºnico comando
git switch nome-da-branch      # forma mais nova de trocar de branch (equivalente ao checkout)
git merge nome-da-branch       # traz as mudanÃ§as da branch informada para a branch atual
```

## Praticando, passo a passo

Usando o repositÃ³rio `teste-git` da Unidade 3:

1. `git branch` â€” deve mostrar sÃ³ `* main` (vocÃª estÃ¡ na main, Ãºnico branch existente)
2. `git checkout -b teste-cor` â€” cria e jÃ¡ muda para a nova branch
3. Altere o `index.html`, adicionando um estilo de cor de fundo (pode ser um `<body style="background-color: lightblue;">`, sÃ³ para o teste)
4. `git add .` e `git commit -m "Testa cor de fundo"`
5. `git checkout main` â€” volta para a branch principal; **repare que o arquivo volta ao estado anterior**, sem a cor â€” a mudanÃ§a sÃ³ existe na branch `teste-cor`
6. `git diff main teste-cor` â€” mostra a diferenÃ§a exata entre as duas branches

## Juntando as branches (merge)

Se vocÃª decidir manter a mudanÃ§a:

```
git checkout main
git merge teste-cor
```

Isso traz as mudanÃ§as da `teste-cor` para dentro da `main`.

## Boa prÃ¡tica

Em projetos com mais de uma pessoa, evite trabalhar direto na `main`. Crie uma branch por funcionalidade (ex.: `feature/menu-responsivo`), trabalhe nela, e sÃ³ depois una Ã  `main` â€” isso evita que um trabalho incompleto quebre a versÃ£o estÃ¡vel que outras pessoas estÃ£o usando.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. No repositÃ³rio `teste-git`, crie uma branch chamada `teste-cor` e faÃ§a a mudanÃ§a de cor de fundo, conforme os passos acima.
2. Volte para a `main` e confirme, com `git diff main teste-cor`, que as duas branches estÃ£o diferentes.
3. FaÃ§a o merge da `teste-cor` para a `main` e confirme, abrindo o `index.html`, que a cor de fundo agora aparece tambÃ©m na `main`.

