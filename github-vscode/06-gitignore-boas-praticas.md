---
title: Unidade 6 â€” .gitignore e Boas PrÃ¡ticas de Commit
parent: GitHub e VS Code
nav_order: 6
---
# Unidade 6 â€” .gitignore e Boas PrÃ¡ticas de Commit

**Objetivo:** Configurar um arquivo `.gitignore` e escrever mensagens de commit claras e Ãºteis.

## Por que ignorar arquivos

Nem tudo que existe na pasta do projeto deveria ir para o repositÃ³rio: pastas geradas automaticamente (como `node_modules`, em projetos com Node.js), arquivos de configuraÃ§Ã£o pessoal do editor, ou arquivos temporÃ¡rios. O arquivo `.gitignore` lista o que o Git deve **ignorar** e nunca enviar ao repositÃ³rio.

## Criando o arquivo

Na raiz do seu projeto (mesmo nÃ­vel do `index.html`), crie um arquivo chamado exatamente `.gitignore` (com o ponto no inÃ­cio, sem extensÃ£o) e adicione:

```
node_modules/
.DS_Store
*.log
.vscode/
.env
```

- `node_modules/` â€” pasta pesada, gerada automaticamente por gerenciadores de pacotes (nÃ£o usada nesta apostila, mas comum em projetos maiores)
- `.DS_Store` â€” arquivo criado automaticamente pelo macOS em cada pasta
- `*.log` â€” qualquer arquivo terminado em `.log`
- `.vscode/` â€” configuraÃ§Ãµes especÃ­ficas do seu VS Code local
- `.env` â€” arquivo onde normalmente ficam senhas e chaves de configuraÃ§Ã£o

> âš ï¸ **Nunca versione arquivos com senhas, chaves de API ou dados sensÃ­veis** (geralmente guardados em `.env`). Uma vez enviados ao GitHub, esses dados ficam no histÃ³rico mesmo que o arquivo seja apagado depois â€” Ã© preciso reescrever o histÃ³rico do zero para removÃª-los de verdade.

## Confirmando que o `.gitignore` estÃ¡ funcionando

1. Crie uma pasta vazia chamada `node_modules` dentro do seu projeto, sÃ³ para o teste
2. Rode `git status`
3. **Como saber se deu certo:** essa pasta **nÃ£o** deve aparecer na lista de arquivos nÃ£o rastreados â€” o Git jÃ¡ a ignora, por causa da regra no `.gitignore`

## Boas prÃ¡ticas de mensagem de commit

- Escreva no **imperativo**: "Corrige alinhamento do menu", nÃ£o "Corrigido" ou "CorreÃ§Ãµes"
- **Uma mudanÃ§a lÃ³gica por commit** â€” evite misturar "ajusta CSS" com "adiciona nova pÃ¡gina" no mesmo commit
- Mensagens curtas na primeira linha (atÃ© ~50 caracteres); detalhes extras podem ir em uma segunda linha, separada por uma linha em branco

## ðŸ“ ExercÃ­cio de fixaÃ§Ã£o

1. Crie um `.gitignore` no seu projeto com as cinco linhas do exemplo acima.
2. Crie uma pasta `node_modules` vazia (sÃ³ para teste) e confirme, com `git status`, que ela nÃ£o aparece como pendente para commit.
3. Reescreva estas trÃªs mensagens de commit ruins, seguindo as boas prÃ¡ticas acima: "coisas", "correÃ§Ã£o", "att".

