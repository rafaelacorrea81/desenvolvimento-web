---
title: Unidade 8 â€” Publicando com GitHub Pages
parent: GitHub e VS Code
nav_order: 8
---
# Unidade 8 â€” Publicando com GitHub Pages

**Objetivo:** Publicar um site estÃ¡tico gratuitamente utilizando o GitHub Pages, passo a passo, sem travar.

## PrÃ©-requisito

VocÃª jÃ¡ precisa ter um repositÃ³rio no GitHub com os arquivos do seu site (Unidade 5).

## Passo a passo

1. Abra o repositÃ³rio do seu site em **github.com**
2. No menu superior do repositÃ³rio, clique em **Settings**
3. No menu lateral esquerdo, clique em **Pages**
4. Em **"Build and deployment"**, no campo **Source**, escolha a fonte:
   - **Deploy from a branch** â€” mais simples, recomendado para este material
   - **GitHub Actions** â€” para projetos com processo de build (React, Vue, etc.), fora do escopo aqui
5. Com **"Deploy from a branch"** selecionado, escolha a branch **main** e a pasta **`/ (root)`**
6. Clique em **Save**
7. Aguarde 1 a 3 minutos e recarregue a pÃ¡gina (F5) â€” uma faixa verde aparece no topo com o link do site:
   ```
   https://seu-usuario.github.io/nome-do-repositorio/
   ```

## Se o link der erro 404

Aguarde mais 1 a 2 minutos (o GitHub ainda estÃ¡ processando a primeira publicaÃ§Ã£o) e recarregue. Se persistir depois de 5 minutos, confirme que a branch selecionada no passo 5 Ã© a mesma onde estÃ£o os arquivos (`main`) e que existe um `index.html` na raiz do repositÃ³rio.

## O caso especial do domÃ­nio raiz

Se o repositÃ³rio se chamar **exatamente** `seu-usuario.github.io`, o site fica disponÃ­vel direto na raiz (`https://seu-usuario.github.io/`), sem o caminho extra do nome do repositÃ³rio.

## Cuidado com links internos

> âš ï¸ Links que comeÃ§am com `/` (barra) podem quebrar no GitHub Pages, porque o site nÃ£o fica na raiz do domÃ­nio, e sim em um subcaminho (`/nome-do-repositorio/`). Prefira caminhos **relativos**, como `./css/estilos.css` ou `css/estilos.css` (sem barra no inÃ­cio).

## Atualizando o site depois de publicado

Basta repetir o fluxo do dia a dia do Git: `git add .` â†’ `git commit -m "..."` â†’ `git push`. O GitHub Pages atualiza sozinho, alguns minutos depois de cada push na branch configurada â€” nÃ£o Ã© preciso repetir a configuraÃ§Ã£o de Settings â†’ Pages.

## ðŸŽ¥ VÃ­deo de apoio

- Publicando um site com GitHub Pages: https://www.youtube.com/watch?v=9iZ-xRiF62Q

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Publique um projeto seu com o GitHub Pages, seguindo os 7 passos acima.
2. Acesse o link final em uma **aba anÃ´nima** do navegador, para confirmar que o site estÃ¡ realmente pÃºblico (nÃ£o aparecendo sÃ³ porque vocÃª estÃ¡ logado).
3. Altere algo no `index.html`, faÃ§a o fluxo `git add` â†’ `git commit` â†’ `git push`, aguarde 2 minutos e recarregue o link pÃºblico para confirmar que a mudanÃ§a chegou atÃ© lÃ¡.

