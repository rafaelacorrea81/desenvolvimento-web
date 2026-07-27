---
title: Unidade 2 â€” Configurando seu Ambiente
parent: Primeiros Passos na Web
nav_order: 2
---
# Unidade 2 â€” Configurando seu Ambiente

**Objetivo:** Instalar o VS Code, instalar a extensÃ£o Live Server e criar a estrutura mÃ­nima de pastas para iniciar um projeto web, sem travar em nenhum passo.

> Esta unidade cobre sÃ³ o essencial para acompanhar o curso. Para instalaÃ§Ã£o detalhada de Git, extensÃµes avanÃ§adas, atalhos e configuraÃ§Ãµes do VS Code, use o livro complementar **"GitHub e VS Code: Conceitos e ConfiguraÃ§Ãµes BÃ¡sicas"** â€” ele foi escrito depois desta apostila e aprofunda cada um desses pontos passo a passo.

## Passo 1 â€” Baixar e instalar o VS Code

1. Abra o navegador e acesse **https://code.visualstudio.com**
2. O site detecta seu sistema operacional automaticamente e mostra um botÃ£o azul grande escrito **Download for Windows** (ou Mac/Linux). Clique nele.
3. **No Windows:** abra o arquivo baixado (algo como `VSCodeUserSetup-x64-x.xx.x.exe`). Na tela de instalaÃ§Ã£o:
   - Aceite os termos de licenÃ§a e clique em **AvanÃ§ar**
   - Na tela "Tarefas Adicionais", marque as caixas **"Adicionar aÃ§Ã£o 'Abrir com Code' ao menu de contexto dos arquivos"** e **"Adicionar ao PATH"** (essa Ãºltima geralmente jÃ¡ vem marcada)
   - Clique em **AvanÃ§ar** e depois em **Instalar**
   - Ao final, deixe marcada a opÃ§Ã£o **"Executar o Visual Studio Code"** e clique em **Concluir**
4. **No macOS:** o download vem em um arquivo `.zip`. Extraia-o (duplo clique) e arraste o Ã­cone do **Visual Studio Code** para a pasta **Aplicativos**. Abra pelo Launchpad ou pela pasta Aplicativos.
5. **No Linux (Debian/Ubuntu):** baixe o pacote `.deb` pelo site e instale com:
   ```
   sudo apt install ./code_*.deb
   ```

**Como saber se deu certo:** o VS Code abre e mostra uma tela de boas-vindas ("Get Started") com o texto "Visual Studio Code" no topo. Se isso aconteceu, a instalaÃ§Ã£o funcionou.

## Passo 2 â€” Criar a pasta do seu projeto

Antes de abrir o VS Code, crie no seu computador (fora de qualquer pasta de sistema, por exemplo dentro de "Documentos" ou "Ãrea de Trabalho") uma pasta chamada `meu-projeto`.

Dentro dela, crie esta estrutura de subpastas e arquivos vazios:

```
meu-projeto/
â”œâ”€â”€ index.html
â”œâ”€â”€ css/
â”‚   â””â”€â”€ style.css
â”œâ”€â”€ js/
â”‚   â””â”€â”€ script.js
â””â”€â”€ img/
    â””â”€â”€ logo.png
```

VocÃª pode criar essas pastas e arquivos vazios pelo prÃ³prio gerenciador de arquivos do sistema operacional (Explorador de Arquivos no Windows, Finder no Mac) antes de abrir o editor â€” Ã© mais fÃ¡cil visualizar assim na primeira vez.

## Passo 3 â€” Abrir a pasta no VS Code (nÃ£o um arquivo solto!)

1. Abra o VS Code
2. No menu superior, clique em **Arquivo â†’ Abrir Pasta...** (em inglÃªs: **File â†’ Open Folder...**)
3. Navegue atÃ© a pasta `meu-projeto` que vocÃª criou e clique em **Selecionar Pasta**

**Ponto de atenÃ§Ã£o:** se vocÃª abrir sÃ³ o arquivo `index.html` (Arquivo â†’ Abrir Arquivo), o VS Code nÃ£o vai mostrar a Ã¡rvore de pastas do projeto nem vai funcionar corretamente com o Live Server. Sempre abra a **pasta inteira**.

**Como saber se deu certo:** no painel Explorer, Ã  esquerda, vocÃª vÃª o nome `MEU-PROJETO` no topo e, abaixo, a Ã¡rvore com `css`, `js`, `img` e `index.html`.

## Passo 4 â€” Instalar as extensÃµes essenciais

1. Na barra lateral esquerda do VS Code, clique no Ã­cone de quadrados (ExtensÃµes) â€” ou use o atalho `Ctrl+Shift+X` (Windows/Linux) ou `Cmd+Shift+X` (Mac)
2. Na caixa de busca que aparece, digite o nome de cada extensÃ£o abaixo, uma de cada vez, e clique em **Install** no resultado correspondente:

| ExtensÃ£o | Autor (confira antes de instalar) | Para que serve |
|---|---|---|
| **Live Server** | Ritwick Dey | Cria um servidor local que atualiza o navegador sozinho a cada Ctrl+S |
| **Prettier - Code formatter** | Prettier | Formata (organiza) o cÃ³digo automaticamente |
| **HTML CSS Support** | ecmel | Sugere nomes de classes CSS enquanto vocÃª digita no HTML |

**Como saber se deu certo:** as trÃªs aparecem na lista de "Instaladas" quando vocÃª clica no Ã­cone de ExtensÃµes novamente.

## Passo 5 â€” Testar o Live Server

1. No painel Explorer, clique no arquivo `index.html` para abri-lo
2. Digite dentro dele uma estrutura HTML simples (veremos a estrutura completa na Unidade 3); por enquanto, sÃ³ para testar, digite:
   ```
   <h1>Funcionou!</h1>
   ```
3. Salve com `Ctrl+S` (Windows/Linux) ou `Cmd+S` (Mac)
4. Clique com o **botÃ£o direito** em qualquer lugar dentro do arquivo `index.html` aberto e escolha **"Open with Live Server"**
5. Seu navegador padrÃ£o abre sozinho, numa URL parecida com `http://127.0.0.1:5500/index.html`, mostrando o texto "Funcionou!"

**Como saber se deu certo:** a partir de agora, toda vez que vocÃª salvar (`Ctrl+S`) qualquer arquivo do projeto com o Live Server ativo, essa aba do navegador atualiza sozinha, sem precisar apertar F5.

Se o navegador **nÃ£o abrir sozinho**: verifique, no canto inferior direito do VS Code, se aparece o texto **"Go Live"** (Live Server desligado) ou um nÃºmero de porta como **"Port: 5500"** (Live Server ligado). Clique nesse texto para ligar/desligar manualmente.

## Ferramentas de IA no editor

Ambientes com agentes de IA embutidos (como o **Google Antigravity**, que Ã© construÃ­do sobre a mesma base do VS Code) jÃ¡ existem no mercado e geram cÃ³digo sozinhos a partir de instruÃ§Ãµes em portuguÃªs. Mas eles exigem que vocÃª jÃ¡ entenda o que estÃ¡ sendo gerado, para revisar e corrigir quando necessÃ¡rio. Por isso, o caminho recomendado aqui Ã©: consolide primeiro o VS Code "tradicional" â€” Ã© a base que te dÃ¡ senso crÃ­tico para usar esse tipo de ferramenta depois, em vez de depender cegamente dela.

## ðŸŽ¥ VÃ­deo de apoio

- InstalaÃ§Ã£o e primeiros passos no VS Code: https://www.youtube.com/watch?v=aQXVGHLXJew

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Instale o VS Code seguindo o Passo 1.
2. Crie a estrutura de pastas do Passo 2 e abra-a corretamente no VS Code (Passo 3).
3. Instale as trÃªs extensÃµes do Passo 4.
4. Teste o Live Server (Passo 5) e confirme que o navegador abre sozinho mostrando "Funcionou!".

**NÃ£o avance para a Unidade 3 atÃ© o navegador abrir sozinho com o Live Server.** Se travar em qualquer passo, releia o "Como saber se deu certo" daquele passo antes de continuar.

