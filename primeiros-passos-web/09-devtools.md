---
title: Unidade 9 â€” Inspecionando e Depurando no Navegador
parent: Primeiros Passos na Web
nav_order: 9
---
# Unidade 9 â€” Inspecionando e Depurando no Navegador

**Objetivo:** Utilizar as DevTools do navegador para inspecionar elementos, testar CSS ao vivo e identificar erros no console, sem depender de ajuda externa.

## Abrindo as DevTools

Existem trÃªs formas, escolha a que preferir:

- Aperte a tecla **F12**
- Clique com o **botÃ£o direito** em qualquer parte da pÃ¡gina e escolha **"Inspecionar"**
- No Chrome/Edge: menu (trÃªs pontinhos) â†’ **Mais ferramentas â†’ Ferramentas do desenvolvedor**

Um painel se abre, geralmente do lado direito ou embaixo da tela. TrÃªs abas sÃ£o essenciais no dia a dia:

## Aba Elements (ou "Elementos")

Exibe o HTML e o CSS aplicado a cada elemento, lado a lado.

**Como usar:** clique no Ã­cone de seta com o retÃ¢ngulo (canto superior esquerdo do painel DevTools, chamado "selecionar elemento") e depois clique em qualquer parte da sua pÃ¡gina. O painel Elements pula direto para o HTML daquele elemento, e o painel de estilos ao lado mostra **todas as regras de CSS que afetam ele**, incluindo as que perderam por especificidade (aparecem riscadas).

**Experimente agora:** clique duas vezes em um valor de `padding` no painel de estilos e mude o nÃºmero. A pÃ¡gina muda **ao vivo**, na hora â€” mas Ã© sÃ³ uma simulaÃ§Ã£o: some ao recarregar a pÃ¡gina (F5). Isso torna a aba Elements um laboratÃ³rio seguro para testar valores antes de copiÃ¡-los para o arquivo `.css` de verdade.

## Aba Console

Mostra mensagens e **erros de JavaScript em vermelho**. Ã‰ o primeiro lugar a olhar quando um botÃ£o nÃ£o responde ou uma funÃ§Ã£o nÃ£o funciona (vamos usar isso de verdade a partir da Unidade 12).

## Aba Network (ou "Rede")

Lista todos os arquivos que a pÃ¡gina carregou (HTML, CSS, JS, imagens). Se uma imagem nÃ£o aparecer na pÃ¡gina, esta aba mostra uma linha em **vermelho** com o nome do arquivo que falhou â€” Ã³timo para descobrir se o caminho do `src` estÃ¡ errado.

## ðŸŽ¥ VÃ­deo de apoio

- Como inspecionar elementos nas Chrome DevTools: https://www.youtube.com/watch?v=KMZKWCcTkm4

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Abra qualquer pÃ¡gina sua no navegador e abra as DevTools com F12.
2. Na aba **Elements**, selecione um elemento e altere ao vivo sua `background-color` e um valor de `padding`.
3. Recarregue a pÃ¡gina (F5) e confirme que a mudanÃ§a some â€” prova de que a ediÃ§Ã£o na aba Elements Ã© sÃ³ temporÃ¡ria.
4. Abra a aba **Console** e confirme que nÃ£o hÃ¡ nenhuma mensagem em vermelho. Se houver, anote o texto do erro (vamos usar essa habilidade bastante a partir da Unidade 14).

