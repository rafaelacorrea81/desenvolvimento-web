---
title: Unidade 11 â€” VS Code: Atalhos e Produtividade
parent: GitHub e VS Code
nav_order: 11
---
# Unidade 11 â€” VS Code: Atalhos e Produtividade

**Objetivo:** Aplicar atalhos de teclado do VS Code para escrever e navegar pelo cÃ³digo com mais velocidade.

## Tabela de atalhos essenciais

| AÃ§Ã£o | Windows/Linux | Mac |
|---|---|---|
| Salvar o arquivo | `Ctrl+S` | `Cmd+S` |
| Comentar/descomentar a linha atual | `Ctrl+/` | `Cmd+/` |
| Desfazer | `Ctrl+Z` | `Cmd+Z` |
| Formatar o documento inteiro | `Shift+Alt+F` | `Shift+Option+F` |
| Abrir arquivo rapidamente pelo nome | `Ctrl+P` | `Cmd+P` |
| Paleta de comandos (busca qualquer aÃ§Ã£o) | `Ctrl+Shift+P` | `Cmd+Shift+P` |
| Seleciona a prÃ³xima ocorrÃªncia da palavra (multi-cursor) | `Ctrl+D` | `Cmd+D` |
| Cria um cursor extra no ponto clicado | `Alt+Clique` | `Option+Clique` |
| Insere uma nova linha **abaixo**, mesmo com o cursor no meio da linha atual | `Ctrl+Enter` | `Cmd+Enter` |
| Insere uma nova linha **acima**, mesmo com o cursor no meio da linha atual | `Ctrl+Shift+Enter` | `Cmd+Shift+Enter` |
| Move a linha atual para cima/para baixo | `Alt+â†‘` / `Alt+â†“` | `Option+â†‘` / `Option+â†“` |
| Abre/fecha o terminal integrado | `` Ctrl+` `` | `` Ctrl+` `` |

## Quebra de linha sem precisar ir atÃ© o final da linha

O atalho comum de "Enter" sÃ³ funciona bem quando o cursor jÃ¡ estÃ¡ no final da linha â€” se ele estiver no meio de um trecho, o Enter normal **quebra o texto ali mesmo**, em vez de criar uma linha nova limpa. Para isso, o VS Code tem um atalho dedicado:

- `Ctrl+Enter` (ou `Cmd+Enter` no Mac) â€” insere uma linha nova **abaixo** da atual, e jÃ¡ posiciona o cursor nela, nÃ£o importa em que ponto da linha vocÃª estava
- `Ctrl+Shift+Enter` (ou `Cmd+Shift+Enter`) â€” faz o mesmo, mas insere a linha **acima**

Exemplo prÃ¡tico: se o cursor estiver no meio de uma linha de CSS (ex.: entre `color` e `blue;`) e vocÃª quiser abrir uma linha nova logo abaixo sem quebrar o que jÃ¡ estava escrito, use `Ctrl+Enter` em vez do Enter comum.

## A Paleta de Comandos â€” o atalho mais poderoso

Aperte `Ctrl+Shift+P` (ou `Cmd+Shift+P`) e uma caixa de busca aparece no topo da tela. Digite parte do nome de **qualquer** aÃ§Ã£o do editor â€” nÃ£o precisa saber onde ela fica no menu. Exemplo: digite "format" para achar "Format Document", ou "theme" para achar "Preferences: Color Theme".

## Praticando multi-cursor

1. Abra um arquivo CSS com pelo menos duas classes com o mesmo nome repetido em lugares diferentes (ex.: `.card` aparecendo em 3 regras diferentes)
2. Clique duas vezes sobre a palavra `card` para selecionÃ¡-la
3. Aperte `Ctrl+D` (ou `Cmd+D`) repetidas vezes â€” a cada aperto, a prÃ³xima ocorrÃªncia da palavra Ã© adicionada Ã  seleÃ§Ã£o
4. Digite um novo nome â€” **todas** as ocorrÃªncias selecionadas mudam ao mesmo tempo

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Em um arquivo CSS com vÃ¡rias classes repetidas, use `Ctrl+D` (ou `Cmd+D`) para selecionar todas as ocorrÃªncias de um nome de classe e renomeie todas ao mesmo tempo.
2. Use `Shift+Alt+F` (ou `Shift+Option+F`) para formatar o arquivo inteiro de uma vez.
3. Abra a Paleta de Comandos (`Ctrl+Shift+P`) e busque por "theme" â€” experimente trocar o tema de cores do editor sÃ³ para praticar a busca.

