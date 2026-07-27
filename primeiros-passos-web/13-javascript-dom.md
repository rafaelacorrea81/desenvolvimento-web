---
title: Unidade 13 â€” JavaScript: Interagindo com a PÃ¡gina
parent: Primeiros Passos na Web
nav_order: 13
---
# Unidade 13 â€” JavaScript: Interagindo com a PÃ¡gina

**Objetivo:** Selecionar elementos HTML com JavaScript e alterar seu conteÃºdo em resposta a um evento, sem recarregar a pÃ¡gina.

## Manipulando o DOM

**DOM** (Document Object Model) Ã© a representaÃ§Ã£o da sua pÃ¡gina que o JavaScript consegue "enxergar" e modificar. No `index.html`, substitua o botÃ£o da unidade anterior por:

```html
<p id="saudacao">OlÃ¡!</p>
<input type="text" id="campo-nome" placeholder="Digite seu nome">
<button onclick="atualizarSaudacao()">Atualizar</button>

<script>
  function atualizarSaudacao() {
    const nome = document.querySelector("#campo-nome").value;
    document.querySelector("#saudacao").textContent = "OlÃ¡, " + nome + "!";
  }
</script>
```

## O que cada peÃ§a faz

| CÃ³digo | O que faz |
|---|---|
| `document.querySelector("#campo-nome")` | Localiza, na pÃ¡gina, o elemento com `id="campo-nome"` |
| `.value` | LÃª o valor **digitado** pelo usuÃ¡rio dentro daquele campo (sÃ³ funciona em `input`/`textarea`) |
| `document.querySelector("#saudacao")` | Localiza o elemento com `id="saudacao"` |
| `.textContent = "..."` | Substitui o texto visÃ­vel daquele elemento pelo texto novo |

`document.querySelector()` aceita os mesmos seletores do CSS: `#id` para id, `.classe` para classe, ou o nome de uma tag (`p`, `button`) sem sÃ­mbolo nenhum.

> âš ï¸ **AtenÃ§Ã£o:** `#mensagem` no seletor **nÃ£o** encontra `class="mensagem"` no HTML. Use `#` para id e `.` (ponto) para classe â€” misturar os dois Ã© um dos erros mais comuns nesta unidade.

## Testando

1. Salve e abra no navegador
2. Digite seu nome no campo de texto
3. Clique em "Atualizar"
4. O texto "OlÃ¡!" deve virar "OlÃ¡, [seu nome]!", **sem a pÃ¡gina recarregar** (repare que a URL na barra do navegador nÃ£o muda)

Se nada mudar: abra o Console (F12) e veja se aparece um erro do tipo `Cannot read properties of null` â€” isso normalmente significa que o `id` usado no `querySelector` nÃ£o bate, letra por letra, com o `id` escrito no HTML.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

Crie um "contador de cliques": um `<p id="contador">0</p>` e um botÃ£o que, a cada clique, some 1 ao nÃºmero exibido.

Dica de estrutura â€” a variÃ¡vel que guarda o nÃºmero precisa ficar **fora** da funÃ§Ã£o, senÃ£o ela reinicia em 0 a cada clique:

```js
let cliques = 0;

function incrementar() {
  cliques = cliques + 1;
  document.querySelector("#contador").textContent = cliques;
}
```

Clique no botÃ£o pelo menos 5 vezes e confirme que o nÃºmero exibido sobe de 1 em 1, sem travar em 1 ou reiniciar sozinho.

