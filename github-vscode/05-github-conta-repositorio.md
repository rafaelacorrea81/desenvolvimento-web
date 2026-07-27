---
title: Unidade 5 â€” GitHub: Criando Conta e RepositÃ³rio Remoto
parent: GitHub e VS Code
nav_order: 5
---
# Unidade 5 â€” GitHub: Criando Conta e RepositÃ³rio Remoto

**Objetivo:** Criar uma conta no GitHub, criar um repositÃ³rio remoto e conectÃ¡-lo a um repositÃ³rio local, do zero.

## Passo 1 â€” Criar a conta

1. Acesse **https://github.com**
2. Clique em **Sign up**, no canto superior direito
3. Preencha e-mail, crie uma senha e escolha um nome de usuÃ¡rio (esse nome aparece na URL dos seus projetos publicados â€” evite espaÃ§os e caracteres especiais)
4. Resolva a verificaÃ§Ã£o de seguranÃ§a (um quebra-cabeÃ§a visual simples) e clique em **Create account**
5. O GitHub envia um cÃ³digo de verificaÃ§Ã£o para seu e-mail â€” digite-o na tela seguinte para confirmar a conta

## Passo 2 â€” Criar um repositÃ³rio novo

1. JÃ¡ logado, clique no Ã­cone **+** no canto superior direito â†’ **New repository**
2. Em **Repository name**, digite um nome (ex.: `meu-primeiro-site`)
3. Deixe **Public** selecionado (necessÃ¡rio para usar o GitHub Pages gratuito depois)
4. **NÃ£o marque** a caixa **"Add a README file"** se vocÃª jÃ¡ tem um projeto local pronto â€” isso evita um conflito de histÃ³rico no primeiro envio
5. Clique em **Create repository**
6. Na pÃ¡gina seguinte, copie a URL mostrada (formato `https://github.com/seu-usuario/meu-primeiro-site.git`)

## Passo 3 â€” Conectando o repositÃ³rio local ao remoto

No terminal, dentro da pasta do seu projeto (que jÃ¡ deve ter passado por `git init`, `git add`, `git commit` â€” Unidade 3):

```
git remote add origin https://github.com/seu-usuario/meu-primeiro-site.git
git branch -M main
git push -u origin main
```

Troque a URL pela que vocÃª copiou no Passo 2.

**Como saber se deu certo:** recarregue a pÃ¡gina do repositÃ³rio no GitHub (F5) â€” os arquivos do projeto devem aparecer listados.

## Trazendo mudanÃ§as do remoto (em outro computador, por exemplo)

```
git clone https://github.com/seu-usuario/meu-primeiro-site.git   # copia um repositÃ³rio existente para uma pasta nova
git pull                                                          # baixa e mescla mudanÃ§as novas do remoto
```

## O que significa "origin" e o "-u"

`origin` Ã© apenas um apelido (vocÃª poderia escolher outro nome) para a URL do repositÃ³rio remoto. O `-u` em `git push -u origin main`, usado sÃ³ na primeira vez, cria a ligaÃ§Ã£o entre a branch local `main` e a branch remota `main` â€” depois disso, basta digitar `git push` sozinho, sem repetir `origin main`.

## Se pedir autenticaÃ§Ã£o

Na primeira vez que vocÃª fizer `git push`, pode abrir uma janela do navegador pedindo para autorizar o acesso Ã  sua conta GitHub â€” clique em **Authorize**. Se em vez disso aparecer um campo de senha direto no terminal, veja a nota sobre autenticaÃ§Ã£o na Unidade 13 (VS Code + Git Integrados).

## ðŸŽ¥ VÃ­deo de apoio

- GitHub, guia completo para iniciantes: https://www.youtube.com/watch?v=BUGZZaChiYw

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Crie sua conta no GitHub (se ainda nÃ£o tiver) seguindo o Passo 1.
2. Crie um repositÃ³rio novo (Passo 2) para um projeto seu.
3. Conecte-o ao repositÃ³rio local (Passo 3) e confirme, no site, que os arquivos e o histÃ³rico de commits aparecem corretamente.

