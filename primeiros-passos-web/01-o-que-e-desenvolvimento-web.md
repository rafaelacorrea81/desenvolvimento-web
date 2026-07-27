---
title: Unidade 1 â€” O que Ã© Desenvolvimento Web
parent: Primeiros Passos na Web
nav_order: 1
---
# Unidade 1 â€” O que Ã© Desenvolvimento Web

**Objetivo:** Diferenciar front-end de back-end e reconhecer as trÃªs linguagens fundamentais que constroem qualquer pÃ¡gina da web.

## Antes de comeÃ§ar

VocÃª nÃ£o precisa de nenhum programa instalado para esta unidade. Ã‰ sÃ³ leitura e reflexÃ£o â€” a parte prÃ¡tica de instalaÃ§Ã£o comeÃ§a na Unidade 2.

## O que Ã© a internet e o que Ã© a web

A **internet** Ã© a infraestrutura fÃ­sica: cabos submarinos, roteadores, antenas e servidores espalhados pelo mundo, todos conectados entre si. A **web** Ã© uma das formas de usar essa infraestrutura â€” um sistema de pÃ¡ginas e documentos interligados por links (por isso o nome "world wide web", teia mundial).

Quando vocÃª digita um endereÃ§o como `www.exemplo.com` no navegador e aperta Enter, acontece nos bastidores, em poucos segundos, esta sequÃªncia:

1. Seu navegador pergunta a um serviÃ§o chamado **DNS** qual Ã© o endereÃ§o numÃ©rico (IP) daquele nome.
2. Seu navegador manda um pedido para o servidor que estÃ¡ naquele endereÃ§o, pedindo a pÃ¡gina.
3. O servidor processa o pedido e devolve os arquivos da pÃ¡gina (HTML, CSS, JavaScript, imagens).
4. Seu navegador monta esses arquivos na tela â€” isso Ã© o que vocÃª vÃª.

## Front-end x Back-end

| | Front-end | Back-end |
|---|---|---|
| **O que Ã©** | Tudo que vocÃª vÃª e com que interage no navegador: texto, imagens, botÃµes, cores | A parte que roda no servidor: processa dados, acessa bancos de dados, decide o que enviar de volta |
| **ConstruÃ­do com** | HTML, CSS e JavaScript | Linguagens como PHP, Python, Node.js, Java, entre outras, + banco de dados |
| **ResponsÃ¡vel por** | ExperiÃªncia do usuÃ¡rio, velocidade de carregamento, acessibilidade, visual | AutenticaÃ§Ã£o, seguranÃ§a, regras de negÃ³cio |
| **Exemplo prÃ¡tico** | O botÃ£o "Comprar" que vocÃª vÃª e clica | O sistema que confere se o produto ainda estÃ¡ em estoque quando vocÃª clica |

## As trÃªs linguagens do front-end

Todo site que vocÃª vÃª no navegador Ã© construÃ­do sobre trÃªs pilares. Cada um tem um papel bem separado dos outros dois:

- **HTML** (HyperText Markup Language) â€” estrutura e conteÃºdo da pÃ¡gina. Ã‰ o esqueleto: tÃ­tulos, parÃ¡grafos, imagens e links, organizados em hierarquia lÃ³gica. Sem HTML, nÃ£o existe pÃ¡gina.
- **CSS** (Cascading Style Sheets) â€” aparÃªncia e layout visual. Controla cores, fontes, espaÃ§amentos e posicionamento. Sem CSS, a pÃ¡gina existe, mas aparece como texto puro, sem nenhum estilo.
- **JavaScript** â€” comportamento e interatividade. Responde a cliques, valida formulÃ¡rios, atualiza conteÃºdo sem recarregar a pÃ¡gina. Sem JavaScript, a pÃ¡gina Ã© estÃ¡tica (sÃ³ mostra, nÃ£o reage).

> ðŸ’¡ **Analogia:** pense em uma casa. HTML Ã© a estrutura de tijolos e cÃ´modos (sem ela nÃ£o existe casa). CSS Ã© a pintura, o piso e a decoraÃ§Ã£o (a casa existe sem isso, mas fica feia e sem identidade). JavaScript Ã© a parte elÃ©trica e automaÃ§Ã£o (portas que abrem sozinhas, luzes que acendem com sensor) â€” a casa funciona sem isso, mas de forma mais limitada.

## O que Ã© um desenvolvedor full-stack?

Um desenvolvedor **full-stack** domina tanto o front-end quanto o back-end â€” consegue construir uma aplicaÃ§Ã£o web de ponta a ponta. Ã‰ uma habilidade valorizada no mercado, mas que exige um caminho gradual: a grande maioria dos profissionais comeÃ§a se especializando em um dos dois lados (geralmente o front-end, por ser mais visual e ter uma curva de aprendizado mais suave no inÃ­cio) antes de expandir para o outro.

## ðŸŽ¥ VÃ­deo de apoio

Se quiser ver esse mesmo conteÃºdo explicado em vÃ­deo, o MÃ³dulo 1 do **Curso em VÃ­deo de HTML5 e CSS3** (professor Gustavo Guanabara) comeÃ§a exatamente por aqui â€” evoluÃ§Ã£o da internet, front-end x back-end e as trÃªs linguagens:

- Playlist completa do MÃ³dulo 1: https://www.youtube.com/playlist?list=PLHz_AreHm4dkZ9-atkcmcBaMZdmLHft8n

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Escolha um site que vocÃª usa com frequÃªncia (rede social, e-commerce, banco). Liste **3 elementos** que vocÃª classificaria como front-end (o que vocÃª vÃª e clica) e **2 processos** que provavelmente acontecem no back-end (o que nÃ£o Ã© visÃ­vel, mas precisa existir para o site funcionar).
2. Sem consultar a tabela acima, escreva de memÃ³ria a diferenÃ§a entre HTML, CSS e JavaScript em uma frase para cada um. Depois compare com o texto e corrija o que faltou.

**NÃ£o avance para a Unidade 2 atÃ© conseguir fazer os dois itens acima sem olhar o material.**

