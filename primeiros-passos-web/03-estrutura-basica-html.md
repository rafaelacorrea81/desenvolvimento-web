---
title: Unidade 3 â€” HTML: Estrutura BÃ¡sica de uma PÃ¡gina
parent: Primeiros Passos na Web
nav_order: 3
---
# Unidade 3 â€” HTML: Estrutura BÃ¡sica de uma PÃ¡gina

**Objetivo:** Descrever a estrutura mÃ­nima obrigatÃ³ria de um documento HTML, o papel de cada parte, e escrever a primeira pÃ¡gina completa sozinho.

## A estrutura mÃ­nima

Todo documento HTML comeÃ§a com a mesma estrutura base. Abra o arquivo `index.html` (da Unidade 2) no VS Code, apague o que tinha e digite exatamente isto:

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha primeira pÃ¡gina</title>
  </head>
  <body>
    <h1>Bem-vindo ao meu site</h1>
    <p>Este Ã© meu primeiro parÃ¡grafo.</p>
  </body>
</html>
```

**O que cada linha faz, em ordem:**

- `<!DOCTYPE html>` â€” a primeira linha do arquivo, sempre. Informa ao navegador que a pÃ¡gina usa o padrÃ£o HTML5. Sem ela, navegadores antigos podem interpretar a pÃ¡gina de forma inconsistente.
- `<html lang="pt-br">` â€” a tag que envolve todo o resto do documento. O atributo `lang="pt-br"` informa o idioma da pÃ¡gina (importante para leitores de tela e para o Google).
- `<head>` â€” metadados e configuraÃ§Ãµes que **nÃ£o aparecem** na tela, sÃ³ na aba do navegador ou nos bastidores.
  - `<meta charset="UTF-8">` â€” define a codificaÃ§Ã£o de caracteres. Sem essa linha, acentos e "Ã§" podem aparecer como sÃ­mbolos estranhos (ex.: "ÃƒÂ§" no lugar de "Ã§").
  - `<meta name="viewport" ...>` â€” instrui o navegador a respeitar a largura real da tela (essencial para celular; veremos isso com detalhe na Unidade 11).
  - `<title>` â€” o texto que aparece na aba do navegador.
- `<body>` â€” todo o conteÃºdo **visÃ­vel** ao usuÃ¡rio fica aqui dentro: tÃ­tulos, textos, imagens, tudo.

## Testando no navegador

1. Salve o arquivo (`Ctrl+S`)
2. Se o Live Server ainda estiver aberto de uma aba anterior, ela jÃ¡ deve ter atualizado sozinha. Se nÃ£o, clique com o botÃ£o direito no `index.html` â†’ **Open with Live Server**
3. VocÃª deve ver, na pÃ¡gina: o tÃ­tulo **"Bem-vindo ao meu site"** em destaque (grande e em negrito, porque `<h1>` Ã© um tÃ­tulo) e, abaixo, o texto "Este Ã© meu primeiro parÃ¡grafo." em tamanho normal
4. Olhe tambÃ©m a **aba do navegador**: deve mostrar o texto "Minha primeira pÃ¡gina" â€” esse Ã© o efeito do `<title>`

Se a pÃ¡gina aparecer **em branco**, veja a Unidade 14 (Erros Comuns) antes de continuar.

## Como as tags funcionam

Quase toda tag HTML vem em par: uma de abertura (`<p>`) e uma de fechamento (`</p>`, com a barra `/`), com o conteÃºdo entre elas. Esquecer o fechamento Ã© o erro mais comum de quem estÃ¡ comeÃ§ando â€” e o navegador, na maioria das vezes, **nÃ£o mostra mensagem de erro nenhuma**, ele simplesmente renderiza de um jeito estranho (por exemplo, o texto de um parÃ¡grafo "vazando" para dentro de outro).

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Adicione, dentro do `<body>`, mais um `<h1>` e dois `<p>` falando sobre vocÃª (nome, o que estuda, um hobby).
2. Salve e confira no navegador se os quatro elementos aparecem na ordem certa, de cima para baixo.
3. Agora provoque um erro de propÃ³sito: apague sÃ³ a barra `/` do fechamento de um dos `<p>` (deixe `<p>` sem fechar). Salve e observe o que muda na pÃ¡gina â€” normalmente o texto seguinte "gruda" no texto de dentro daquele parÃ¡grafo.
4. Corrija o erro e confirme que a pÃ¡gina volta ao normal antes de seguir para a prÃ³xima unidade.

**NÃ£o avance para a Unidade 4 atÃ© completar os 4 passos acima e ver a diferenÃ§a visual do passo 3 com os prÃ³prios olhos.**

