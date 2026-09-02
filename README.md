# FATEC Profº Jessen Vidal - São José dos Campos - 6º Semestre DSM - 2026

<p>Projeto desenvolvido para a API (Aprendizagem por Projeto Integrado) do 6° Semestre do curso Desenvolvimento de Software Multiplataforma (DSM) em parceria com a GSW.</p>

> _A API se trata de um projeto submetido à metodologia de ensino em implantação na Fatec São José dos Campos, do qual os alunos formam equipes baseadas na metodologia ágil SCRUM, tendo um aluno como Scrum Master, um sendo o Product Owner e o restante dos integrantes como Dev Team._

<img src="docs/chatinbanner.jpg">

<!-- [PREENCHER] Substituir pelo banner real do projeto (docs/chatinbanner.jpg) -->

---

### 📃 Repositórios
- [Repositório App](#) <!-- [PREENCHER] -->
- [Repositório BackEnd](#) <!-- [PREENCHER] -->
- [Repositório BD](#) <!-- [PREENCHER] -->

---

## 📑 Sumário
- [Dores do Cliente](#dores)
- [Visão do Projeto](#visao-do-projeto)
- [Cronograma do Projeto](#cronograma)
- [Tecnologias utilizadas](#tecnologias)
- [Padrões de Commit](#padrao)
- [Requisitos](#requisitos)
- [Arquitetura](#arquitetura)
- [Wireframes](#wireframes)
- [Product Backlog](#backlog)
- [Sprint Backlog](#backsprint)
- [Links úteis](#links)
- [Equipe](#equipe)

---

## 🏥 Dores do Cliente <a name="dores"></a>

### Verificar
Problemas relacionados ao acompanhamento do próprio estudo:

- Dificuldade em identificar o nível real de conhecimento em cada matéria antes de começar a estudar.
- Falta de clareza sobre o que estudar a cada momento, diante do grande volume de conteúdo do vestibular.
- Ausência de acompanhamento contínuo da própria evolução ao longo da preparação.
- Falta de feedback imediato sobre erros e acertos nas atividades realizadas.
- Perda de motivação por não perceber progresso de forma tangível.

### Planejar
Problemas relacionados à organização da rotina de estudos:

- Dificuldade em montar uma rotina de estudos adequada ao tempo restante até a prova.
- Dificuldade em priorizar matérias e tópicos com maior déficit de conhecimento.
- Custo elevado de cursinhos e mentorias particulares para um acompanhamento personalizado.
- Falta de engajamento contínuo, levando ao abandono do plano de estudos.
- Necessidade de uso consciente de IA, considerando restrições de custo e limite de uso.

### Controlar
Problemas relacionados à gestão do progresso e dos recursos do sistema:

- Falta de indicadores claros de progresso e desempenho ao longo do tempo.
- Dificuldade em verificar se o plano de estudos está de fato sendo seguido.
- Ausência de um histórico consultável de atividades e resultados anteriores.
- Necessidade de garantir que o sistema continue funcional mesmo com a IA indisponível.
- Necessidade de controlar e limitar o consumo (chamadas/tokens) de IA.

---

## 👁 Visão do Projeto <a name="visao-do-projeto"></a>

<p>O CHATin é um assistente de estudos baseado em IA: o estudante informa um tema, o sistema busca fontes confiáveis (via web search ou fontes enviadas pelo próprio estudante), gera um resumo citando essas fontes e, ao final, gera um questionário com gabarito para testar o entendimento — com correção automática. A partir desse núcleo, o assistente evolui em "personas" ao longo das sprints: um <b>Mentor</b> que recomenda o próximo tema com base no desempenho, um <b>Assistente</b> para tirar dúvidas em chat, e um <b>Avaliador</b> que dá feedback mais aprofundado sobre o progresso. O engajamento é reforçado por gamificação (XP, níveis, streak e conquistas). O núcleo (tema → fontes → resumo → questionário) é propositalmente genérico, validado no contexto de preparação para o vestibular, mas pensado para ser adaptado a outros domínios de aprendizado sem reconstrução completa da aplicação.</p>

---

## 🧩 Personas e Adaptabilidade

O requisito do parceiro é claro: a solução precisa ser validada em um contexto real (aqui, **Vestibular**), mas o núcleo do assistente deve ser adaptável a outros domínios (ex.: Redação do ENEM, Culinária, Idiomas) **sem reconstrução completa da aplicação**.

Para isso, o CHATin separa duas camadas:
- **Núcleo (domain-agnostic):** tema → busca de fontes → resumo com IA → questionário + gabarito → correção. Não depende de nenhuma regra específica de vestibular.
- **Personas (Mentor, Assistente, Avaliador):** camada configurável por domínio/trilha — implementada como agentes de IA configuráveis (sugestão: **Google ADK — Agent Development Kit**), reaproveitando o mesmo núcleo. Trocar de domínio (ex.: de Vestibular para Idiomas) significa reconfigurar a persona/trilha, não reescrever o núcleo.

> Essa separação está refletida nas Regras de Negócio das User Stories de persona (US06 — Mentor, US08 — Assistente, US11 — Avaliador) no [DoR](docs/DoR_CHATin.pdf).

---

## Cronograma de Sprints <a name="cronograma"></a>

| Sprint | Período | Status | Relatório |
|:------:|:-------:|:------:|:---------:|
| 1 | 07/09/2026 à 27/09/2026 | Não iniciado | — |
| 2 | 05/10/2026 à 25/10/2026 | Não iniciado | — |
| 3 | 02/11/2026 à 22/11/2026 | Não iniciado | — |

---

## 💻 Tecnologias utilizadas <a name="tecnologias"></a>

| Tecnologia | Finalidade |
|:----------:|------------|
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Frontend / App |
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Backend / API |
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Banco de Dados |
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Provedor de IA / PLN |
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Design de interfaces e prototipação |
| ![A definir](https://img.shields.io/badge/A%20definir-lightgrey?style=for-the-badge) | Empacotamento / Deploy |

> Assim que a stack for definida, trocar cada badge pelo padrão usado nos projetos anteriores, ex.: `![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)`.

---

### 📃 Estrutura de Branches
- **Main** — Estado principal que armazena a versão estável do projeto
- **Dev** — Estado de desenvolvimento atual

### ⬜ Status do projeto: 0/3 Sprints

---

## 💻 Padrões de Commit <a name="padrao"></a>

**FEAT**: Adiciona um novo recurso ou funcionalidade.
> Exemplo: `FEAT - Adição do diagnóstico inicial`

**FIX**: Corrige um bug.
> Exemplo: `FIX - Corrige o cálculo de XP após atividade`

**CHORE**: Atualizações de manutenção que não alteram a lógica de negócio ou visual.
> Exemplo: `CHORE - Atualização das dependências do Node.js`

**DOCS**: Altera a documentação.
> Exemplo: `DOCS - Atualiza README com informações sobre novas rotas`

**STYLE**: Modifica a formatação do código sem alterar a lógica.
> Exemplo: `STYLE - Adiciona comentários no código para facilitar a leitura`

**REFACTOR**: Refatora o código sem adicionar funcionalidades ou corrigir bugs.
> Exemplo: `REFACTOR - Refatora o serviço de jornada, deixando-o mais legível`

**TEST**: Adiciona, modifica ou remove testes.
> Exemplo: `TEST - Adiciona teste para o cálculo de nível`

**PERF**: Melhora a performance.
> Exemplo: `PERF - Otimiza a consulta de histórico de atividades`

**REVERT**: Reverte um commit anterior.
> Exemplo: `REVERT - Reverte a adição do cache de respostas da IA`

**HOTFIX**: Corrige um bug crítico em produção de forma urgente.
> Exemplo: `HOTFIX - Corrige vazamento de chave de API no cliente`

> **Nomenclatura de variáveis:** padrão `camelCase` (ex: `nomeCompleto`).

---

## 📋 Requisitos <a name="requisitos"></a>

### Requisitos Funcionais

| RF | Nome | Descritivo |
|----|------|------------|
| RF1 | Definição de Tema de Estudo | O sistema deve permitir que o estudante informe livremente um tema/assunto que deseja estudar. |
| RF2 | Busca de Fontes | O sistema deve buscar fontes sobre o tema (web search) ou aceitar fontes enviadas pelo estudante. |
| RF3 | Geração de Resumo com IA | O sistema deve gerar um resumo do tema com base nas fontes, citando-as. |
| RF4 | Geração de Questionário e Gabarito | O sistema deve gerar um questionário com gabarito a partir do resumo gerado. |
| RF5 | Correção do Questionário | O sistema deve corrigir automaticamente as respostas do estudante comparando com o gabarito. |
| RF6 | Persona Mentor | O sistema deve recomendar o próximo tema de estudo com base no desempenho do estudante. |
| RF7 | Persona Assistente (Chat) | O sistema deve permitir que o estudante converse com o assistente para tirar dúvidas sobre o tema. |
| RF8 | Persona Avaliador | O sistema deve gerar uma avaliação aprofundada sobre pontos fortes e fracos do estudante. |
| RF9 | Registro de Desempenho | O sistema deve registrar o resultado de cada questionário respondido pelo estudante. |
| RF10 | Dashboard de Progresso | O sistema deve exibir um painel com XP, nível, streak e temas estudados pelo estudante. |
| RF11 | Gamificação — XP e Níveis | O sistema deve conceder XP e níveis com base no desempenho nos questionários. |
| RF12 | Gamificação — Mecânica Extra | O sistema deve implementar ao menos uma mecânica adicional de gamificação (streak e/ou conquistas). |
| RF13 | Jornada Adaptativa | O sistema deve ajustar os próximos temas/questionários com base no desempenho recente do estudante. |

### Requisitos Não Funcionais

| RNF | Nome | Descritivo |
|-----|------|------------|
| RNF1 | Manual de Instalação | Documentação obrigatória (Fatec) explicando como instalar e rodar o projeto. |
| RNF2 | Manual do Usuário | Documentação obrigatória (Fatec) explicando como usar a aplicação. |
| RNF3 | Documentação da API | Documentação dos principais endpoints/integrações da API. |
| RNF4 | Modelagem de Dados | Modelo do banco de dados ou estrutura de persistência utilizada, documentado. |
| RNF5 | Segurança de Segredos | Chaves e segredos de APIs externas não podem ficar hardcoded no código-fonte. |
| RNF6 | Resiliência à Falha de IA | A aplicação deve continuar funcional (missões, XP, progresso, dashboard) mesmo com a IA indisponível ou cota esgotada. |
| RNF7 | Controle de Consumo de IA | O sistema deve registrar e exibir o consumo de IA (nº de chamadas e, quando disponível, tokens). |
| RNF8 | Redução de Consumo de IA | O sistema deve aplicar ao menos uma estratégia de redução de consumo (ex.: memória resumida do estudante em vez de reenviar histórico completo). |
| RNF9 | Arquitetura de Personas Configuráveis | As personas (Mentor, Assistente, Avaliador) devem ser implementadas de forma configurável por domínio/trilha (sugestão: Google ADK — Agent Development Kit), reaproveitando o núcleo de resumo e questionário sem exigir reescrevê-lo para cada novo domínio. |

---

## 🏗 Arquitetura <a name="arquitetura"></a>

<!-- [PREENCHER] Inserir diagrama de arquitetura do CHATin -->
`[PREENCHER] — imagem/diagrama de arquitetura`

---

## 🖥 Wireframes <a name="wireframes"></a>

<!-- [PREENCHER] Inserir wireframes/mockups das telas principais -->
`[PREENCHER] — telas de Login, Diagnóstico, Jornada, Chat, Dashboard, etc.`

---

## 📜 Product Backlog <a name="backlog"></a>

| RANK | SPRINT | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:------:|:----------:|:----------:|------------|:--:|:------:|
| 1 | 1 | Alta | 5 | Como estudante, quero informar um tema/assunto que desejo estudar, para que o sistema saiba sobre o que gerar conteúdo. | RF1 | ⬜ |
| 2 | 1 | Alta | 8 | Como estudante, quero que o sistema busque fontes confiáveis sobre o tema informado (ou aceite fontes que eu enviar), para que o conteúdo gerado seja embasado. | RF2 | ⬜ |
| 3 | 1 | Alta | 8 | Como estudante, quero receber um resumo gerado por IA do tema estudado, com as fontes utilizadas indicadas, para entender o conteúdo rapidamente e poder verificar a origem das informações. | RF3 | ⬜ |
| 4 | 1 | Alta | 8 | Como estudante, quero receber um questionário gerado automaticamente ao final do resumo, com gabarito, para testar meu entendimento do tema. | RF4 | ⬜ |
| 5 | 1 | Alta | 5 | Como estudante, quero responder o questionário pelo aplicativo e ver meu resultado corrigido automaticamente, para saber o que acertei e errei. | RF5 | ⬜ |
| 6 | 2 | Alta | 8 | Como estudante, quero que o assistente (persona Mentor) sugira o próximo tema de estudo com base no meu desempenho nos questionários, para saber o que estudar em seguida. | RF6 | ⬜ |
| 7 | 2 | Alta | 5 | Como estudante, quero que meu desempenho em cada questionário seja registrado, para acompanhar minha evolução ao longo do tempo. | RF9 | ⬜ |
| 8 | 2 | Alta | 8 | Como estudante, quero conversar com o assistente (persona Assistente) para tirar dúvidas sobre o tema estudado, para aprofundar meu entendimento. | RF7 | ⬜ |
| 9 | 2 | Média | 5 | Como estudante, quero ganhar XP e subir de nível a cada questionário concluído, para acompanhar minha evolução de forma gamificada. | RF11 | ⬜ |
| 10 | 2 | Alta | 5 | Como estudante, quero que meu registro de desempenho e a jornada do Mentor continuem funcionando mesmo se a IA estiver indisponível, para não travar meus estudos. | RNF6 | ⬜ |
| 11 | 3 | Alta | 8 | Como estudante, quero receber uma avaliação mais aprofundada (persona Avaliador) sobre meus pontos fortes e fracos ao final de um ciclo de estudos, para entender melhor meu progresso. | RF8 | ⬜ |
| 12 | 3 | Média | 8 | Como estudante, quero que os próximos temas/questionários se ajustem automaticamente ao meu desempenho, para receber conteúdo no nível de dificuldade certo. | RF13 | ⬜ |
| 13 | 3 | Alta | 8 | Como estudante, quero acessar um dashboard com meu progresso, XP e histórico de temas estudados, para visualizar minha evolução. | RF10 | ⬜ |
| 14 | 3 | Média | 5 | Como estudante, quero manter uma sequência de dias de estudo (streak) e desbloquear conquistas, para me sentir motivado a continuar. | RF12 | ⬜ |
| 15 | 3 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ⬜ |
| 16 | 3 | Alta | 5 | Como estudante, quero que o assistente use um resumo do meu histórico em vez de reenviar tudo para a IA a cada interação, para economizar consumo sem perder contexto relevante. | RNF8 | ⬜ |

---

## 📝 Sprint Backlog <a name="backsprint"></a>

<details>
<summary><strong>Sprint 1 — Núcleo: Resumo e Questionário com IA</strong></summary>

<br>

> **Período:** 07/09/2026 à 27/09/2026
> **Foco:** O estudante informa um tema de estudo, o sistema busca fontes (via web search ou fontes enviadas), gera um resumo citando as fontes e, ao final, gera um questionário com gabarito que o estudante responde e tem corrigido automaticamente.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 1 | Alta | 5 | Como estudante, quero informar um tema/assunto que desejo estudar, para que o sistema saiba sobre o que gerar conteúdo. | RF1 | ⬜ |
| 2 | Alta | 8 | Como estudante, quero que o sistema busque fontes confiáveis sobre o tema informado (ou aceite fontes que eu enviar), para que o conteúdo gerado seja embasado. | RF2 | ⬜ |
| 3 | Alta | 8 | Como estudante, quero receber um resumo gerado por IA do tema estudado, com as fontes utilizadas indicadas, para entender o conteúdo rapidamente e poder verificar a origem das informações. | RF3 | ⬜ |
| 4 | Alta | 8 | Como estudante, quero receber um questionário gerado automaticamente ao final do resumo, com gabarito, para testar meu entendimento do tema. | RF4 | ⬜ |
| 5 | Alta | 5 | Como estudante, quero responder o questionário pelo aplicativo e ver meu resultado corrigido automaticamente, para saber o que acertei e errei. | RF5 | ⬜ |

</details>

---

<details>
<summary><strong>Sprint 2 — Personas: Mentor e Assistente</strong></summary>

<br>

> **Período:** 05/10/2026 à 25/10/2026
> **Foco:** O sistema passa a orientar o estudante numa jornada de recomendações (persona Mentor), oferece um chat de dúvidas (persona Assistente), registra desempenho e traz gamificação básica — com resiliência caso a IA falhe.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 6 | Alta | 8 | Como estudante, quero que o assistente (persona Mentor) sugira o próximo tema de estudo com base no meu desempenho nos questionários, para saber o que estudar em seguida. | RF6 | ⬜ |
| 7 | Alta | 5 | Como estudante, quero que meu desempenho em cada questionário seja registrado, para acompanhar minha evolução ao longo do tempo. | RF9 | ⬜ |
| 8 | Alta | 8 | Como estudante, quero conversar com o assistente (persona Assistente) para tirar dúvidas sobre o tema estudado, para aprofundar meu entendimento. | RF7 | ⬜ |
| 9 | Média | 5 | Como estudante, quero ganhar XP e subir de nível a cada questionário concluído, para acompanhar minha evolução de forma gamificada. | RF11 | ⬜ |
| 10 | Alta | 5 | Como estudante, quero que meu registro de desempenho e a jornada do Mentor continuem funcionando mesmo se a IA estiver indisponível, para não travar meus estudos. | RNF6 | ⬜ |

</details>

---

<details>
<summary><strong>Sprint 3 — Persona Avaliador e Consolidação</strong></summary>

<br>

> **Período:** 02/11/2026 à 22/11/2026
> **Foco:** O sistema ganha uma persona Avaliador com feedback mais aprofundado, a jornada se ajusta ao desempenho, o estudante acompanha tudo num dashboard, com gamificação extra e governança de consumo de IA.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 11 | Alta | 8 | Como estudante, quero receber uma avaliação mais aprofundada (persona Avaliador) sobre meus pontos fortes e fracos ao final de um ciclo de estudos, para entender melhor meu progresso. | RF8 | ⬜ |
| 12 | Média | 8 | Como estudante, quero que os próximos temas/questionários se ajustem automaticamente ao meu desempenho, para receber conteúdo no nível de dificuldade certo. | RF13 | ⬜ |
| 13 | Alta | 8 | Como estudante, quero acessar um dashboard com meu progresso, XP e histórico de temas estudados, para visualizar minha evolução. | RF10 | ⬜ |
| 14 | Média | 5 | Como estudante, quero manter uma sequência de dias de estudo (streak) e desbloquear conquistas, para me sentir motivado a continuar. | RF12 | ⬜ |
| 15 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ⬜ |
| 16 | Alta | 5 | Como estudante, quero que o assistente use um resumo do meu histórico em vez de reenviar tudo para a IA a cada interação, para economizar consumo sem perder contexto relevante. | RNF8 | ⬜ |

</details>

---

## Links Úteis <a name="links"></a>

- [Definition of Ready (DoR)](docs/DoR_CHATin.pdf)
- `[PREENCHER]` — demais links (arquitetura, wireframes, etc.)

---

## 👥 Equipe <a name="equipe"></a>

| Foto | Função | Nome | LinkedIn | GitHub |
|:----:|:------:|:----:|:--------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/160733714?v=4" width="75px"> | Dev Team | Eduardo da Silva Fontes | [LinkedIn](https://www.linkedin.com/in/eduardo-da-silva-fontes/) | [GitHub](https://github.com/DuuhZero) |
| <img src="https://avatars.githubusercontent.com/u/162118889?v=4" width="75px"> | Dev Team | Eduardo Kuwahara Jr. | [LinkedIn](https://www.linkedin.com/in/eduardo-kuwahara-3b2267303/) | [GitHub](https://github.com/EduardoKuwahara) |
| <img src="https://avatars.githubusercontent.com/u/161594793?v=4" width="75px"> | Dev Team | Eric Kawata | [LinkedIn](https://www.linkedin.com/in/eric-kawata-99678b302/) | [GitHub](https://github.com/ericFatec) |
| <img src="https://avatars.githubusercontent.com/u/144804717?v=4" width="75px"> | Dev Team | Fábio Hiroshi | [LinkedIn](https://www.linkedin.com/in/f%C3%A1bio-hiroshi-5393a51a0) | [GitHub](https://github.com/FabioHiros) |
| <img src="https://avatars.githubusercontent.com/u/162117916?v=4" width="75px"> | Product Owner | João Vitor Rossi Ferreira | [LinkedIn](https://www.linkedin.com/in/joão-rossi-7311a0301/) | [GitHub](https://github.com/joaorossiferreira) |
| <img src="https://avatars.githubusercontent.com/u/95691713?v=4" width="75px"> | Dev Team | Kathellyn Caroline Alves dos Santos | [LinkedIn](https://www.linkedin.com/in/kathellyn-caroline-a562101b9) | [GitHub](https://github.com/CarolineKathellyn) |
| <img src="https://avatars.githubusercontent.com/u/161987258?v=4" width="75px"> | Dev Team | Victor Daniel | [LinkedIn](https://www.linkedin.com/in/victor-daniel-ramos-bessa-1436a3215/) | [GitHub](https://github.com/victordanielrb) |
| <img src="https://avatars.githubusercontent.com/u/162117908?v=4" width="75px"> | Scrum Master | Paulo Henrique Martins de Almeida | [LinkedIn](https://www.linkedin.com/in/paulo-almeida-3102452a7/) | [GitHub](https://github.com/pauloalmeida46) |
