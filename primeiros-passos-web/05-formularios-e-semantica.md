---
title: Unidade 5 â€” HTML: FormulÃ¡rios e SemÃ¢ntica
parent: Primeiros Passos na Web
nav_order: 5
---
# Unidade 5 â€” HTML: FormulÃ¡rios e SemÃ¢ntica

**Objetivo:** Reconhecer tags semÃ¢nticas e criar um formulÃ¡rio simples de coleta de dados, testÃ¡vel no prÃ³prio navegador.

## FormulÃ¡rio bÃ¡sico

```html
<form>
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome">

  <label for="email">E-mail:</label>
  <input type="email" id="email" name="email">

  <button type="submit">Enviar</button>
</form>
```

**Ponto que costuma confundir:** o atributo `for` do `<label>` precisa ser **exatamente igual** ao `id` do `<input>` correspondente (no exemplo, os dois sÃ£o `nome` e depois `email`). Isso conecta rÃ³tulo e campo: ao clicar no texto do label, o cursor vai direto para o campo, e leitores de tela conseguem anunciar corretamente qual campo Ã© qual.

**Tipos de `input` mais usados:**

| `type` | Para que serve | Comportamento especial |
|---|---|---|
| `text` | Texto livre curto (nome, cidade) | Nenhum |
| `email` | E-mail | O navegador valida o formato (precisa ter `@`) antes de enviar |
| `password` | Senha | Os caracteres aparecem como pontos |
| `number` | NÃºmeros | Mostra setinhas para incrementar/decrementar |
| `date` | Data | Mostra um seletor de calendÃ¡rio |

Para um campo de texto **longo** (uma mensagem, por exemplo), use `<textarea>` em vez de `<input>`:

```html
<label for="mensagem">Mensagem:</label>
<textarea id="mensagem" name="mensagem" rows="4"></textarea>
```

## Tags semÃ¢nticas

Tags semÃ¢nticas descrevem o **significado** do conteÃºdo, nÃ£o apenas sua aparÃªncia visualmente. Ajudam navegadores, leitores de tela e buscadores a entender a estrutura da pÃ¡gina:

```html
<header>CabeÃ§alho do site</header>
<nav>Menu de navegaÃ§Ã£o</nav>
<main>ConteÃºdo principal</main>
<footer>RodapÃ©</footer>
```

Uma pÃ¡gina inteira, combinando tudo, fica assim:

```html
<body>
  <header>
    <h1>Nome do Site</h1>
  </header>

  <main>
    <form>
      <!-- formulÃ¡rio de contato aqui -->
    </form>
  </main>

  <footer>
    <p>&copy; 2026 - Todos os direitos reservados</p>
  </footer>
</body>
```

## Testando

1. Salve o arquivo e veja no navegador (Live Server)
2. Clique dentro do campo "Nome" e digite algo
3. Clique no texto do label "E-mail:" (nÃ£o no campo) â€” o cursor deve pular para o campo de e-mail automaticamente, se o `for`/`id` estiverem corretos
4. Digite um e-mail **sem o `@`** no campo de e-mail e clique em "Enviar": o navegador deve mostrar sozinho uma mensagem pedindo para corrigir o formato â€” isso Ã© a validaÃ§Ã£o nativa do `type="email"`, sem nenhuma linha de JavaScript

Se o clique no label nÃ£o pular para o campo certo, confira se o valor de `for` estÃ¡ **idÃªntico, letra por letra**, ao `id` do input (maiÃºsculas/minÃºsculas importam).

## ðŸŽ¥ VÃ­deo de apoio

- FormulÃ¡rios e tags semÃ¢nticas fazem parte do MÃ³dulo 1 e 4 do Curso em VÃ­deo de HTML5/CSS3 (playlist do mÃ³dulo 1, mesma da Unidade 1): https://www.youtube.com/playlist?list=PLHz_AreHm4dkZ9-atkcmcBaMZdmLHft8n

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Construa um formulÃ¡rio de contato completo com campos de nome (`text`), e-mail (`email`) e uma mensagem (`textarea`).
2. Envolva a pÃ¡gina inteira na estrutura semÃ¢ntica: `<header>` (com um tÃ­tulo do site), `<main>` (com o formulÃ¡rio dentro) e `<footer>` (com um texto de rodapÃ©).
3. Teste o clique no label de cada campo e confirme que o cursor pula corretamente.
4. Teste enviar o formulÃ¡rio com o e-mail em formato invÃ¡lido (sem `@`) e confirme que o navegador bloqueia sozinho.

