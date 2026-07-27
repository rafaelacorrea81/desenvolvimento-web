---
title: Unidade 7 â€” CSS: Seletores e Propriedades BÃ¡sicas
parent: Primeiros Passos na Web
nav_order: 7
---
# Unidade 7 â€” CSS: Seletores e Propriedades BÃ¡sicas

**Objetivo:** Aplicar seletores CSS (tag, classe, id) para estilizar elementos especÃ­ficos da pÃ¡gina, sabendo prever qual estilo "vence" quando hÃ¡ conflito.

## Os trÃªs seletores bÃ¡sicos

**Seletor de tag** â€” afeta **todos** os elementos daquele tipo na pÃ¡gina:
```css
p {
  color: gray;
}
```

**Seletor de classe** (usa `.` antes do nome) â€” afeta sÃ³ os elementos que tiverem aquela classe no atributo `class`. Um elemento pode ter vÃ¡rias classes, separadas por espaÃ§o:
```css
.destaque {
  color: red;
  font-weight: bold;
}
```
```html
<p class="destaque">Este parÃ¡grafo Ã© destacado.</p>
```

**Seletor de id** (usa `#` antes do nome) â€” afeta um Ãºnico elemento, especÃ­fico. **Nunca repita o mesmo `id` em dois elementos da mesma pÃ¡gina.**
```css
#titulo-principal {
  text-align: center;
}
```
```html
<h1 id="titulo-principal">Bem-vindo</h1>
```

## Qual estilo "vence"? (especificidade)

Quando mais de uma regra tenta estilizar o mesmo elemento, o CSS segue uma ordem de prioridade, da menor para a maior:

1. Seletor de tag (`p`) â€” menor prioridade
2. Seletor de classe (`.destaque`)
3. Seletor de id (`#titulo-principal`) â€” maior prioridade

Ou seja: se um `<p class="destaque" id="aviso">` tiver cor definida nos trÃªs seletores ao mesmo tempo, a cor do `#aviso` Ã© a que aparece na tela.

> âš ï¸ **AtenÃ§Ã£o:** CSS Ã© sensÃ­vel a maiÃºsculas e minÃºsculas! `.destaque` no CSS **nÃ£o** afeta `class="Destaque"` no HTML â€” sÃ£o considerados nomes diferentes.

## Testando a especificidade na prÃ¡tica

1. No seu `style.css`, crie as trÃªs regras dos exemplos acima
2. No `index.html`, crie um `<p class="destaque" id="titulo-principal">Teste de prioridade</p>`
3. Salve os dois arquivos e veja no navegador: o texto deve ficar **centralizado** (regra do `id`, que vence) e ao mesmo tempo **vermelho e em negrito** (regra da classe, que nÃ£o conflita com a de centralizar) â€” mas se tanto a classe quanto o id tentassem definir a mesma propriedade (por exemplo, `color`), venceria o `id`

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Na sua pÃ¡gina, crie uma classe `.destaque` e aplique-a em **dois** elementos diferentes.
2. Crie um `id` Ãºnico e aplique-o em **um Ãºnico** elemento.
3. FaÃ§a a classe e o id definirem a **mesma propriedade** (por exemplo, `color`) com valores diferentes, no mesmo elemento, e confirme no navegador que o valor do `id` Ã© o que aparece â€” comprovando a ordem de prioridade explicada acima.

