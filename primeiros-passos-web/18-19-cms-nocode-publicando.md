---
title: Unidades 18 e 19 â€” CMS, No-Code e Publicando seu Primeiro Site
parent: Primeiros Passos na Web
nav_order: 18
---
# Unidades 18 e 19 â€” CMS, No-Code e Publicando seu Primeiro Site

**Objetivo:** Reconhecer alternativas no-code/CMS ao desenvolvimento manual e publicar um site prÃ³prio usando GitHub Pages, do inÃ­cio ao fim.

## Nem tudo precisa ser construÃ­do do zero

| Ferramenta | O que Ã© |
|---|---|
| **WordPress** | CMS mais usado do mundo, ideal para blogs e sites com banco de dados |
| **Wix / Canva Sites** | Editores visuais de arrastar e soltar â€” zero cÃ³digo necessÃ¡rio |
| **Google Sites** | Gratuito, simples, integrado ao ecossistema Google |

Essas ferramentas sÃ£o Ã³timas para quem precisa de um site rÃ¡pido sem programar. O que vocÃª aprendeu nesta apostila Ã© o que roda **por baixo** delas e permite personalizar alÃ©m do que os editores visuais oferecem.

## Publicando com GitHub Pages â€” passo a passo completo

PrÃ©-requisito: vocÃª jÃ¡ enviou seu projeto para o GitHub na Unidade 15.

1. Abra o repositÃ³rio do seu site em **github.com** (na sua conta)
2. No menu superior do repositÃ³rio, clique em **Settings**
3. No menu lateral esquerdo, clique em **Pages**
4. Em **"Build and deployment"**, no campo **Source**, verifique se estÃ¡ selecionado **"Deploy from a branch"**
5. Logo abaixo, no seletor de branch, escolha **main** e, na pasta, deixe **`/ (root)`**
6. Clique em **Save**
7. Aguarde de 1 a 3 minutos. Recarregue a pÃ¡gina de Settings â†’ Pages: deve aparecer uma faixa verde no topo com o link do seu site, no formato:
   ```
   https://seu-usuario.github.io/nome-do-repositorio/
   ```
8. Clique no link para conferir â€” se aparecer um erro "404", aguarde mais um minuto e tente de novo (o GitHub ainda estÃ¡ processando)

> âš ï¸ Se o repositÃ³rio se chamar exatamente `seu-usuario.github.io`, o site fica na raiz do domÃ­nio, sem o caminho extra do nome do repositÃ³rio.

## Se vocÃª atualizar o site depois

Sempre que quiser publicar uma nova versÃ£o: repita o fluxo curto da Unidade 15 (`git add .` â†’ `git commit -m "..."` â†’ `git push`). O GitHub Pages atualiza sozinho, poucos minutos depois de cada push na branch `main` â€” nÃ£o Ã© preciso repetir a configuraÃ§Ã£o de Settings â†’ Pages.

## ðŸŽ¥ VÃ­deo de apoio

- Como publicar seu site com GitHub Pages: https://www.youtube.com/watch?v=9iZ-xRiF62Q

## ParabÃ©ns! ðŸŽ‰

Ao publicar seu primeiro site, vocÃª concluiu a jornada completa: do HTML bÃ¡sico atÃ© a web real. Agora Ã© hora de praticar, experimentar e criar seus prÃ³prios projetos.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Publique com o GitHub Pages qualquer um dos projetos construÃ­dos ao longo desta apostila, seguindo os 8 passos acima.
2. Abra o link final em uma aba anÃ´nima do navegador (para garantir que estÃ¡ realmente pÃºblico, nÃ£o sÃ³ visÃ­vel para vocÃª).
3. Compartilhe o link com o professor e com pelo menos uma pessoa fora da turma, pedindo um feedback rÃ¡pido sobre a primeira impressÃ£o do site.

