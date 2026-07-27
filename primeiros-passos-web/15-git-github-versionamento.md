---
title: Unidade 15 â€” Versionamento com Git e GitHub
parent: Primeiros Passos na Web
nav_order: 15
---
# Unidade 15 â€” Versionamento com Git e GitHub

**Objetivo:** Inicializar um repositÃ³rio Git local, registrar mudanÃ§as com commits e enviÃ¡-las para o GitHub, do zero.

> Esta unidade cobre sÃ³ o suficiente para publicar seu projeto. Se travar em qualquer passo, ou quiser entender cada comando com mais profundidade (branches, `.gitignore`, colaboraÃ§Ã£o), use o livro complementar **"GitHub e VS Code: Conceitos e ConfiguraÃ§Ãµes BÃ¡sicas"** â€” as Unidades 1 a 8 dele cobrem exatamente esse caminho, com muito mais detalhe.

## O que Ã© o Git e o que Ã© o GitHub

O **Git** Ã© um programa que roda no seu computador e cria um histÃ³rico de versÃµes do seu projeto â€” se algo der errado, vocÃª pode voltar a qualquer ponto anterior. O **GitHub** Ã© um serviÃ§o na nuvem que hospeda esse histÃ³rico, permitindo compartilhÃ¡-lo e fazer backup.

## Passo 1 â€” Instalar o Git (se ainda nÃ£o tiver)

1. Acesse **https://git-scm.com/downloads**
2. Baixe a versÃ£o do seu sistema operacional e instale com as opÃ§Ãµes padrÃ£o do instalador (pode clicar em "Next" em todas as telas, sem mudar nada)
3. Para confirmar que instalou: abra o terminal integrado do VS Code (`Ctrl+\`` ) e digite:
   ```
   git --version
   ```
   Deve aparecer algo como `git version 2.4x.x`

## Passo 2 â€” Configurar sua identidade (uma vez sÃ³, por computador)

No mesmo terminal:

```
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

Use o **mesmo e-mail** que vocÃª vai usar (ou jÃ¡ usa) para criar a conta no GitHub, no prÃ³ximo passo.

## Passo 3 â€” Criar conta no GitHub

1. Acesse **https://github.com**
2. Clique em **Sign up**, no canto superior direito
3. Preencha e-mail, senha e um nome de usuÃ¡rio (esse nome vai aparecer na URL do seu site depois â€” escolha algo profissional, sem espaÃ§os)
4. Resolva a verificaÃ§Ã£o (um quebra-cabeÃ§a simples) e clique em **Create account**
5. Confirme seu e-mail clicando no link que o GitHub envia para a caixa de entrada

## Passo 4 â€” Criar o repositÃ³rio no GitHub

1. JÃ¡ logado no GitHub, clique no **+** no canto superior direito â†’ **New repository**
2. DÃª um nome ao repositÃ³rio (ex.: `meu-primeiro-site`)
3. Deixe marcado **Public**
4. **NÃ£o marque** a caixa "Add a README file" (vocÃª jÃ¡ tem arquivos localmente; marcar isso cria conflito no primeiro envio)
5. Clique em **Create repository**
6. Na pÃ¡gina que abre, copie a URL mostrada em "â€¦or push an existing repository from the command line" (algo como `https://github.com/seu-usuario/meu-primeiro-site.git`)

## Passo 5 â€” Enviar seu projeto local pela primeira vez

No terminal do VS Code, com a pasta do seu projeto aberta, digite um comando de cada vez, apertando Enter depois de cada um:

```
git init
git add .
git commit -m "Primeira versÃ£o do site"
git remote add origin https://github.com/seu-usuario/meu-primeiro-site.git
git branch -M main
git push -u origin main
```

**Troque a URL do `git remote add origin` pela que vocÃª copiou no Passo 4.**

Na primeira vez, uma janela do navegador pode abrir pedindo para autorizar o VS Code/Git a acessar sua conta GitHub â€” clique em **Authorize**.

## O que cada comando faz

| Comando | O que faz |
|---|---|
| `git init` | Cria o repositÃ³rio Git local, na pasta do projeto |
| `git add .` | Prepara **todos** os arquivos modificados para o prÃ³ximo commit |
| `git commit -m "..."` | Registra um ponto de salvamento, com a mensagem entre aspas |
| `git remote add origin <url>` | Liga o repositÃ³rio local ao repositÃ³rio remoto no GitHub |
| `git branch -M main` | Garante que a branch principal se chama `main` |
| `git push -u origin main` | Envia o histÃ³rico para o GitHub |

## Como saber se deu certo

Volte Ã  pÃ¡gina do repositÃ³rio no GitHub (recarregue com F5) â€” os arquivos do seu projeto (`index.html`, pastas `css`, `js`, `img`) devem aparecer listados ali, junto com a mensagem "Primeira versÃ£o do site" do seu commit.

## Fazendo um segundo commit (o dia a dia)

Depois da primeira vez, o fluxo fica mais curto. Toda vez que vocÃª alterar algo:

```
git add .
git commit -m "Descreva o que vocÃª mudou"
git push
```

## ðŸŽ¥ VÃ­deo de apoio

- Git e GitHub, tutorial completo para iniciantes: https://www.youtube.com/watch?v=_hZf1teRFNg

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Siga os 5 passos acima, do zero, com o projeto que vocÃª construiu ao longo desta apostila.
2. Confirme no site do GitHub que os arquivos aparecem.
3. Altere algo em qualquer arquivo (por exemplo, um texto no `index.html`), salve, e faÃ§a um segundo commit com uma mensagem diferente da primeira, usando o fluxo curto acima.
4. Recarregue a pÃ¡gina do repositÃ³rio no GitHub e confirme que agora aparecem **dois** commits no histÃ³rico (clique em "commits" logo acima da lista de arquivos para ver).

