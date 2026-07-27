---
title: Unidade 17 â€” SEO: OtimizaÃ§Ã£o para Mecanismos de Busca
parent: Primeiros Passos na Web
nav_order: 17
---
# Unidade 17 â€” SEO: OtimizaÃ§Ã£o para Mecanismos de Busca

**Objetivo:** Aplicar boas prÃ¡ticas de SEO on-page e compreender como o Google rastreia, indexa e ranqueia uma pÃ¡gina.

## On-page x off-page

- **SEO on-page** â€” otimizaÃ§Ãµes feitas **dentro** do prÃ³prio site: tÃ­tulos, descriÃ§Ãµes, estrutura do HTML, qualidade do conteÃºdo. Ã‰ o foco desta unidade e o que vocÃª jÃ¡ consegue controlar sozinho.
- **SEO off-page** â€” fatores **externos**, como links de outros sites apontando para o seu (backlinks) e menÃ§Ãµes em redes sociais.

## Tags essenciais, no `<head>` da sua pÃ¡gina

```html
<title>Padaria PÃ£o Dourado - Vila Velha, ES</title>
<meta name="description" content="Padaria artesanal com pÃ£es e bolos frescos todo dia.">
```

## Open Graph â€” como o link aparece quando compartilhado

```html
<meta property="og:title" content="Padaria PÃ£o Dourado">
<meta property="og:description" content="PÃ£es e bolos artesanais frescos todo dia.">
<meta property="og:image" content="https://seusite.com.br/img/preview.jpg">
```

Essas trÃªs tags controlam o **tÃ­tulo, descriÃ§Ã£o e imagem** que aparecem quando alguÃ©m cola o link do seu site no WhatsApp, Instagram ou Facebook.

## Boas prÃ¡ticas â€” checklist rÃ¡pido

- [ ] Use apenas **um** `<h1>` por pÃ¡gina, com a palavra-chave principal
- [ ] Escreva `alt` descritivo em **todas** as imagens
- [ ] Site responsivo (mobile-first, Unidade 11) â€” fator de ranqueamento no Google
- [ ] URLs curtas e descritivas
- [ ] Imagens comprimidas (existem ferramentas gratuitas online, como o TinyPNG) para carregamento rÃ¡pido
- [ ] ConteÃºdo original, relevante, escrito para pessoas â€” o Google prioriza conteÃºdo "Ãºtil e confiÃ¡vel", nÃ£o texto feito sÃ³ para agradar o algoritmo
- [ ] Registrar o site no **Google Search Console** (gratuito) para monitorar desempenho e erros

## Como o Google indexa uma pÃ¡gina

1. **Rastreamento (crawling)** â€” robÃ´s automatizados do Google (o Googlebot) percorrem a web seguindo links de pÃ¡gina em pÃ¡gina
2. **IndexaÃ§Ã£o** â€” o conteÃºdo encontrado Ã© analisado e armazenado em um enorme banco de dados
3. **Ranqueamento** â€” a ordem em que as pÃ¡ginas aparecem nos resultados, considerando centenas de fatores: relevÃ¢ncia do conteÃºdo, velocidade do site, quantidade de backlinks e experiÃªncia do usuÃ¡rio (as chamadas Core Web Vitals)

| Fator | Impacto | Como aplicar |
|---|---|---|
| TÃ­tulo da pÃ¡gina `<title>` | Alto | Palavra-chave principal no inÃ­cio, atÃ© 60 caracteres |
| Meta description | MÃ©dio | Resumo atrativo de atÃ© 160 caracteres, com a palavra-chave |
| Velocidade de carregamento | Alto | Comprima imagens, minimize CSS/JS, use cache do navegador |
| Mobile-friendly | Alto | Design responsivo com meta viewport (teste no Google Mobile-Friendly Test) |

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Escolha uma das pÃ¡ginas que vocÃª criou nesta apostila e adicione: um `<title>` descritivo, uma `meta description` de atÃ© 160 caracteres, e as trÃªs tags Open Graph.
2. Verifique se hÃ¡ mais de um `<h1>` na pÃ¡gina (use Ctrl+F no cÃ³digo para contar) e corrija se houver.
3. Confira todas as imagens da pÃ¡gina e confirme que nenhuma tem `alt=""` vazio.

