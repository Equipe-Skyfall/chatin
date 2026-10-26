# AGENTS.md

Convenções e contexto deste projeto para qualquer agente de codificação (Claude Code, Cursor, Copilot, Codex etc.) vivem em:

- [`docs/AGENTS.md`](docs/AGENTS.md) — convenções comuns aos dois repositórios: padrão de commits/PR, review e testes.

O que é específico de cada lado vive dentro do próprio submodule:

- `chatin-back/docs/AGENTS.md` — stack do backend, ambiente/segurança, testes (pytest).
- `chatin-front/docs/AGENTS.md` — stack do frontend, estrutura de componentes, testes (Vitest).
- `chatin-front/docs/DESIGN.md` — identidade visual (cores, tipografia, componentes).

Cada submodule tem seu próprio `AGENTS.md`/`CLAUDE.md` apontando de volta para `docs/AGENTS.md` deste repositório, para que as convenções comuns tenham uma única fonte de verdade.
