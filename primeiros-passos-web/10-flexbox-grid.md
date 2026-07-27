---
title: Unidade 10 â€” Layout Moderno com Flexbox e Grid
parent: Primeiros Passos na Web
nav_order: 10
---
# Unidade 10 â€” Layout Moderno com Flexbox e Grid

**Objetivo:** Organizar elementos lado a lado ou em grade utilizando Flexbox e Grid CSS, sabendo escolher qual dos dois usar em cada situaÃ§Ã£o.

## Flexbox â€” uma dimensÃ£o

Ideal para alinhar itens em **uma** linha ou coluna. Perfeito para menus, barras de navegaÃ§Ã£o e grupos de botÃµes.

```css
.container-flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

```html
<nav class="container-flex">
  <a href="#">InÃ­cio</a>
  <a href="#">Sobre</a>
  <a href="#">Contato</a>
</nav>
```

- `display: flex` â€” transforma o elemento em um "container flexÃ­vel"; todos os filhos diretos (no exemplo, os trÃªs `<a>`) passam a se organizar em linha, automaticamente, um do lado do outro
- `justify-content: space-between` â€” distribui os filhos com espaÃ§o igual entre eles (o primeiro encosta na esquerda, o Ãºltimo na direita)
- `align-items: center` â€” centraliza os filhos verticalmente dentro do container

## Grid â€” duas dimensÃµes

Ideal para criar grades completas, com linhas **e** colunas ao mesmo tempo. Perfeito para galerias, cards e layouts de pÃ¡gina inteira.

```css
.container-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}
```

```html
<div class="container-grid">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
  <div class="card">Card 4</div>
  <div class="card">Card 5</div>
  <div class="card">Card 6</div>
</div>
```

- `display: grid` â€” transforma o elemento em um "container de grade"
- `grid-template-columns: repeat(3, 1fr)` â€” cria 3 colunas de largura igual (`1fr` = "1 fraÃ§Ã£o" do espaÃ§o disponÃ­vel); com 6 filhos, o resultado Ã© 2 linhas de 3 colunas cada, automaticamente
- `gap: 16px` â€” espaÃ§o entre as cÃ©lulas da grade, tanto na horizontal quanto na vertical

## Regra prÃ¡tica para escolher

Pergunte: **"estou organizando em uma direÃ§Ã£o sÃ³, ou preciso controlar linhas e colunas ao mesmo tempo?"** Uma direÃ§Ã£o â†’ Flexbox. Linhas e colunas â†’ Grid. Os dois podem, inclusive, ser combinados no mesmo projeto (um Grid geral de pÃ¡gina, com um Flexbox dentro de uma das cÃ©lulas, por exemplo).

## Testando

1. Crie o menu com Flexbox e a galeria com Grid no seu `index.html` e `style.css`
2. No navegador, redimensione a janela (arraste a borda para deixÃ¡-la mais estreita) e observe: por enquanto, sem media queries (isso vem na prÃ³xima unidade), o layout **nÃ£o se adapta** â€” os 3 cards continuam apertados em telas pequenas. Vamos resolver isso na Unidade 11.

## ðŸŽ¥ VÃ­deo de apoio

- Flexbox na prÃ¡tica (Curso em VÃ­deo): https://www.youtube.com/watch?v=YeGn9nGies0
- CSS Grid Layout na prÃ¡tica (Curso em VÃ­deo): https://www.youtube.com/watch?v=1FKUfMWBcLM

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Crie um menu de navegaÃ§Ã£o horizontal com 4 links usando `display: flex` e `justify-content`.
2. Crie uma galeria de 6 "cards" (podem ser `<div>` coloridas, com `background-color` diferente em cada uma) organizados em 3 colunas com `display: grid`.
3. Troque `grid-template-columns: repeat(3, 1fr)` por `repeat(2, 1fr)` e depois por `repeat(4, 1fr)`, salvando entre cada troca, sÃ³ para ver visualmente o efeito do nÃºmero de colunas.

