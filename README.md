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

<p>O CHATin é um <b>coach de estudos via chat com IA</b>: o estudante conversa livremente sobre o que está estudando, e o assistente busca fontes confiáveis para embasar as respostas (sempre citando de onde tirou a informação), podendo também usar documentos que o próprio estudante anexar à conversa. A qualquer momento, o estudante pode pedir para gerar um <b>resumo</b> da conversa, que fica salvo na <b>Biblioteca</b> — um repositório pessoal de resumos, privado por usuário. A partir de um ou mais resumos salvos, o estudante gera um <b>questionário com gabarito</b>, responde e recebe <b>correção automática</b>. O engajamento é reforçado por uma camada de desempenho: XP por questionário concluído, sequência de dias de estudo (streak), percentual médio de acerto, contagem de resumos revisados e um <b>ranking</b> comparando o XP dos estudantes (identificados por apelido, não pelo nome real). O chat não sugere assunto por conta própria — é sempre o estudante quem dá o ponto de partida da conversa, e a IA se adapta ao tema que for trazido, o que já torna o produto naturalmente aplicável a qualquer domínio de estudo, validado inicialmente no contexto de preparação para o vestibular.</p>

---

## Cronograma de Sprints <a name="cronograma"></a>

| Sprint | Período | Status | Relatório |
|:------:|:-------:|:------:|:---------:|
| 1 | 07/09/2026 à 27/09/2026 | Em Andamento | [Ver Relatório](https://github.com/Equipe-Skyfall/chatin/tree/main/docs/sprint1) |
| 2 | 05/10/2026 à 25/10/2026 | Não iniciado | — |
| 3 | 02/11/2026 à 22/11/2026 | Não iniciado | — |

---

## 💻 Tecnologias utilizadas <a name="tecnologias"></a>

| Tecnologia | Finalidade |
|:----------:|------------|
| ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white) ![Lucide](https://img.shields.io/badge/Lucide-1E1E1E?style=for-the-badge&logo=lucide&logoColor=white) | Frontend / App |
| ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) | Backend / API |
| ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white) | Banco de Dados |
| ![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white) | Provedor de IA / PLN |
| ![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white) | Interface / Design e prototipação |
| ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white) | Empacotamento / Deploy |

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
| RF1 | Cadastro e Login | O sistema deve permitir que o estudante crie uma conta (com apelido) e faça login. |
| RF2 | Chat com o Coach de IA | O sistema deve permitir uma conversa livre entre o estudante e o assistente, sempre iniciada pelo estudante. |
| RF3 | Busca e Citação de Fontes | O sistema deve buscar fontes confiáveis sobre o assunto da conversa e sempre indicar de onde a informação foi retirada. |
| RF4 | Anexar Documentos ao Chat | O sistema deve permitir que o estudante envie documentos para auxiliar a IA durante a conversa. |
| RF5 | Geração de Resumo | O sistema deve gerar, sob pedido, um resumo da conversa e salvá-lo como um arquivo na Biblioteca. |
| RF6 | Biblioteca de Resumos | O sistema deve permitir listar, abrir e revisar os resumos salvos pelo estudante. |
| RF7 | Seleção de Resumos para Questionário | O sistema deve permitir selecionar um ou mais resumos da Biblioteca para gerar um questionário. |
| RF8 | Geração de Questionário e Gabarito | O sistema deve gerar um questionário com gabarito a partir dos resumos selecionados. |
| RF9 | Correção do Questionário | O sistema deve corrigir automaticamente as respostas do estudante comparando com o gabarito. |
| RF10 | Registro de Desempenho | O sistema deve registrar o resultado de cada questionário respondido pelo estudante. |
| RF11 | Gamificação — XP | O sistema deve conceder XP ao estudante a cada questionário concluído. |
| RF12 | Gamificação — Streak de Estudos | O sistema deve contar a sequência de dias consecutivos em que o estudante respondeu ao menos um questionário. |
| RF13 | Percentual Médio de Acerto | O sistema deve calcular e exibir a % média de acerto do estudante nos questionários. |
| RF14 | Ranking entre Usuários | O sistema deve exibir um ranking comparando o XP dos estudantes, identificados por apelido. |
| RF15 | Contagem de Cards Revisados | O sistema deve contar quantos resumos da Biblioteca o estudante já revisou. |

### Requisitos Não Funcionais

| RNF | Nome | Descritivo |
|-----|------|------------|
| RNF1 | Manual de Instalação | Documentação obrigatória (Fatec) explicando como instalar e rodar o projeto. |
| RNF2 | Manual do Usuário | Documentação obrigatória (Fatec) explicando como usar a aplicação. |
| RNF3 | Documentação da API | Documentação dos principais endpoints/integrações da API. |
| RNF4 | Modelagem de Dados | Modelo do banco de dados ou estrutura de persistência utilizada, documentado. |
| RNF5 | Segurança de Segredos | Chaves e segredos de APIs externas não podem ficar hardcoded no código-fonte. |
| RNF6 | Resiliência à Falha de IA | A aplicação deve continuar funcional (Biblioteca, resumos salvos, desempenho registrado) mesmo com a IA indisponível ou cota esgotada. |
| RNF7 | Controle de Consumo de IA | O sistema deve registrar e exibir o consumo de IA (nº de chamadas e, quando disponível, tokens). |
| RNF8 | Redução de Consumo de IA | O sistema deve aplicar ao menos uma estratégia de redução de consumo (ex.: memória resumida do estudante em vez de reenviar histórico completo). |
| RNF9 | Privacidade da Biblioteca e Conversas | Resumos salvos na Biblioteca e o histórico de conversas do chat são estritamente privados por usuário; o Ranking (RF14) expõe apenas apelido e XP, nunca o conteúdo estudado. |

---

## 🏗 Arquitetura <a name="arquitetura"></a>

<img src="docs/arquitetura.jpg">

---

## 🖥 Wireframes <a name="wireframes"></a>

- [Wireframe do produto](docs/wireframe/Wireframe_CHATin.pdf)

---

## 📜 Product Backlog <a name="backlog"></a>

| RANK | SPRINT | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:------:|:----------:|:----------:|------------|:--:|:------:|
| 1 | 1 | Alta | 8 | Como estudante, quero conversar livremente com o assistente sobre o que estou estudando, para tirar dúvidas e receber apoio sobre o assunto que eu trouxer. | RF2 | ⬜ |
| 2 | 1 | Alta | 8 | Como estudante, quero que o assistente busque fontes confiáveis sobre o assunto da conversa e sempre me mostre de onde tirou a informação, para confiar no que está sendo dito. | RF3 | ⬜ |
| 3 | 1 | Média | 5 | Como estudante, quero anexar documentos à conversa, para que o assistente use esse material como apoio ao me responder. | RF4 | ⬜ |
| 4 | 1 | Alta | 5 | Como estudante, quero pedir para o assistente gerar um resumo da conversa a qualquer momento, para guardar o conteúdo estudado. | RF5 | ⬜ |
| 5 | 1 | Alta | 5 | Como estudante, quero acessar uma biblioteca com todos os resumos que já salvei, para revisar o que estudei quando quiser. | RF6 | ⬜ |
| 6 | 2 | Alta | 5 | Como estudante, quero selecionar um ou mais resumos da minha biblioteca, para gerar um questionário sobre esse conteúdo. | RF7 | ⬜ |
| 7 | 2 | Alta | 8 | Como estudante, quero receber um questionário com gabarito gerado a partir dos resumos que selecionei, para testar meu conhecimento sobre eles. | RF8 | ⬜ |
| 8 | 2 | Alta | 5 | Como estudante, quero responder o questionário e ver minha correção automática, para saber o que acertei e errei. | RF9 | ⬜ |
| 9 | 2 | Alta | 5 | Como estudante, quero que meu desempenho em cada questionário seja registrado, para acompanhar minha evolução ao longo do tempo. | RF10 | ⬜ |
| 10 | 2 | Média | 5 | Como estudante, quero ganhar XP ao concluir um questionário, para acompanhar meu progresso de forma gamificada. | RF11 | ⬜ |
| 11 | 2 | Alta | 5 | Como estudante, quero que meus resumos salvos e meu histórico de desempenho continuem acessíveis mesmo se a IA estiver indisponível, para não perder o que já estudei. | RNF6 | ⬜ |
| 12 | 3 | Média | 5 | Como estudante, quero manter uma sequência de dias respondendo questionários (streak), para me sentir motivado a continuar estudando. | RF12 | ⬜ |
| 13 | 3 | Média | 5 | Como estudante, quero ver minha porcentagem média de acerto nos questionários, para entender meu nível geral de desempenho. | RF13 | ⬜ |
| 14 | 3 | Média | 8 | Como estudante, quero ver um ranking com o XP de outros estudantes (por apelido), para me sentir motivado a competir de forma saudável. | RF14 | ⬜ |
| 15 | 3 | Baixa | 5 | Como estudante, quero que o sistema conte quantos resumos da minha biblioteca eu já revisei, para acompanhar meu hábito de revisão. | RF15 | ⬜ |
| 16 | 3 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ⬜ |
| 17 | 3 | Alta | 5 | Como estudante, quero que o assistente use um resumo do meu histórico em vez de reenviar tudo para a IA a cada interação, para economizar consumo sem perder contexto relevante. | RNF8 | ⬜ |

---

## 📝 Sprint Backlog <a name="backsprint"></a>

> Os Critérios de Aceitação abaixo também estão detalhados, junto das Regras de Negócio, no [DoR (PDF)](docs/DoR_CHATin.pdf).

<details>
<summary><strong>Sprint 1 — Núcleo: Chat Coach e Biblioteca de Resumos</strong></summary>

<br>

> **Período:** 07/09/2026 à 27/09/2026
> **Foco:** O estudante conversa livremente com o assistente, que busca e cita fontes (e aceita documentos anexados), gera resumos sob pedido, e o estudante consegue revisá-los na Biblioteca.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 1 | Alta | 8 | Como estudante, quero conversar livremente com o assistente sobre o que estou estudando, para tirar dúvidas e receber apoio sobre o assunto que eu trouxer. | RF2 | ⬜ |
| 2 | Alta | 8 | Como estudante, quero que o assistente busque fontes confiáveis sobre o assunto da conversa e sempre me mostre de onde tirou a informação, para confiar no que está sendo dito. | RF3 | ⬜ |
| 3 | Média | 5 | Como estudante, quero anexar documentos à conversa, para que o assistente use esse material como apoio ao me responder. | RF4 | ⬜ |
| 4 | Alta | 5 | Como estudante, quero pedir para o assistente gerar um resumo da conversa a qualquer momento, para guardar o conteúdo estudado. | RF5 | ⬜ |
| 5 | Alta | 5 | Como estudante, quero acessar uma biblioteca com todos os resumos que já salvei, para revisar o que estudei quando quiser. | RF6 | ⬜ |

---

<details>
<summary>US01 — Chat livre com o assistente</summary>

**Critérios de Aceitação**
- [ ] O sistema deve permitir que o estudante envie mensagens de texto livre a qualquer momento.
- [ ] O assistente deve responder de forma coerente com o assunto trazido pelo estudante.
- [ ] O assistente não deve iniciar um novo assunto por conta própria — a conversa sempre parte do estudante.

</details>

<details>
<summary>US02 — Busca e citação de fontes</summary>

**Critérios de Aceitação**
- [ ] O sistema deve buscar fontes relacionadas ao assunto da conversa quando necessário para embasar a resposta.
- [ ] Toda resposta que utilizar uma fonte externa deve indicar de onde a informação foi retirada.
- [ ] As fontes citadas devem ser verificáveis (título e/ou link).

</details>

<details>
<summary>US03 — Anexar documentos à conversa</summary>

**Critérios de Aceitação**
- [ ] O estudante deve poder anexar um documento à conversa a qualquer momento.
- [ ] O conteúdo do documento anexado deve ser considerado pelo assistente nas respostas seguintes.
- [ ] Documentos em formato não suportado devem exibir mensagem de erro clara.

</details>

<details>
<summary>US04 — Geração de resumo da conversa</summary>

**Critérios de Aceitação**
- [ ] O estudante deve poder solicitar a geração de um resumo a qualquer momento durante a conversa.
- [ ] O resumo gerado deve ser salvo automaticamente como um novo arquivo na Biblioteca.
- [ ] O resumo deve refletir o conteúdo discutido até o momento do pedido.

</details>

<details>
<summary>US05 — Biblioteca de resumos salvos</summary>

**Critérios de Aceitação**
- [ ] A Biblioteca deve listar todos os resumos salvos pelo estudante, com título e data.
- [ ] O estudante deve poder abrir um resumo salvo para revisão a qualquer momento.
- [ ] A Biblioteca deve ser acessível apenas pelo próprio estudante (privada).

</details>

</details>

---

<details>
<summary><strong>Sprint 2 — Questionário a partir da Biblioteca</strong></summary>

<br>

> **Período:** 05/10/2026 à 25/10/2026
> **Foco:** O estudante seleciona resumos da Biblioteca para gerar um questionário, responde, recebe correção automática, tem o desempenho registrado e ganha XP — com resiliência caso a IA falhe.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 6 | Alta | 5 | Como estudante, quero selecionar um ou mais resumos da minha biblioteca, para gerar um questionário sobre esse conteúdo. | RF7 | ⬜ |
| 7 | Alta | 8 | Como estudante, quero receber um questionário com gabarito gerado a partir dos resumos que selecionei, para testar meu conhecimento sobre eles. | RF8 | ⬜ |
| 8 | Alta | 5 | Como estudante, quero responder o questionário e ver minha correção automática, para saber o que acertei e errei. | RF9 | ⬜ |
| 9 | Alta | 5 | Como estudante, quero que meu desempenho em cada questionário seja registrado, para acompanhar minha evolução ao longo do tempo. | RF10 | ⬜ |
| 10 | Média | 5 | Como estudante, quero ganhar XP ao concluir um questionário, para acompanhar meu progresso de forma gamificada. | RF11 | ⬜ |
| 11 | Alta | 5 | Como estudante, quero que meus resumos salvos e meu histórico de desempenho continuem acessíveis mesmo se a IA estiver indisponível, para não perder o que já estudei. | RNF6 | ⬜ |

---

<details>
<summary>US06 — Seleção de resumos para questionário</summary>

**Critérios de Aceitação**
- [ ] O estudante deve poder selecionar um ou mais resumos da Biblioteca.
- [ ] O sistema deve exigir ao menos um resumo selecionado antes de permitir gerar o questionário.
- [ ] A seleção deve permitir combinar resumos de conversas diferentes.

</details>

<details>
<summary>US07 — Geração de questionário e gabarito</summary>

**Critérios de Aceitação**
- [ ] O questionário deve ser gerado a partir do conteúdo dos resumos selecionados.
- [ ] Cada questão deve ter um gabarito associado, gerado junto com o questionário.
- [ ] O questionário deve conter uma quantidade mínima de questões definida pela equipe.

</details>

<details>
<summary>US08 — Correção automática do questionário</summary>

**Critérios de Aceitação**
- [ ] O estudante deve poder responder o questionário diretamente no aplicativo.
- [ ] O sistema deve corrigir automaticamente as respostas comparando com o gabarito.
- [ ] O estudante deve visualizar quais questões acertou e errou ao final.

</details>

<details>
<summary>US09 — Registro de desempenho</summary>

**Critérios de Aceitação**
- [ ] Cada questionário corrigido deve gerar um registro de desempenho (data, resumos utilizados, resultado).
- [ ] O histórico de desempenho deve ficar vinculado ao perfil do estudante.
- [ ] Nenhum registro deve ser perdido em caso de falha da IA.

</details>

<details>
<summary>US10 — Ganho de XP por questionário concluído</summary>

**Critérios de Aceitação**
- [ ] O estudante deve ganhar XP ao concluir um questionário.
- [ ] O sistema deve exibir o XP atual do estudante.
- [ ] O cálculo de XP deve ser feito pela aplicação, não pela IA.

</details>

<details>
<summary>US11 — Resiliência à falha de IA</summary>

**Critérios de Aceitação**
- [ ] A Biblioteca e o histórico de desempenho devem continuar acessíveis mesmo com a IA indisponível.
- [ ] O chat deve sinalizar claramente quando não conseguir gerar uma resposta.
- [ ] Nenhuma funcionalidade não dependente de IA deve ficar bloqueada por essa falha.

</details>

</details>

---

<details>
<summary><strong>Sprint 3 — Desempenho Social e Governança de IA</strong></summary>

<br>

> **Período:** 02/11/2026 à 22/11/2026
> **Foco:** O estudante acompanha streak, % média de acerto, ranking entre usuários (por apelido) e cards revisados, enquanto a equipe garante controle e redução de consumo de IA.

| RANK | PRIORIDADE | ESTIMATIVA | USER STORY | RF | STATUS |
|:----:|:----------:|:----------:|------------|:--:|:------:|
| 12 | Média | 5 | Como estudante, quero manter uma sequência de dias respondendo questionários (streak), para me sentir motivado a continuar estudando. | RF12 | ⬜ |
| 13 | Média | 5 | Como estudante, quero ver minha porcentagem média de acerto nos questionários, para entender meu nível geral de desempenho. | RF13 | ⬜ |
| 14 | Média | 8 | Como estudante, quero ver um ranking com o XP de outros estudantes (por apelido), para me sentir motivado a competir de forma saudável. | RF14 | ⬜ |
| 15 | Baixa | 5 | Como estudante, quero que o sistema conte quantos resumos da minha biblioteca eu já revisei, para acompanhar meu hábito de revisão. | RF15 | ⬜ |
| 16 | Alta | 5 | Como administrador, quero visualizar o consumo de chamadas e tokens de IA, para controlar custo e uso do recurso. | RNF7 | ⬜ |
| 17 | Alta | 5 | Como estudante, quero que o assistente use um resumo do meu histórico em vez de reenviar tudo para a IA a cada interação, para economizar consumo sem perder contexto relevante. | RNF8 | ⬜ |

---

<details>
<summary>US12 — Streak de dias de estudo</summary>

**Critérios de Aceitação**
- [ ] O sistema deve contar a sequência de dias consecutivos em que o estudante respondeu ao menos um questionário.
- [ ] O streak deve ser exibido de forma visível na tela de Desempenho.
- [ ] A quebra do streak deve reiniciar a contagem a zero.

</details>

<details>
<summary>US13 — Percentual médio de acerto</summary>

**Critérios de Aceitação**
- [ ] O sistema deve calcular a % média de acerto com base em todos os questionários respondidos.
- [ ] O valor deve ser atualizado automaticamente a cada novo questionário concluído.
- [ ] A % deve ser exibida na tela de Desempenho.

</details>

<details>
<summary>US14 — Ranking entre usuários</summary>

**Critérios de Aceitação**
- [ ] O ranking deve exibir os estudantes ordenados por XP, do maior para o menor.
- [ ] O ranking deve identificar cada estudante apenas pelo apelido, nunca pelo nome real.
- [ ] O estudante deve conseguir identificar sua própria posição no ranking.

</details>

<details>
<summary>US15 — Contagem de cards revisados</summary>

**Critérios de Aceitação**
- [ ] O sistema deve contar quantas vezes o estudante abriu um resumo da Biblioteca para revisão.
- [ ] A contagem deve ser exibida na tela de Desempenho.
- [ ] Revisar o mesmo resumo mais de uma vez deve incrementar a contagem.

</details>

<details>
<summary>US16 — Controle de consumo de IA</summary>

**Critérios de Aceitação**
- [ ] O sistema deve registrar cada chamada feita à IA (data/hora e funcionalidade de origem).
- [ ] Quando disponível pelo provedor, o sistema deve registrar também a quantidade de tokens usados.
- [ ] O administrador deve conseguir visualizar um resumo do consumo por período.

</details>

<details>
<summary>US17 — Redução de consumo de IA</summary>

**Critérios de Aceitação**
- [ ] O sistema deve manter um resumo do histórico do estudante em vez do histórico completo.
- [ ] As chamadas à IA devem usar essa versão resumida como contexto.
- [ ] Deve ser possível demonstrar a redução de consumo obtida com a estratégia escolhida.

</details>

</details>

---

## Links Úteis <a name="links"></a>

- [Desafio do Parceiro Acadêmico (GSW)](docs/Desafio%20do%20Parceiro%20Academico%206DSM%20-%20GSW%20-%20final.pdf)

---

## 👥 Equipe <a name="equipe"></a>

| Foto | Função | Nome | LinkedIn | GitHub |
|:----:|:------:|:----:|:--------:|:------:|
| <img src="https://avatars.githubusercontent.com/u/160733714?v=4" width="75px"> | Dev Team | Eduardo da Silva Fontes | [LinkedIn](https://www.linkedin.com/in/eduardo-da-silva-fontes/) | [GitHub](https://github.com/DuuhZero) |
| <img src="https://avatars.githubusercontent.com/u/162118889?v=4" width="75px"> | Dev Team | Eduardo Kuwahara Jr. | [LinkedIn](https://www.linkedin.com/in/eduardo-kuwahara-3b2267303/) | [GitHub](https://github.com/EduardoKuwahara) |
| <img src="https://avatars.githubusercontent.com/u/144804717?v=4" width="75px"> | Dev Team | Fábio Hiroshi | [LinkedIn](https://www.linkedin.com/in/f%C3%A1bio-hiroshi-5393a51a0) | [GitHub](https://github.com/FabioHiros) |
| <img src="https://avatars.githubusercontent.com/u/162117916?v=4" width="75px"> | Product Owner | João Vitor Rossi Ferreira | [LinkedIn](https://www.linkedin.com/in/joão-rossi-7311a0301/) | [GitHub](https://github.com/joaorossiferreira) |
| <img src="https://avatars.githubusercontent.com/u/95691713?v=4" width="75px"> | Dev Team | Kathellyn Caroline Alves dos Santos | [LinkedIn](https://www.linkedin.com/in/kathellyn-caroline-a562101b9) | [GitHub](https://github.com/CarolineKathellyn) |
| <img src="https://avatars.githubusercontent.com/u/161987258?v=4" width="75px"> | Dev Team | Victor Daniel | [LinkedIn](https://www.linkedin.com/in/victor-daniel-ramos-bessa-1436a3215/) | [GitHub](https://github.com/victordanielrb) |
| <img src="https://avatars.githubusercontent.com/u/162117908?v=4" width="75px"> | Scrum Master | Paulo Henrique Martins de Almeida | [LinkedIn](https://www.linkedin.com/in/paulo-almeida-3102452a7/) | [GitHub](https://github.com/pauloalmeida46) |