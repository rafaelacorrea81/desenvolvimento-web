---
icon: bolt
---

# Aula 02 - Estrutura Básica de um Documento HTML

## Objetivos da Aula

Ao final desta aula, o estudante deverá ser capaz de:

* Compreender a estrutura básica de um documento HTML.
* Identificar as principais tags de uma página Web.
* Construir páginas HTML simples.
* Aplicar conceitos básicos de HTML5.
* Organizar conteúdos utilizando elementos estruturais.

***

## Revisão da Aula Anterior

Na aula anterior estudamos:

* História da Internet
* História da Web
* O que é HTML
* O que é uma linguagem de marcação
* Conceitos iniciais de HTML5
* Introdução à semântica

Nesta aula iremos criar nossas primeiras páginas.

***

## O Que é HTML?

HTML significa:

**HyperText Markup Language**

ou

**Linguagem de Marcação de Hipertexto**

O HTML não é uma linguagem de programação.

O HTML é uma linguagem utilizada para estruturar conteúdos em páginas Web.

***

## Estrutura Básica de um Documento HTML

Todo documento HTML5 possui uma estrutura mínima.

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

***

## Entendendo Cada Parte

### DOCTYPE

```html
<!DOCTYPE html>
```

Informa ao navegador que o documento utiliza HTML5.

***

### HTML

```html
<html>
</html>
```

Representa o documento HTML completo.

Todos os demais elementos ficam dentro dele.

***

### HEAD

```html
<head>
</head>
```

Contém informações sobre a página.

Exemplos:

* título
* descrição
* estilos
* scripts

***

### TITLE

```html
<title>Meu Site</title>
```

Define o nome exibido na aba do navegador.

***

### BODY

```html
<body>
</body>
```

Contém todo o conteúdo visível da página.

Exemplos:

* textos
* imagens
* menus
* tabelas
* formulários

***

## Criando a Primeira Página

Exemplo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Minha Primeira Página</title>
</head>

<body>
    <h1>Olá Mundo!</h1>
    <p>Meu primeiro site.</p>
</body>

</html>
```

***

## Títulos

HTML possui seis níveis de títulos.

```html
<h1>Título Principal</h1>

<h2>Subtítulo</h2>

<h3>Título Menor</h3>

<h4>Título Nível 4</h4>

<h5>Título Nível 5</h5>

<h6>Título Nível 6</h6>
```

***

## Parágrafos

Para criar parágrafos utilizamos:

```html
<p>Este é um parágrafo.</p>
```

Exemplo:

```html
<p>O desenvolvimento web é uma área em constante crescimento.</p>
```

***

## Quebra de Linha

```html
<br>
```

Exemplo:

```html
Linha 1<br>
Linha 2
```

***

## Comentários

Comentários não aparecem para o usuário.

```html
<!-- Comentário -->
```

Exemplo:

```html
<!-- Cabeçalho do site -->
```

***

## Boas Práticas

✅ Utilizar identação.

✅ Manter código organizado.

✅ Utilizar nomes significativos.

✅ Fechar as tags corretamente.

***

## Demonstração Prática

Criar um arquivo denominado:

```
index.html
```

Inserir:

```html
<!DOCTYPE html>
<html>

<head>
    <title>Meu Perfil</title>
</head>

<body>

    <h1>Meu Nome</h1>

    <p>Estudante do curso Técnico em Multimídia.</p>

</body>

</html>
```

Salvar e abrir no navegador.

***

## Atividade Prática

### Minha Primeira Página Web

Desenvolver uma página contendo:

* Nome completo
* Curso
* Cidade
* Um texto de apresentação
* Um título principal
* Dois subtítulos
* Três parágrafos

***

## Exercício Fixação

Responder:

1. O que significa HTML?
2. Qual a função da tag `<head>`?
3. Qual a função da tag `<body>`?
4. Para que serve a tag `<title>`?
5. O que é um documento HTML?

***

## Exercícios de Fixação

### Questão 1

Identificar a função do DOCTYPE.

***

### Questão 2

Explicar a diferença entre HEAD e BODY.

***

### Questão 3

Qual tag é utilizada para criar parágrafos?

***

### Questão 4

Qual tag é utilizada para criar títulos?

***

### Questão 5

Explicar a importância da organização do código.

***

## Desafio

Desenvolver uma página chamada:

```
sobre-mim.html
```

Contendo:

* Nome
* Curso
* Hobbies
* Objetivos profissionais

Aplicando títulos e parágrafos corretamente.

***

## Critérios de Acompanhamento

| Critério                     | Pontos |
| ---------------------------- | -----: |
| Compreender a estrutura HTML |    0,5 |
| Desenvolver página funcional |    0,5 |
| Aplicar corretamente as tags |    0,5 |
| Organizar o código           |    0,5 |

***

## Resumo

✅ HTML é uma linguagem de marcação.

✅ Todo documento HTML possui uma estrutura básica.

✅ O conteúdo visível fica dentro da tag BODY.

✅ Títulos e parágrafos são elementos fundamentais.

✅ A organização do código facilita a manutenção dos projetos.

***

## Próxima Aula

### Aula 03 - Trabalhando com Textos, Listas e Links

Na próxima aula iremos aprender a criar:

* listas
* links
* menus simples
* navegação entre páginas
