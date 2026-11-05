---
name: destrava-pr-workflow
description: Regras obrigatórias para qualquer alteração no repositório do site Destrava Surf. Usar sempre que for editar código, conteúdo, configuração ou assets do site.
---

# Destrava Surf — Workflow obrigatório com Pull Requests

## Regra principal

Toda alteração no repositório `iza-alcanfor/destravasurf` deve ser feita em uma branch própria e entregue por Pull Request para revisão. Nunca faça alterações diretamente na branch `main`.

## Processo obrigatório

1. **Inspecionar antes de alterar**
   - Leia os arquivos relevantes e entenda a estrutura existente.
   - Preserve o design, os padrões e as funcionalidades atuais, salvo pedido explícito em contrário.
   - Confirme os preços e informações comerciais no código ou com a pessoa responsável; não invente valores.

2. **Criar uma branch**
   - Crie uma branch descritiva a partir da versão atual de `main`.
   - Use nomes curtos, por exemplo: `feat/seo-homepage`, `feat/gallery-updates`, `fix/mobile-layout` ou `docs/content-levels`.

3. **Implementar na branch**
   - Faça todos os commits exclusivamente na branch de trabalho.
   - Mantenha o escopo do PR pequeno e coeso.
   - Não misture refatorações não solicitadas com mudanças de conteúdo ou design.
   - Ao adicionar imagens, mantenha os arquivos no repositório e use caminhos relativos compatíveis com a hospedagem do site.

4. **Validar**
   - Revise o diff e os arquivos alterados.
   - Verifique links, caminhos de imagens, responsividade e consistência entre português e inglês quando aplicável.
   - Procure erros óbvios de HTML, CSS e JavaScript.
   - Informe claramente qualquer validação que não tenha sido possível executar.

5. **Abrir um Pull Request**
   - Abra um PR da branch de trabalho para `main`.
   - Descreva objetivo, principais mudanças, arquivos afetados e validações realizadas.
   - Liste riscos ou pontos que precisam de conferência manual.
   - Inclua capturas de tela quando forem úteis para mudanças visuais.

6. **Aguardar aprovação**
   - Compartilhe o link do PR e um resumo com a responsável pelo projeto.
   - **Não faça merge, não publique e não atualize a `main` sem autorização explícita da usuária.**
   - Se houver pedidos de ajuste, atualize a mesma branch e o mesmo PR.

## Reversibilidade e segurança

- Nunca force push nem reescreva histórico sem autorização explícita.
- Nunca apague arquivos ou dados sem explicar o impacto e obter autorização.
- Prefira commits pequenos, claros e fáceis de reverter.
- Não faça deploy manual como atalho para contornar o PR.
- A publicação só deve acontecer pelo fluxo aprovado após o merge autorizado.

## Comunicação

Ao concluir cada tarefa, informe:
- branch criada;
- link e número do PR;
- resumo das alterações;
- validações realizadas e limitações;
- confirmação explícita de que o PR está aguardando revisão e não foi mesclado.

## Regra de decisão

Se não for possível criar branch ou PR, pare antes de modificar a `main`. Explique o bloqueio e peça orientação. Não substitua o fluxo por commits diretos.
