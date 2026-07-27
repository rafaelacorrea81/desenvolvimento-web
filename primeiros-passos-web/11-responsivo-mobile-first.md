---
title: Unidade 11 â€” Design Responsivo â€” Mobile-First
parent: Primeiros Passos na Web
nav_order: 11
---
# Unidade 11 â€” Design Responsivo â€” Mobile-First

**Objetivo:** Adaptar o layout de uma pÃ¡gina para diferentes tamanhos de tela usando media queries, testando sem precisar de um celular fÃ­sico.

## A tag viewport Ã© obrigatÃ³ria

VocÃª jÃ¡ adicionou esta linha no `<head>` desde a Unidade 3 â€” ela Ã© o que permite a pÃ¡gina respeitar a largura real da tela do celular, em vez de mostrar uma versÃ£o "encolhida" do site de computador:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Sem essa linha, **nenhuma media query funciona corretamente** em celulares â€” Ã© o erro mais comum de responsividade em quem estÃ¡ comeÃ§ando.

## Mobile-first com media query

A abordagem **mobile-first** define o estilo padrÃ£o pensando na tela pequena primeiro, e usa media queries para **expandir** o layout em telas maiores (o caminho contrÃ¡rio do que a maioria imagina):

```css
/* Layout padrÃ£o: 1 coluna no celular */
.container-grid {
  grid-template-columns: 1fr;
}

/* A partir de 768px: 3 colunas */
@media (min-width: 768px) {
  .container-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

- A regra fora do `@media` vale para **qualquer** tamanho de tela, por padrÃ£o
- `@media (min-width: 768px)` â€” a regra dentro sÃ³ Ã© aplicada quando a largura da tela for **maior ou igual a** 768 pixels (aproximadamente o tamanho de um tablet)

## Testando sem precisar de um celular

1. Abra as DevTools (`F12`)
2. Clique no Ã­cone de celular/tablet no canto superior esquerdo do painel DevTools (chamado "Toggle device toolbar" â€” no Chrome, o atalho Ã© `Ctrl+Shift+M`)
3. No topo do painel que aparece, escolha um aparelho da lista (ex.: "iPhone SE") ou arraste a borda da simulaÃ§Ã£o para mudar a largura manualmente, em pixels, observando o nÃºmero que aparece
4. Reduza a largura para menos de 768px e depois aumente para mais de 768px, observando seu Grid da Unidade 10 mudar de 1 coluna para 3 colunas exatamente na marca dos 768px

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Pegue a galeria de cards da Unidade 10 e torne-a responsiva:
   - 1 coluna em telas menores que 600px (comportamento padrÃ£o, fora de qualquer media query)
   - 2 colunas a partir de 600px
   - 3 colunas a partir de 900px
2. Usando a simulaÃ§Ã£o de dispositivo das DevTools (passo "Testando" acima), confirme visualmente as trÃªs larguras, arrastando a rÃ©gua atÃ© ultrapassar cada um dos dois pontos de quebra (600px e 900px).

