---
title: Unidade 6 â€” CSS: O que Ã© e para que serve
parent: Primeiros Passos na Web
nav_order: 6
---
# Unidade 6 â€” CSS: O que Ã© e para que serve

**Objetivo:** Explicar o papel do CSS na separaÃ§Ã£o entre estrutura (HTML) e apresentaÃ§Ã£o visual, e conectar um arquivo `.css` externo a uma pÃ¡gina HTML.

## HTML sem CSS x HTML com CSS

Sem CSS, uma pÃ¡gina HTML Ã© conteÃºdo estruturado, mas sem cor, sem fonte escolhida, sem layout â€” funcional, mas sem nenhuma personalidade visual. O CSS entra exatamente para resolver isso: cores, tipografia, espaÃ§amento e posicionamento.

## TrÃªs formas de aplicar CSS (e qual usar)

| Forma | Como se escreve | Quando usar |
|---|---|---|
| Inline | `<p style="color: blue;">texto</p>` | Nunca, exceto testes rapidÃ­ssimos â€” mistura estrutura e estilo no mesmo lugar |
| Interna | `<style>` dentro do `<head>` | Para pÃ¡ginas Ãºnicas e pequenas |
| **Externa** | Arquivo `.css` separado, ligado com `<link>` | **A forma profissional â€” Ã© a que vamos usar daqui em diante** |

## Conectando o CSS externo Ã  sua pÃ¡gina

VocÃª jÃ¡ tem o arquivo `css/style.css` criado desde a Unidade 2. No `<head>` do seu `index.html`, logo depois do `<title>`, adicione:

```html
<link rel="stylesheet" href="css/style.css">
```

No arquivo `css/style.css`, digite:

```css
p {
  color: blue;
  font-size: 18px;
}
```

## Testando a ligaÃ§Ã£o

1. Salve **os dois arquivos** (`index.html` e `css/style.css`) â€” `Ctrl+S` em cada aba aberta
2. Olhe o navegador (Live Server): todos os parÃ¡grafos `<p>` da pÃ¡gina devem ficar **azuis** e com fonte um pouco maior
3. Se nada mudou, confira, nessa ordem:
   - O caminho no `href` estÃ¡ exatamente `css/style.css` (respeitando maiÃºsculas/minÃºsculas)?
   - O arquivo `style.css` estÃ¡ mesmo dentro da pasta `css/`, e nÃ£o na raiz do projeto?
   - VocÃª salvou os dois arquivos, nÃ£o sÃ³ um deles?

## Por que a forma externa Ã© a profissional

MantÃ©m o HTML limpo (sÃ³ estrutura) e o CSS reutilizÃ¡vel â€” o mesmo arquivo `style.css` pode ser ligado a vÃ¡rias pÃ¡ginas do mesmo site (uma pÃ¡gina "sobre", uma "contato", etc.), garantindo visual consistente sem repetir cÃ³digo.

## ðŸŽ¥ VÃ­deo de apoio

- IntroduÃ§Ã£o ao CSS faz parte do MÃ³dulo 1 do Curso em VÃ­deo: https://www.youtube.com/playlist?list=PLHz_AreHm4dkZ9-atkcmcBaMZdmLHft8n

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Pegue a pÃ¡gina que vocÃª criou na Unidade 4 e ligue o arquivo `css/style.css` a ela, exatamente como mostrado acima.
2. No `style.css`, altere a cor de um `<h1>` (crie uma regra `h1 { color: ... }`) e o tamanho da fonte dos parÃ¡grafos.
3. Confirme visualmente as duas mudanÃ§as no navegador antes de seguir em frente.

