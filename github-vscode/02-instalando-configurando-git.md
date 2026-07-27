---
title: Unidade 2 â€” Instalando e Configurando o Git
parent: GitHub e VS Code
nav_order: 2
---
# Unidade 2 â€” Instalando e Configurando o Git

**Objetivo:** Instalar o Git no sistema operacional e configurar identidade (nome e e-mail) usada em todo commit, confirmando cada passo pelo terminal.

## InstalaÃ§Ã£o por sistema operacional

**Windows**
1. Acesse **https://git-scm.com/download/win** â€” o download deve comeÃ§ar automaticamente
2. Abra o instalador baixado
3. Em todas as telas, pode deixar as opÃ§Ãµes padrÃ£o marcadas e clicar em **Next** â€” a Ãºnica tela que vale conferir Ã© a de "Adjusting your PATH environment", onde a opÃ§Ã£o recomendada (geralmente jÃ¡ marcada) Ã© **"Git from the command line and also from 3rd-party software"**
4. Clique em **Install** e, ao final, em **Finish**

**macOS**
- A forma mais simples: abra o **Terminal** e digite `git --version`. Se o Git ainda nÃ£o estiver instalado, o macOS oferece para instalar as "Command Line Tools" automaticamente â€” aceite.
- Alternativa, se vocÃª jÃ¡ usa Homebrew: `brew install git`

**Linux (Debian/Ubuntu)**
```
sudo apt update
sudo apt install git
```

## Confirmando a instalaÃ§Ã£o

Abra um terminal (no VS Code, `Ctrl+\`` ) e digite:

```
git --version
```

**Como saber se deu certo:** aparece uma linha como `git version 2.4x.x.windows.1` (o nÃºmero exato varia). Se aparecer uma mensagem de "comando nÃ£o encontrado", a instalaÃ§Ã£o nÃ£o terminou corretamente ou o terminal precisa ser reaberto (fechar e abrir de novo o VS Code costuma resolver, no Windows).

## Configurando sua identidade

Todo commit fica assinado com um nome e um e-mail. Configure isso **uma Ãºnica vez por computador** â€” vale para todos os projetos:

```
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

Use o mesmo e-mail que vocÃª usa (ou vai usar) na sua conta do GitHub (Unidade 5) â€” isso faz o GitHub reconhecer seus commits como seus, com sua foto de perfil no histÃ³rico.

## Conferindo o que foi salvo

```
git config --list
```

**Como saber se deu certo:** entre as linhas exibidas, devem aparecer `user.name=Seu Nome` e `user.email=seu-email@exemplo.com`, com os valores exatos que vocÃª digitou.

> ðŸ’¡ `--global` aplica a configuraÃ§Ã£o a todos os repositÃ³rios do seu usuÃ¡rio no computador. Sem essa flag, a configuraÃ§Ã£o vale sÃ³ para o repositÃ³rio da pasta atual â€” Ãºtil quando vocÃª usa e-mails diferentes para projetos pessoais e de trabalho.

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Instale o Git seguindo as instruÃ§Ãµes do seu sistema operacional.
2. Rode `git --version` e confirme que aparece um nÃºmero de versÃ£o.
3. Configure seu nome e e-mail com `--global`.
4. Rode `git config --list` e confirme, na tela, que os dois valores aparecem exatamente como vocÃª digitou (sem erros de digitaÃ§Ã£o â€” isso vai aparecer em todo commit que vocÃª fizer daqui para frente).

