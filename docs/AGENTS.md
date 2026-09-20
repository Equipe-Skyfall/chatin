# AGENTS.md — CHATin

Este arquivo é o "README para agentes": contexto e convenções **comuns aos dois repositórios** (`chatin-back`, `chatin-front`) que qualquer agente de codificação (Claude Code, Cursor, Copilot, Codex etc.) deve seguir. Complementa o `README.md` (que é para humanos).

Stack, bibliotecas, segurança/ambiente e identidade visual são específicos de cada lado e vivem em `chatin-front/docs/` e `chatin-back/docs/` — leia o `AGENTS.md` de dentro do repo em que você está trabalhando, além deste.

## Visão geral do projeto

CHATin é um coach de estudos baseado em IA: o estudante conversa livremente com um assistente, que reconhece a matéria/tópico discutido, gera resumos, cria questionários e acompanha o progresso ao longo do tempo. Ver `README.md` para o backlog completo e `docs/DoR_CHATin.pdf` para critérios de aceitação.

## Padrão de commits

Formato: `TIPO - descrição curta no imperativo`.

| Tipo | Uso |
|---|---|
| `FEAT` | Novo recurso ou funcionalidade |
| `FIX` | Correção de bug |
| `CHORE` | Manutenção que não afeta lógica/visual (deps, configs) |
| `DOCS` | Alteração de documentação |
| `STYLE` | Formatação, sem mudar lógica |
| `REFACTOR` | Refatoração sem adicionar feature nem corrigir bug |
| `TEST` | Adiciona/ajusta testes |
| `PERF` | Melhoria de performance |
| `REVERT` | Reverte um commit anterior |
| `HOTFIX` | Correção urgente de bug crítico |

Exemplo: `FEAT - Adiciona geração de resumo a partir da conversa`

Branches: `main` (estável) e `dev` (desenvolvimento). Nunca commitar direto na `main`.

## Padrão de Pull Request

- **Título:** `[TIPO] Descrição curta` (mesmo vocabulário da tabela de commits acima, ex.: `[FEAT] Correção automática de questionário`).
- **Descrição obrigatória com 3 seções:**
  - `O que mudou` — resumo objetivo.
  - `Como testar` — passos manuais ou comando de teste automatizado.
  - `Screenshots` — obrigatório para qualquer mudança visual (comparar com `chatin-front/docs/DESIGN.md`).
- PR pequeno e focado em uma única User Story ou Task sempre que possível.
- Nenhum PR é aprovado pelo próprio autor — sempre precisa de revisão de outra pessoa antes do merge (ver `Guia do GitHub` da API).

## Padrão de comentários em review de PR

Usar o padrão [Conventional Comments](https://conventionalcomments.org/) para deixar claro o peso de cada comentário:

- `nit:` — sugestão de estilo, não bloqueia o merge.
- `issue:` — problema que precisa ser corrigido antes do merge.
- `question:` — dúvida genuína, precisa de resposta antes de aprovar.
- `suggestion:` — proposta de mudança, com justificativa.
- `praise:` — reforço positivo (usar também, não só apontar problema).

Exemplo: `suggestion: extrair essa lógica de cálculo de XP para uma função separada, facilita testar isoladamente.`

## Padrão de testes (princípios gerais)

> A estratégia de testes ainda não foi formalizada pela equipe (item em aberto no checklist do DoR). Até que isso seja decidido, siga esta convenção mínima — as ferramentas usadas em cada lado (pytest, Vitest...) estão documentadas no `AGENTS.md` de cada repo:

- Regras determinísticas (cálculo de XP, streak, correção automática de questionário, avanço/reforço de módulo) **devem ter teste unitário** — são lógica pura da aplicação, não dependem da IA, e são baratas de testar.
- Chamadas à IA (geração de resumo, geração de questionário, chat) não precisam de teste de conteúdo gerado, mas devem ter teste do comportamento de fallback (o que acontece quando a IA falha/está indisponível).
- Todo teste deve poder rodar localmente sem depender de uma chave de API real (usar mocks para chamadas ao Gemini).
