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

<p>O CHATin é um assistente virtual gamificado que atua como coach de estudos para candidatos ao vestibular, utilizando processamento de linguagem natural e inteligência artificial de forma pontual para orientar a jornada de aprendizado do estudante. A partir de um diagnóstico inicial e do objetivo informado (curso e data da prova), o sistema monta uma trilha de estudos personalizada, propõe atividades e missões, acompanha o desempenho e oferece feedback individualizado. O engajamento é mantido por meio de mecânicas de gamificação (XP, níveis, streak e conquistas). O núcleo do assistente foi projetado para ser adaptável a outros contextos de aprendizado além do vestibular, sem a necessidade de reconstrução completa da aplicação.</p>

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
| [PREENCHER] | Frontend / App |
| [PREENCHER] | Backend / API |
| [PREENCHER] | Banco de Dados |
| [PREENCHER] | Provedor de IA / PLN |
| [PREENCHER] | Design de interfaces e prototipação |
| [PREENCHER] | Empacotamento / Deploy |

---

### 📃 Estrutura de Branches
- **Main** — Estado principal que armazena a versão estável do projeto
- **Dev** — Estado de desenvolvimento atual

### ⏳ Status do projeto: 0/3 Sprints

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
| RF1 | Cadastro e Login | O sistema deve permitir que o estudante crie uma conta e faça login para acessar sua jornada. |
| RF2 | Definição de Objetivo | O sistema deve permitir informar o vestibular/curso alvo e a data da prova. |
| RF3 | Diagnóstico Inicial | O sistema deve aplicar um teste diagnóstico para identificar o nível atual do estudante por matéria. |
| RF4 | Jornada Personalizada | O sistema deve gerar uma trilha de estudos personalizada com base no diagnóstico e no objetivo informado. |
| RF5 | Atividades/Missões | O sistema deve propor atividades ou missões diárias/periódicas ao estudante. |
| RF6 | Registro de Desempenho | O sistema deve registrar as respostas e o desempenho do estudante em cada atividade. |
| RF7 | Feedback Personalizado | O sistema deve gerar, via IA, um feedback personalizado sobre o desempenho do estudante. |
| RF8 | Gamificação — XP e Níveis | O sistema deve conceder XP e níveis com base no progresso do estudante. |
| RF9 | Gamificação — Mecânica Extra | O sistema deve implementar ao menos uma mecânica adicional de gamificação (streak de dias e/ou conquistas). |
| RF10 | Dashboard de Progresso | O sistema deve exibir um painel com a evolução do estudante ao longo do tempo. |
| RF11 | Chat com o Assistente | O sistema deve permitir que o estudante converse com o assistente virtual para tirar dúvidas e receber orientação. |
| RF12 | Histórico de Atividades | O sistema deve manter um histórico consultável das atividades e resultados anteriores. |
| RF13 | Jornada Adaptativa | O sistema deve ajustar a dificuldade/sequência das atividades com base no desempenho recente do estudante. |
| RF14 | Gestão de Conteúdo | O sistema deve permitir o cadastro/manutenção de matérias, tópicos e questões usados na jornada. |

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
| 1 | 1 | Baixa | 3 | Como estudante, quero criar uma conta e fazer login, para acessar minha jornada de estudos de forma segura. | RF1 | ❌ |
| 2 | 1 | Alta | 5 | Como estudante, quero informar meu curso/vestibular alvo e a data da prova, para que o assistente monte uma jornada adequada ao meu prazo. | RF2 | ❌ |
| 3 | 1 | Alta | 5 | Como administrador, quero cadastrar matérias, tópicos e questões, para alimentar a base de conteúdo usada na jornada dos estudantes. | RF14 | ❌ |
| 4 | 1 | Alta | 8 | Como estudante, quero responder um teste diagnóstico inicial, para que o sistema identifique meu nível atual em cada matéria. | RF3 | ❌ |
| 5 | 1 | Alta | 8 | Como estudante, quero receber uma jornada de estudos personalizada com base no meu diagnóstico e objetivo, para saber por onde começar. | RF4 | ❌ |
| 6 | 1 | Média | 5 | Como estudante, quero visualizar meu nível e XP desde o início, para acompanhar minha evolução ao longo do tempo. | RF8 | ❌ |
| 7 | 2 | Alta | 8 | Como estudante, quero receber atividades/missões sugeridas pelo assistente, para manter uma rotina de estudos consistente. | RF5 | ❌ |
| 8 | 2 | Alta | 5 | Como estudante, quero que minhas respostas e desempenho em cada atividade sejam registrados, para que meu progresso não se perca. | RF6 | ❌ |
| 9 | 2 | Alta | 8 | Como estudante, quero receber feedback personalizado sobre meu desempenho, para entender meus pontos fortes e o que preciso melhorar. | RF7 | ❌ |
| 10 | 2 | Alta | 8 | Como estudante, quero conversar com o assistente virtual para tirar dúvidas sobre a jornada, para não ficar perdido no processo de estudo. | RF11 | ❌ |
| 11 | 2 | Média | 5 | Como estudante, quero manter uma sequência de dias de estudo (streak) e desbloquear conquistas, para me sentir motivado a continuar. | RF9 | ❌ |
| 12 | 2 | Alta | 5 | Como estudante, quero que missões, XP e progresso continuem funcionando mesmo se a IA estiver indisponível, para não travar meus estudos. | RNF6 | ❌ |
| 13 | 3 | Alta | 8 | Como estudante, quero acessar um dashboard com meu progresso e evolução, para visualizar meu avanço rumo ao objetivo. | RF10 | ❌ |
| 14 | 3 | Média | 5 | Como estudante, quero consultar o histórico de atividades e resultados anteriores, para revisar meu desempenho passado. | RF12 | ❌ |
| 15 | 3 | Média | 8 | Como estudante, quero que minha jornada se ajuste automaticamente conforme meu desempenho, para receber atividades no nível de dificuldade certo. | RF13 | ❌ |
| 16 | 3 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ❌ |
| 17 | 3 | Alta | 5 | Como estudante, quero que o assistente use um resumo da minha jornada em vez do histórico completo, para que o sistema economize consumo de IA sem perder contexto relevante. | RNF8 | ❌ |

---

## 📝 Sprint Backlog <a name="backsprint"></a>

<details>
<summary><strong>Sprint 1 — Onboarding, Diagnóstico e Jornada Inicial</strong></summary>

<br>

> **Período:** 07/09/2026 à 27/09/2026
> **Foco:** O estudante consegue se cadastrar, definir seu objetivo, fazer o diagnóstico inicial e receber uma jornada de estudos personalizada.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 1 | Baixa | 3 | Como estudante, quero criar uma conta e fazer login, para acessar minha jornada de estudos de forma segura. | RF1 | ❌ |
| 2 | Alta | 5 | Como estudante, quero informar meu curso/vestibular alvo e a data da prova, para que o assistente monte uma jornada adequada ao meu prazo. | RF2 | ❌ |
| 3 | Alta | 5 | Como administrador, quero cadastrar matérias, tópicos e questões, para alimentar a base de conteúdo usada na jornada dos estudantes. | RF14 | ❌ |
| 4 | Alta | 8 | Como estudante, quero responder um teste diagnóstico inicial, para que o sistema identifique meu nível atual em cada matéria. | RF3 | ❌ |
| 5 | Alta | 8 | Como estudante, quero receber uma jornada de estudos personalizada com base no meu diagnóstico e objetivo, para saber por onde começar. | RF4 | ❌ |
| 6 | Média | 5 | Como estudante, quero visualizar meu nível e XP desde o início, para acompanhar minha evolução ao longo do tempo. | RF8 | ❌ |

</details>

---

<details>
<summary><strong>Sprint 2 — Engajamento, Feedback e Resiliência de IA</strong></summary>

<br>

> **Período:** 05/10/2026 à 25/10/2026
> **Foco:** O estudante cumpre missões, tem seu desempenho registrado, recebe feedback via IA, tira dúvidas no chat e se mantém engajado por gamificação — com o sistema resiliente caso a IA falhe.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 7 | Alta | 8 | Como estudante, quero receber atividades/missões sugeridas pelo assistente, para manter uma rotina de estudos consistente. | RF5 | ❌ |
| 8 | Alta | 5 | Como estudante, quero que minhas respostas e desempenho em cada atividade sejam registrados, para que meu progresso não se perca. | RF6 | ❌ |
| 9 | Alta | 8 | Como estudante, quero receber feedback personalizado sobre meu desempenho, para entender meus pontos fortes e o que preciso melhorar. | RF7 | ❌ |
| 10 | Alta | 8 | Como estudante, quero conversar com o assistente virtual para tirar dúvidas sobre a jornada, para não ficar perdido no processo de estudo. | RF11 | ❌ |
| 11 | Média | 5 | Como estudante, quero manter uma sequência de dias de estudo (streak) e desbloquear conquistas, para me sentir motivado a continuar. | RF9 | ❌ |
| 12 | Alta | 5 | Como estudante, quero que missões, XP e progresso continuem funcionando mesmo se a IA estiver indisponível, para não travar meus estudos. | RNF6 | ❌ |

</details>

---

<details>
<summary><strong>Sprint 3 — Consolidação, Adaptação e Governança de IA</strong></summary>

<br>

> **Período:** 02/11/2026 à 22/11/2026
> **Foco:** O estudante visualiza sua evolução completa e histórico, a jornada se adapta ao desempenho, e a equipe garante controle/redução de consumo de IA.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 13 | Alta | 8 | Como estudante, quero acessar um dashboard com meu progresso e evolução, para visualizar meu avanço rumo ao objetivo. | RF10 | ❌ |
| 14 | Média | 5 | Como estudante, quero consultar o histórico de atividades e resultados anteriores, para revisar meu desempenho passado. | RF12 | ❌ |
| 15 | Média | 8 | Como estudante, quero que minha jornada se ajuste automaticamente conforme meu desempenho, para receber atividades no nível de dificuldade certo. | RF13 | ❌ |
| 16 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ❌ |
| 17 | Alta | 5 | Como estudante, quero que o assistente use um resumo da minha jornada em vez do histórico completo, para que o sistema economize consumo de IA sem perder contexto relevante. | RNF8 | ❌ |

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
