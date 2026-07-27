---
title: Unidade 14 â€” Erros Comuns e Como Resolver Sozinho
parent: Primeiros Passos na Web
nav_order: 14
---
# Unidade 14 â€” Erros Comuns e Como Resolver Sozinho

**Objetivo:** Aplicar um processo sistemÃ¡tico de diagnÃ³stico para os erros mais frequentes de iniciantes, sem depender de ajuda externa.

Todo programador comete erros â€” a diferenÃ§a estÃ¡ em saber como encontrÃ¡-los. Antes de pedir ajuda a alguÃ©m, passe pelo checklist abaixo, na ordem, procurando o sintoma mais parecido com o que vocÃª estÃ¡ vendo.

## 1. A pÃ¡gina abre em branco

- Confira o **nome e a extensÃ£o** do arquivo no painel Explorer do VS Code. Deve ser exatamente `index.html`. Um erro comum: o Bloco de Notas do Windows salva como `index.html.txt` sem avisar, se vocÃª nÃ£o escolher "Todos os arquivos" ao salvar. Se aparecer `index.html.txt`, renomeie removendo o `.txt` final.
- Confira se vocÃª abriu a pÃ¡gina certa: a URL no navegador deve terminar em `index.html`, nÃ£o em outro nome de arquivo.

## 2. Salvei e nada mudou na tela

- Olhe o canto inferior direito do VS Code: deve aparecer **"Port: 5500"** (ou similar) â€” se aparecer **"Go Live"**, o Live Server estÃ¡ desligado; clique nele para ligar.
- Confirme que vocÃª salvou o arquivo certo (`Ctrl+S`) â€” abas com mudanÃ§as nÃ£o salvas mostram uma bolinha branca no lugar do "x" de fechar, no topo da aba.
- Se o Live Server estiver ligado e ainda assim nÃ£o atualizar, feche a aba do navegador e clique de novo com o botÃ£o direito â†’ "Open with Live Server".

## 3. CSS nÃ£o aplica no elemento

- Abra as DevTools (F12), aba **Elements**, clique no elemento em questÃ£o
- No painel de estilos ao lado, procure sua propriedade: se ela aparecer **riscada**, outra regra com maior especificidade estÃ¡ vencendo (revise a Unidade 7 â€” ordem tag â†’ classe â†’ id)
- Confira se o seletor no CSS bate exatamente com o HTML: `.destaque` sÃ³ funciona com `class="destaque"`, nunca com `class="Destaque"` (maiÃºscula diferente) nem com `id="destaque"`
- Confirme que o `<link rel="stylesheet" href="...">` estÃ¡ apontando para o arquivo certo (Unidade 6)

## 4. JavaScript nÃ£o funciona (botÃ£o nÃ£o faz nada)

- Abra o **Console** (F12) e leia a mensagem em vermelho â€” ela indica o arquivo e o nÃºmero da linha do problema
- Erros mais comuns e o que significam:

| Mensagem no Console | O que normalmente significa | Como corrigir |
|---|---|---|
| `Uncaught ReferenceError: nomeDaFuncao is not defined` | O nome da funÃ§Ã£o no `onclick` do HTML nÃ£o bate com o nome da funÃ§Ã£o no `<script>` | Confira maiÃºsculas/minÃºsculas nos dois lugares |
| `Uncaught TypeError: Cannot read properties of null (reading 'value')` | `document.querySelector("#algo")` nÃ£o encontrou nenhum elemento com esse id | Confira se o `id` no HTML estÃ¡ escrito exatamente igual ao usado no `querySelector` |
| `Uncaught SyntaxError: missing ) after argument list` | Faltou fechar um parÃªntese em alguma linha anterior | Releia a funÃ§Ã£o de cima para baixo contando parÃªnteses abertos e fechados |

## 5. Imagem nÃ£o aparece

- Abra as DevTools, aba **Network**, recarregue a pÃ¡gina (F5) e procure uma linha em vermelho com o nome do arquivo de imagem
- Confira o caminho no atributo `src`: se a imagem estÃ¡ em `img/logo.png`, o `src` deve ser exatamente `img/logo.png` (sem barra `/` no inÃ­cio)
- O nome do arquivo Ã© **sensÃ­vel a maiÃºsculas** em muitos sistemas: `Foto.jpg` Ã© diferente de `foto.jpg`. Renomeie o arquivo ou corrija o `src` para que fiquem idÃªnticos

## 6. Git/GitHub travou pedindo login ou senha no meio de um `git push`

Este ponto Ã© aprofundado no material complementar de GitHub/VS Code, mas o sintoma mais comum: uma janela do navegador abre pedindo para vocÃª autorizar o acesso â€” aceite normalmente. Se em vez disso aparecer um campo de senha no terminal, veja a Unidade 5 do material complementar.

## Regra geral quando nada da lista bate

1. Copie a mensagem de erro exata (do Console ou de onde ela aparecer)
2. Cole em uma busca no Google incluindo a palavra "javascript" ou "html" ou "css" conforme o caso
3. Se a busca nÃ£o ajudar, use um dos vÃ­deos de apoio da unidade relacionada ao problema (por exemplo, volte Ã  Unidade 9 se o problema for de DevTools)

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

Pegue qualquer projeto seu e provoque, de propÃ³sito, cada um dos 5 primeiros erros listados acima, um de cada vez:

1. Renomeie `index.html` para `index.html.txt` e tente abrir com Live Server â€” veja o que acontece, depois desfaÃ§a
2. Desligue o Live Server (clique em "Port: 5500" para virar "Go Live") e mude algo no CSS â€” confirme que nÃ£o atualiza, depois ligue de novo
3. Escreva um seletor de classe com a capitalizaÃ§Ã£o errada de propÃ³sito e confirme, pela aba Elements, que o estilo aparece riscado ou nem aparece
4. Escreva errado o nome de uma funÃ§Ã£o no `onclick` e leia a mensagem de erro exata no Console
5. Troque o `src` de uma imagem para um nome de arquivo que nÃ£o existe e confirme a linha vermelha na aba Network

Pratique encontrar e corrigir cada um usando o checklist â€” sem consultar a soluÃ§Ã£o antes de tentar sozinho por pelo menos 3 minutos em cada item.

