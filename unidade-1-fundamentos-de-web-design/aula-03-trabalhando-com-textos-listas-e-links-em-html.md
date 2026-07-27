---
icon: compass
---

# Aula 03 - Trabalhando com Textos, Listas e Links em HTML

<div><figure><img src="../.gitbook/assets/Designer (1).png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Designer (3).png" alt=""><figcaption></figcaption></figure></div>

_Figura 1. Estrutura HTML, textos, listas, links e navegação entre páginas._

***

## Objetivos da Aula

Ao final desta aula, o estudante deverá ser capaz de:

* Utilizar corretamente elementos textuais em HTML.
* Criar títulos, parágrafos e quebras de linha.
* Construir listas ordenadas e não ordenadas.
* Criar links e sistemas básicos de navegação.
* Desenvolver páginas mais organizadas e informativas.

***

## Revisão da Aula Anterior

Na aula anterior estudamos:

* Estrutura básica do HTML5
* Tag `<html>`
* Tag `<head>`
* Tag `<title>`
* Tag `<body>`
* Títulos e parágrafos
* Estrutura mínima de uma página Web

Hoje vamos aprender a organizar melhor o conteúdo utilizando listas e criar links para navegar entre páginas.

***

## A Importância da Organização do Conteúdo

Quando acessamos um website, esperamos encontrar as informações de forma organizada.

Observe o exemplo:

#### Texto sem organização

```
Produtos
Notebook
Mouse
Teclado
Monitor
Impressora
```

#### Texto organizado

* Notebook
* Mouse
* Teclado
* Monitor
* Impressora

Qual é mais fácil de ler?

A organização da informação é uma das responsabilidades do desenvolvedor Web.

***

## Trabalhando com Títulos

Os títulos ajudam a organizar o conteúdo de uma página.

```html
<h1>Título Principal</h1>

<h2>Subtítulo</h2>

<h3>Subseção</h3>
```

#### Exemplo

```html
<h1>Curso Técnico em Multimídia</h1>

<h2>Disciplina de Desenvolvimento Web</h2>

<h3>HTML5</h3>
```

***

## Trabalhando com Parágrafos

Os parágrafos são utilizados para apresentar blocos de texto.

```html
<p>Este é um parágrafo.</p>
```

Exemplo:

```html
<p>
O HTML é uma linguagem de marcação utilizada para estruturar conteúdos na Web.
</p>
```

***

## Quebras de Linha

Para criar uma quebra de linha utilizamos:

```html
<br>
```

Exemplo:

```html
Nome: João<br>
Curso: Multimídia<br>
Cidade: Vila Velha
```

Resultado:

```
Nome: João
Curso: Multimídia
Cidade: Vila Velha
```

***

## Comentários

Comentários são utilizados para documentar o código.

Eles não aparecem na página.

```html
<!-- Comentário -->
```

Exemplo:

```html
<!-- Início do cabeçalho -->
```

***

## Listas em HTML

As listas são utilizadas para organizar informações.

Existem dois tipos principais:

* Lista Não Ordenada
* Lista Ordenada

***

## Lista Não Ordenada

Utiliza a tag:

```html
<ul>
```

Cada item utiliza:

```html
<li>
```

Exemplo:

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Resultado:

* HTML
* CSS
* JavaScript

***

## Lista Ordenada

Utiliza a tag:

```html
<ol>
```

Exemplo:

```html
<ol>
    <li>Planejamento</li>
    <li>Design</li>
    <li>Desenvolvimento</li>
</ol>
```

Resultado:

1. Planejamento
2. Design
3. Desenvolvimento

***

## Quando Utilizar Cada Tipo?

#### Lista Não Ordenada

Quando a ordem não é importante.

Exemplo:

* Cores
* Tecnologias
* Ferramentas

***

#### Lista Ordenada

Quando existe sequência.

Exemplo:

1. Fazer login.
2. Preencher formulário.
3. Enviar dados.

***

## O Que São Links?

Os links são a base da navegação na Web.

Sem eles a Web não existiria como conhecemos.

Eles permitem:

* Navegar entre páginas.
* Abrir documentos.
* Acessar outros sites.
* Fazer downloads.

***

## A Tag de Link

Utilizamos a tag:

```html
<a>
```

Exemplo:

```html
<a href="https://www.google.com">
Google
</a>
```

***

## Entendendo o href

O atributo:

```html
href
```

indica o endereço de destino.

Exemplo:

```html
<a href="https://www.youtube.com">
YouTube
</a>
```

***

## Link para Outro Site

```html
<a href="https://www.github.com">
Visitar GitHub
</a>
```

***

## Link para Outra Página

Exemplo:

```html
<a href="contato.html">
Página de Contato
</a>
```

Isso permite criar menus dentro do próprio website.

***

## Criando um Menu Simples

Exemplo:

```html
<a href="index.html">Início</a>

<a href="sobre.html">Sobre</a>

<a href="contato.html">Contato</a>
```

***

## Estrutura Completa

Exemplo:

```html
<!DOCTYPE html>

<html>

<head>
    <title>Meu Site</title>
</head>

<body>

<h1>Meu Portfólio</h1>

<p>Bem-vindo ao meu site.</p>

<h2>Tecnologias Estudadas</h2>

<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>

<h2>Links Úteis</h2>

https://www.w3schools.com
W3Schools
</a>

</body>

</html>
```

***

## Demonstração Prática

Criar um arquivo chamado:

```
index.html
```

Contendo:

* Título principal
* Texto de apresentação
* Lista de hobbies
* Lista de tecnologias
* Link para Google
* Link para YouTube

Executar no navegador.

***

## Atividade Prática

### Construindo Meu Perfil

Desenvolver uma página contendo:

#### Dados pessoais

* Nome
* Curso
* Cidade

#### Hobbies

Utilizar lista não ordenada.

#### Objetivos Profissionais

Utilizar lista ordenada.

#### Links

Adicionar:

* Google
* GitHub
* Site da Escola

***

## Exercício Guiado

Responder:

1. Qual a função da tag `<ul>`?
2. Qual a função da tag `<ol>`?
3. Qual a função da tag `<li>`?
4. O que é um hyperlink?
5. Para que serve o atributo `href`?

***

## Exercícios de Fixação

### Questão 1

Explicar a diferença entre listas ordenadas e não ordenadas.

***

### Questão 2

Qual tag é utilizada para criar links?

***

### Questão 3

Qual atributo define o endereço do link?

***

### Questão 4

Por que os links são importantes para a Web?

***

### Questão 5

Criar um exemplo de lista ordenada contendo três itens.

***

### Questão 6

Criar um exemplo de link para Google.

***

## Desafio

Desenvolver uma página chamada:

```
meu-portfolio.html
```

Contendo:

* Título principal
* Breve apresentação
* Lista de habilidades
* Lista de objetivos profissionais
* Menu com três links
* Link para um site externo

***

## Critérios de Acompanhamento

| Critério                               | Pontos |
| -------------------------------------- | -----: |
| Utilizar corretamente textos e títulos |    0,5 |
| Utilizar listas adequadamente          |    0,5 |
| Criar links funcionais                 |    0,5 |
| Organizar o código HTML                |    0,5 |

***

## Resumo

✅ Títulos organizam o conteúdo.

✅ Parágrafos apresentam informações.

✅ Listas ajudam na estruturação dos dados.

✅ Links permitem a navegação entre páginas.

✅ O atributo `href` define o destino do link.

✅ Menus são construídos utilizando links.

***

## Próxima Aula

### Aula 04 - Imagens e Elementos Multimídia

Na próxima aula aprenderemos:

* Inserção de imagens
* Formatos de imagem para Web
* Organização de arquivos
* Áudio e vídeo em HTML
* Boas práticas para conteúdo multimídia
