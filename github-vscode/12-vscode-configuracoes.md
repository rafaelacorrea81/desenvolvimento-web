---
title: Unidade 12 â€” VS Code: ConfiguraÃ§Ãµes e PersonalizaÃ§Ã£o
parent: GitHub e VS Code
nav_order: 12
---
# Unidade 12 â€” VS Code: ConfiguraÃ§Ãµes e PersonalizaÃ§Ã£o

**Objetivo:** Ajustar tema, fonte e comportamento do editor por meio das configuraÃ§Ãµes visuais e do arquivo `settings.json`.

## Pela tela de configuraÃ§Ãµes (mais fÃ¡cil para comeÃ§ar)

- **Tema de cores:** menu **Arquivo â†’ PreferÃªncias â†’ Tema de Cores** (ou `Ctrl+K Ctrl+T`). Um tema escuro costuma reduzir o cansaÃ§o visual em sessÃµes longas.
- **ConfiguraÃ§Ãµes gerais:** `Ctrl+,` (vÃ­rgula) abre a tela de ConfiguraÃ§Ãµes, com busca por palavra-chave (tamanho de fonte, tabulaÃ§Ã£o, quebra de linha, etc.) â€” digite o que procura na caixa de busca no topo.

## Pelo `settings.json` (configuraÃ§Ã£o em texto)

Toda opÃ§Ã£o alterada na tela de ConfiguraÃ§Ãµes tambÃ©m pode ser escrita diretamente em texto. Para abrir:

1. `Ctrl+Shift+P` (ou `Cmd+Shift+P`)
2. Digite **"Preferences: Open User Settings (JSON)"** e aperte Enter
3. Adicione (ou edite) as linhas:

```json
{
  "editor.fontSize": 15,
  "editor.formatOnSave": true,
  "editor.tabSize": 2,
  "files.autoSave": "onFocusChange",
  "workbench.colorTheme": "Default Dark+"
}
```

- `editor.fontSize` â€” tamanho da fonte no editor
- `editor.formatOnSave` â€” formata o cÃ³digo automaticamente toda vez que vocÃª salva (combine com o Prettier da Unidade 10 para eliminar a necessidade do atalho manual)
- `editor.tabSize` â€” quantos espaÃ§os cada tabulaÃ§Ã£o representa
- `files.autoSave` â€” salva sozinho quando vocÃª troca de aba ou de janela
- `workbench.colorTheme` â€” nome exato do tema escolhido (deve bater com o nome mostrado na lista de temas)

## Confirmando que funcionou

1. Salve o `settings.json` (`Ctrl+S`)
2. Abra um arquivo `.css` bagunÃ§ado (sem formataÃ§Ã£o) que vocÃª tenha o Prettier instalado
3. Salve esse arquivo (`Ctrl+S`) â€” com `editor.formatOnSave: true`, ele deve se formatar **sozinho**, sem precisar do atalho `Shift+Alt+F`

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Abra seu `settings.json` e adicione as cinco configuraÃ§Ãµes do exemplo acima, ajustando os valores ao seu gosto (por exemplo, um `fontSize` diferente).
2. Teste a `editor.formatOnSave` conforme o passo "Confirmando que funcionou" acima.
3. Troque o `workbench.colorTheme` para outro tema instalado e confirme que a cor do editor muda ao salvar.

