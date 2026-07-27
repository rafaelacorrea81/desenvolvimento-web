---
title: Unidade 8 â€” CSS: Cores, Fontes e Box Model
parent: Primeiros Passos na Web
nav_order: 8
---
# Unidade 8 â€” CSS: Cores, Fontes e Box Model

**Objetivo:** Aplicar propriedades de cor, tipografia e o modelo de caixas (margin, padding, border) no espaÃ§amento dos elementos, prevendo o efeito de cada propriedade antes de testar.

## Propriedades na prÃ¡tica

```css
.caixa {
  background-color: #f0f0f0;
  color: #333333;
  font-family: Arial, sans-serif;
  padding: 16px;
  border: 2px solid #999999;
  margin: 20px;
}
```

```html
<div class="caixa">ConteÃºdo dentro da caixa</div>
```

- `background-color` â€” cor de fundo do elemento
- `color` â€” cor do texto
- `font-family` â€” lista de fontes, em ordem de preferÃªncia (se a primeira nÃ£o existir no computador do visitante, o navegador tenta a prÃ³xima; `sans-serif` Ã© uma fonte genÃ©rica de reserva)
- `padding`, `border`, `margin` â€” ver o Box Model abaixo

## O modelo de caixa (Box Model)

Todo elemento HTML Ã©, para o CSS, uma caixa retangular formada por quatro camadas, de dentro para fora:

1. **Content** â€” o texto ou imagem em si
2. **Padding** â€” espaÃ§o interno, entre o conteÃºdo e a borda
3. **Border** â€” a borda visÃ­vel ao redor do elemento
4. **Margin** â€” espaÃ§o externo, que separa o elemento dos vizinhos

**A confusÃ£o mais comum:** padding Ã© espaÃ§o **dentro** da caixa (empurra o conteÃºdo para dentro, afastando-o da borda); margin Ã© espaÃ§o **fora** da caixa (empurra os elementos vizinhos para longe). Os dois parecem "espaÃ§o em branco" visualmente, mas tÃªm efeitos diferentes quando vocÃª tem duas caixas lado a lado.

## Testando a diferenÃ§a entre padding e margin

1. Crie duas `<div class="caixa">` seguidas no HTML, uma embaixo da outra
2. No CSS, deixe sÃ³ o `padding: 16px;` (remova a margin por enquanto) e observe: o espaÃ§o aparece **dentro** de cada caixa, entre o texto e a borda
3. Agora troque para sÃ³ `margin: 20px;` (remova o padding) e observe: o texto encosta na borda, mas as duas caixas ficam mais **separadas** uma da outra
4. Deixe os dois juntos (como no exemplo original) para ver o efeito combinado

## `box-sizing: border-box` â€” um ajuste que evita surpresas

Por padrÃ£o, quando vocÃª define `width: 300px` em um elemento, o padding e a border sÃ£o **somados** a essa largura (a caixa final fica maior que 300px). Uma prÃ¡tica padrÃ£o em projetos profissionais Ã© adicionar, uma vez, no topo do arquivo CSS:

```css
* {
  box-sizing: border-box;
}
```

Isso faz com que padding e border passem a ser **contados dentro** da largura definida â€” a caixa nunca "cresce" alÃ©m do que vocÃª esperava. Adicione essa regra agora no topo do seu `style.css`; ela nÃ£o muda nada visualmente ainda, mas evita dor de cabeÃ§a nas prÃ³ximas unidades (principalmente Flexbox e Grid).

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Adicione `* { box-sizing: border-box; }` no topo do seu `style.css`.
2. Crie uma `.caixa` com `background-color`, `padding`, `border` e `margin` diferentes dos valores do exemplo.
3. Repita o teste do item "Testando a diferenÃ§a entre padding e margin" acima com seus prÃ³prios valores, e escreva (em um comentÃ¡rio no CSS, usando `/* como comentÃ¡rio */`) qual efeito cada propriedade teve, em suas prÃ³prias palavras.

