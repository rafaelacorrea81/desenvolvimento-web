---
title: Unidade 9 â€” VS Code: InstalaÃ§Ã£o e Primeiros Passos
parent: GitHub e VS Code
nav_order: 9
---
# Unidade 9 â€” VS Code: InstalaÃ§Ã£o e Primeiros Passos

**Objetivo:** Instalar o VS Code e reconhecer as Ã¡reas principais da interface, mesmo sem nenhuma experiÃªncia anterior com editores de cÃ³digo.

> Se vocÃª jÃ¡ instalou o VS Code seguindo a Unidade 2 da apostila "Primeiros Passos na Web", pode pular direto para a seÃ§Ã£o "Reconhecendo a interface" abaixo.

## InstalaÃ§Ã£o

1. Acesse **https://code.visualstudio.com**
2. Clique no botÃ£o de download detectado para o seu sistema operacional
3. **Windows:** abra o instalador, aceite os termos, marque **"Adicionar ao PATH"** (geralmente jÃ¡ vem marcada) e clique em Instalar
4. **macOS:** extraia o `.zip` baixado e arraste o Ã­cone para a pasta Aplicativos
5. **Linux:** instale o pacote `.deb` ou `.rpm` baixado, conforme sua distribuiÃ§Ã£o

## Reconhecendo a interface

| Ãrea | O que Ã© |
|---|---|
| **Barra lateral (Activity Bar)** | Coluna de Ã­cones Ã  esquerda: Explorer (arquivos), Busca, Source Control (Git), Debug, ExtensÃµes |
| **Explorer** | Mostra a Ã¡rvore de pastas e arquivos do projeto aberto |
| **Ãrea de ediÃ§Ã£o** | Onde o cÃ³digo Ã© escrito, com abas para mÃºltiplos arquivos abertos ao mesmo tempo |
| **Terminal integrado** | Um terminal completo dentro do prÃ³prio editor, sem precisar abrir outro programa â€” atalho `Ctrl+\`` (Windows/Linux) ou `Cmd+\`` (Mac) |

## Sempre abra a pasta, nÃ£o o arquivo solto

**Arquivo â†’ Abrir Pasta** (nunca **Arquivo â†’ Abrir Arquivo** para comeÃ§ar um projeto). Isso ativa: busca em todos os arquivos do projeto, o painel Source Control funcionando corretamente, e sugestÃµes de caminho de arquivo corretas (por exemplo, ao digitar `src="img/`, o autocomplete sugere os arquivos que realmente existem na pasta `img`).

## Testando o terminal integrado

1. Abra qualquer pasta de projeto
2. Aperte `` Ctrl+` `` para abrir o terminal
3. Digite `git --version` e aperte Enter
4. **Como saber se deu certo:** aparece um nÃºmero de versÃ£o do Git â€” se aparecer erro de "comando nÃ£o encontrado", volte Ã  Unidade 2 (Instalando e Configurando o Git)

## ðŸŽ¥ VÃ­deo de apoio

- InstalaÃ§Ã£o e configuraÃ§Ã£o do VS Code para iniciantes: https://www.youtube.com/watch?v=aQXVGHLXJew

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Instale o VS Code (se ainda nÃ£o tiver).
2. Abra uma pasta de projeto qualquer e identifique, na tela, os quatro elementos da tabela acima (Barra lateral, Explorer, Ãrea de ediÃ§Ã£o, Terminal).
3. Abra o terminal integrado com `` Ctrl+` `` e rode `git --version` dentro dele.

