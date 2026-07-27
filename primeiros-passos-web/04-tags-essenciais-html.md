---
title: Unidade 4 â€” HTML: Tags Essenciais
parent: Primeiros Passos na Web
nav_order: 4
---
# Unidade 4 â€” HTML: Tags Essenciais

**Objetivo:** Utilizar as tags HTML mais comuns para estruturar qualquer pÃ¡gina com tÃ­tulos, parÃ¡grafos, links, imagens e listas.

## TÃ­tulos e texto

HTML tem 6 nÃ­veis de tÃ­tulo, do mais importante ao menos importante: `<h1>` atÃ© `<h6>`. Use apenas **um `<h1>` por pÃ¡gina** (o tÃ­tulo principal) e organize o resto em `<h2>`, `<h3>`, como um sumÃ¡rio.

```html
<h1>TÃ­tulo principal</h1>
<h2>SubtÃ­tulo</h2>
<p>Um parÃ¡grafo.</p>
```

## Links

```html
<a href="https://exemplo.com">Ir para o site</a>
```

- `href` Ã© o endereÃ§o de destino â€” sempre entre aspas.
- Para abrir o link em uma nova aba (Ãºtil para links externos), adicione `target="_blank"`:
  ```html
  <a href="https://exemplo.com" target="_blank">Ir para o site</a>
  ```

## Imagens

```html
<img src="img/logo.png" alt="DescriÃ§Ã£o da imagem">
```

- `<img>` **nÃ£o tem tag de fechamento** â€” Ã© uma das poucas exceÃ§Ãµes.
- `src` Ã© o caminho atÃ© o arquivo. Se a imagem estiver na pasta `img` dentro do seu projeto (como criamos na Unidade 2), o caminho Ã© `img/nome-do-arquivo.png` â€” sem barra no inÃ­cio.
- `alt` descreve a imagem para leitores de tela e aparece caso a imagem nÃ£o carregue. Ã‰ obrigatÃ³rio por acessibilidade e ajuda tambÃ©m no SEO (Unidade 17).

**Onde colocar a imagem de verdade:** copie um arquivo de imagem (`.png` ou `.jpg`) para dentro da pasta `img/` do seu projeto **pelo gerenciador de arquivos do sistema operacional**, antes de referenciÃ¡-lo no `src`. Se o nome do arquivo tiver letra maiÃºscula (`Foto.jpg`) mas vocÃª escrever `foto.jpg` no `src`, a imagem **nÃ£o aparece** â€” isso serÃ¡ revisitado na Unidade 14.

## Listas

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<ol>
  <li>Passo 1</li>
  <li>Passo 2</li>
</ol>
```

- `<ul>` (unordered list) â€” lista com marcadores (bolinhas), quando a ordem nÃ£o importa.
- `<ol>` (ordered list) â€” lista numerada, quando a ordem importa (um passo a passo, por exemplo).
- `<li>` (list item) â€” cada item, sempre dentro de um `<ul>` ou `<ol>`.

## Testando

Monte, dentro do `<body>` do seu `index.html`, uma combinaÃ§Ã£o dos elementos acima e salve. Com o Live Server ativo, confira visualmente:

- O `<h1>` aparece grande e em negrito
- O link aparece sublinhado e azul (cor padrÃ£o do navegador) â€” passe o mouse por cima: o cursor deve virar uma "mÃ£ozinha"
- A imagem aparece (se vocÃª seguiu o passo de copiar o arquivo para `img/`)
- A lista `<ul>` mostra bolinhas; a `<ol>` mostra nÃºmeros

Se a imagem nÃ£o aparecer, clique com o botÃ£o direito na pÃ¡gina â†’ **Inspecionar** â†’ aba **Console** e veja se hÃ¡ uma mensagem de erro em vermelho mencionando o caminho do arquivo (isso Ã© adiantar um pouco da Unidade 9, mas jÃ¡ ajuda a confirmar o caminho certo).

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

Crie uma pÃ¡gina completa sobre um tema Ã  sua escolha (um hobby, um filme, uma cidade) usando, no mÃ­nimo:

- 1 `<h1>`
- 2 `<h2>`
- 3 parÃ¡grafos `<p>`
- 1 lista (`<ul>` ou `<ol>`, sua escolha)
- 1 link externo, com `target="_blank"`
- 1 imagem, com o arquivo de verdade copiado para a pasta `img/` e o atributo `alt` preenchido de forma descritiva (nÃ£o deixe `alt=""` nem `alt="imagem"`)

Salve, veja no navegador com o Live Server, e confirme visualmente cada um dos seis itens antes de seguir para a prÃ³xima unidade.

