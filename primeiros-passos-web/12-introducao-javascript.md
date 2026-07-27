---
title: Unidade 12 â€” IntroduÃ§Ã£o ao JavaScript
parent: Primeiros Passos na Web
nav_order: 12
---
# Unidade 12 â€” IntroduÃ§Ã£o ao JavaScript

**Objetivo:** Explicar o papel do JavaScript e escrever uma interaÃ§Ã£o simples com o usuÃ¡rio, confirmando o resultado no navegador.

## O que o JavaScript faz que HTML e CSS nÃ£o fazem

HTML define a estrutura e CSS cuida da aparÃªncia â€” mas nenhum dos dois **reage** a uma aÃ§Ã£o do usuÃ¡rio. JavaScript Ã© a linguagem que torna a pÃ¡gina interativa: responde a cliques, valida formulÃ¡rios, atualiza conteÃºdo sem recarregar a pÃ¡gina.

## Sua primeira interaÃ§Ã£o

No `index.html`, dentro do `<body>`, logo antes de fechar `</body>`, adicione:

```html
<button onclick="mostrarMensagem()">Clique aqui</button>

<script>
  function mostrarMensagem() {
    alert("VocÃª clicou no botÃ£o!");
  }
</script>
```

**Ponto de atenÃ§Ã£o:** a tag `<script>` fica **dentro** do `<body>`, no final â€” nÃ£o no `<head>`. Colocar scripts no final garante que o resto da pÃ¡gina jÃ¡ carregou antes do JavaScript rodar.

## Como funciona, passo a passo

1. **Evento** â€” o usuÃ¡rio clica no botÃ£o; isso dispara o evento `onclick`
2. **FunÃ§Ã£o** â€” o navegador executa a funÃ§Ã£o `mostrarMensagem()`, escrita dentro do `<script>`
3. **Resultado** â€” o navegador exibe uma caixa de alerta (`alert`) com a mensagem

## Testando

1. Salve o arquivo
2. No navegador, clique no botÃ£o "Clique aqui"
3. Deve aparecer uma caixa de diÃ¡logo do prÃ³prio navegador (nÃ£o faz parte do design da pÃ¡gina) com o texto "VocÃª clicou no botÃ£o!" e um botÃ£o "OK"
4. Clique em "OK" para fechar

Se **nada acontecer** ao clicar: abra as DevTools (`F12`), vÃ¡ na aba **Console** e veja se hÃ¡ uma mensagem em vermelho. O erro mais comum aqui Ã© escrever o nome da funÃ§Ã£o errado no `onclick` (por exemplo, `onclick="mostrarmensagem()"` com "m" minÃºsculo, quando a funÃ§Ã£o foi definida como `mostrarMensagem` com "M" maiÃºsculo) â€” JavaScript diferencia maiÃºsculas de minÃºsculas em nomes de funÃ§Ã£o.

## ðŸŽ¥ VÃ­deo de apoio

- IntroduÃ§Ã£o prÃ¡tica ao JavaScript e Ã  DOM: https://www.youtube.com/watch?v=UPD0vts-eMQ

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

Crie um botÃ£o que, ao ser clicado, exiba um `alert` com uma mensagem **diferente** a cada nova tentativa. Dica â€” crie um array com 3 frases e sorteie uma delas com `Math.random()`:

```js
function mostrarMensagem() {
  const frases = ["Boa!", "De novo?", "VocÃª nÃ£o cansa, hein"];
  const indice = Math.floor(Math.random() * frases.length);
  alert(frases[indice]);
}
```

Clique no botÃ£o pelo menos 6 vezes seguidas e confirme que mensagens diferentes aparecem (Ã© normal repetir de vez em quando, jÃ¡ que Ã© aleatÃ³rio).

