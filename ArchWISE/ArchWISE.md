# Arquitetura ArchHypo Agent Harness

## Visão Geral

A arquitetura **ArchHypo Agent Harness** segue um modelo de **Sistema Hierárquico de Agentes Autônomos** (*Hierarchical Autonomous Multi-Agent System*).

Diferentemente de arquiteturas baseadas em um fluxo rígido de grafos, o **Coordinator Agent** é responsável apenas por compreender o objetivo, planejar em alto nível e delegar tarefas aos especialistas.

Cada **Subagent** encapsula toda a inteligência necessária para resolver seu domínio de atuação, incluindo planejamento, raciocínio, loops internos, uso de ferramentas, acesso à memória e até mesmo a criação de novos Subagents.

A **Harness Platform** fornece toda a infraestrutura compartilhada necessária para execução dos agentes, como memória, base de conhecimento, integrações, governança e observabilidade.

---

## Coordinator Agent

Responsabilidades:

- compreender o objetivo;
- criar o planejamento estratégico;
- selecionar especialistas;
- delegar objetivos;
- monitorar execuções;
- consolidar resultados;
- tomar a decisão final.

O Coordinator permanece simples e desacoplado da lógica específica de cada domínio.

---

## Subagents

Cada Subagent representa um especialista autônomo.

Suas capacidades incluem:

- planejamento;
- raciocínio;
- reflexão;
- utilização de ferramentas;
- acesso à memória;
- recuperação de conhecimento;
- autoavaliação;
- loops internos;
- criação dinâmica de novos Subagents.

Cada especialista é responsável por sua própria estratégia de execução.

---

## Harness Platform

A Harness Platform disponibiliza serviços compartilhados para todos os agentes.

### Camada de Memória

- Memória de Trabalho;
- Memória Conversacional;
- Memória de Longo Prazo;
- Banco Vetorial.

### Camada de Conhecimento

- ADRs;
- Documentação Arquitetural;
- Boas Práticas;
- Lições Aprendidas;
- Padrões Arquiteturais.

### Ferramentas

- GitHub;
- MCP Servers;
- Busca;
- Análise de Código;
- Processadores de Documentos.

### Integrações

- LLMs;
- APIs;
- CI/CD;
- Sistemas Corporativos;
- Notificações.

### Governança

- Controle de Acesso;
- Auditoria;
- Políticas;
- Segurança.

### Observabilidade

- Logs;
- Métricas;
- Traces;
- Dashboards;
- Monitoramento de Custos;
- Consumo de Tokens.

---

# Benefícios da Arquitetura

Esta arquitetura oferece diversas vantagens:

- o Coordinator permanece simples, independentemente do crescimento do sistema;
- cada Subagent pode evoluir de forma independente;
- novos especialistas podem ser adicionados sem modificar a orquestração;
- toda a lógica especializada permanece encapsulada;
- a criação dinâmica de novos agentes permite resolver problemas cada vez mais complexos;
- a infraestrutura compartilhada reduz duplicação de funcionalidades;
- o aprendizado contínuo melhora progressivamente a qualidade das decisões arquiteturais.

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/015d4050-5867-42b5-bad7-57b101564ead" />

<!-- <img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/1e8aebd5-9d17-4120-b338-990945e8061a" /> -->


# Fluxo de Execução

## Passo 1 — Recebimento do Objetivo

O processo inicia quando um usuário fornece um objetivo de alto nível.

Exemplos:

- Identificar incertezas arquiteturais;
- Gerar hipóteses arquiteturais;
- Avaliar uma arquitetura de software;
- Gerar um ADR;
- Analisar trade-offs;
- Planejar experimentos arquiteturais.

Neste momento, o **Coordinator Agent** entende apenas **o que deve ser feito**, mas não **como será executado**.

---

## Passo 2 — Planejamento Estratégico

O Coordinator Agent analisa:

- objetivo solicitado;
- contexto disponível;
- artefatos arquiteturais;
- restrições;
- decisões anteriores;
- especialistas disponíveis.

Com essas informações, ele cria um plano de execução de alto nível.

Exemplo:

```
Objetivo

↓

Discovery Agent
↓

Hypothesis Agent
↓

Impact Agent
↓

Trade-off Agent
```

O Coordinator define apenas quais especialistas serão responsáveis pela execução.

---

## Passo 3 — Delegação dos Objetivos

Após o planejamento, o Coordinator delega objetivos para um ou mais Subagents.

```
Coordinator Agent

↓

Hypothesis Subagent
```

Cada delegação contém:

- objetivo;
- contexto;
- requisitos;
- restrições;
- critérios de sucesso;
- artefatos necessários.

O Coordinator **não define o algoritmo interno** que será utilizado pelo especialista.

---

## Passo 4 — Execução Autônoma do Subagent

Ao receber a tarefa, o Subagent torna-se completamente autônomo.
Cada Subagent possui seus próprios loop/ciclos de raciocínio.

Ele pode executar diversas skills internamente, como:

- elaborar um plano;
- refletir sobre o problema;
- executar raciocínio iterativo;
- consultar memória;
- recuperar conhecimento via RAG;
- utilizar ferramentas externas;
- validar resultados;
- refinar respostas.

Toda essa lógica permanece encapsulada.

Enquanto isso, o Coordinator apenas acompanha o estado da execução.

---

## Passo 5 — Utilização de Ferramentas

Durante sua execução, o Subagent pode utilizar diversos recursos externos, por exemplo:

- GitHub;
- Jira;
- Confluence;
- Banco Vetorial;
- RAG;
- MCP Servers;
- APIs internas;
- Bancos de Dados;
- Modelos de Linguagem (LLMs);
- Documentações arquiteturais.

O Coordinator não precisa conhecer quais ferramentas estão sendo utilizadas.

---


## Passo 6 — Retorno dos Resultados

Ao concluir sua execução, o Subagent retorna:

- descobertas;
- evidências;
- nível de confiança;
- riscos identificados;
- recomendações;
- métricas;
- rastreabilidade.

---

## Passo 7 — Consolidação dos Resultados

O Coordinator reúne as informações produzidas pelos diversos especialistas.

Exemplo:

```
Discovery

+

Hypothesis

+

Impact

+

Trade-off

+

Evidence

↓

Decisão
```

Neste momento ocorre a síntese das informações.

---

## Passo 8 — Tomada de Decisão

Com todas as evidências disponíveis, o Coordinator decide entre:

- finalizar o processo;
- solicitar outro especialista;
- executar novos experimentos;
- buscar mais evidências;
- retornar o resultado ao usuário.

---

## Passo 9 — Geração dos Artefatos

Dependendo do objetivo inicial, a arquitetura pode produzir:

- ADRs;
- Hipóteses Arquiteturais;
- Relatórios Técnicos;
- Evidências;
- Planos de Experimentos;
- Avaliações de Riscos;
- Atualizações da Base de Conhecimento.

---

## Passo 10 — Aprendizado Contínuo

Após a execução, todo conhecimento gerado pode ser armazenado para reutilização futura.

Exemplos:

- novas evidências;
- ADRs;
- lições aprendidas;
- métricas;
- decisões arquiteturais;
- resultados experimentais.

Nas próximas execuções, os agentes poderão utilizar esse conhecimento para tomar decisões melhores.

---

## SubAgents Catalog

<img width="1693" height="1361" alt="image" src="https://github.com/user-attachments/assets/87baa06d-f5e8-44ba-a685-d97836d34717" />

| SubAgents                     | Categoria              | Descrição                                                   | Input                      | Output                   |
| ----------------------------- | -------------     | ----------------------------------------------------------- | -------------------------- | ------------------------ |
| Uncertainty Discovery Agent   | Discovery         | Identifica incertezas em requisitos, tecnologias e decisões | Backlog, ADRs, requisitos  | Lista de incertezas      |
| Hypothesis Formulation Agent  | Discovery         | Converte incertezas em hipóteses testáveis                  | Incertezas identificadas   | Hipóteses estruturadas   |
| NFR Agent                     | Analysis          | Classifica a hipotese em NFR                                | Hipótese                   | NFR                      |
| Impact Assessment Agent       | Analysis          | Avalia impacto potencial da hipótese                        | Hipótese                   | Score de impacto         |
| Uncertainty Assessment Agent  | Analysis          | Mede nível de incerteza                                     | Hipótese, evidências       | Score de incerteza       |
| Trade-off  Agent              | Analysis          | Analisa trade-offs arquiteturais                            | Alternativas arquiteturais | Matriz de trade-offs     |
| Technical Plan Agent          | Experimentation   | Define plano técnico para validar hipótese                  | Hipótese + risco           | Plano de experimentação  |
| Architectural Patterns Agent  | Experimentation   | Classifica a hipótese dado ArchHypo Patterns                | Hipótese                   | ArchHypo Pattern        |
| Experiment Agent              | Experimentation   | Gera provas de conceito                                     | Hipótese, arquitetura      | Resultado do PoC         |
| Evidence Collection Agent     | Learning          | Coleta evidências dos experimentos                          | Logs, métricas, testes     | Evidências               |
| Learning Agent                | Learning          | Extrai aprendizados                                         | Evidências                 | Lições aprendidas        |
| Decision Agent                | Decision          | Decide confirmar, refutar ou adiar hipótese                 | Evidências e aprendizados  | Decisão                  |
| Documentation Agent           | Decision          | Gera Architecture Decision Records                          | Decisão                    | ADR                      |
| Continuous Architecture Agent | Decision          | Sugere decisões adiáveis                                    | Roadmap e hipóteses        | Backlog arquitetural     |


# Skill Catalog

## 🔍 Discovery

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `uncertainty_identification` | Discovery | Identifies uncertainties across requirements, architecture, and tech decisions | Uncertainty Discovery Agent |
| `uncertainty_classification` | Discovery | Classifies uncertainty (technical, business, integration, operational) | Uncertainty Discovery Agent |
| `context_framing` | Discovery | Organizes business, system context, constraints, NFRs | Uncertainty Discovery Agent |
| `problem_structuring` | Discovery | Separates problem, symptoms, scope, and unknowns | Uncertainty Discovery Agent |

---

## 🧪 Hypothesis

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `hypothesis_generation` | Hypothesis | Generates testable hypotheses from uncertainty | Hypothesis Formulation Agent |
| `hypothesis_structuring` | Hypothesis | Structures hypothesis (If / When / Then + measurable outcome) | Hypothesis Formulation Agent |
| `assumption_extraction` | Hypothesis | Extracts implicit and explicit assumptions | Hypothesis Formulation Agent |
| `decision_option_generation` | Hypothesis | Generates architectural alternatives | Hypothesis Formulation Agent |

---

## 📊 Analysis

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `nfr_classification` | Analysis | Classifies hypothesis into NFR category (latency, cost, security…) | NFR Agent |
| `impact_mapping` | Analysis | Maps impacted systems, domains, flows, teams | Impact Assessment Agent |
| `impact_scoring` | Analysis | Scores business/technical impact | Impact Assessment Agent |
| `uncertainty_scoring` | Analysis | Measures uncertainty level (low → high) | Uncertainty Assessment Agent |
| `dependency_analysis` | Analysis | Identifies dependencies and rollout sequencing | Impact Assessment Agent |
| `risk_identification` | Analysis | Identifies technical/operational/security risks | Impact / NFR / Trade-off Agent |
| `tradeoff_matrix_generation` | Analysis | Builds trade-off matrix (pros/cons/risks) | Trade-off Agent |
| `architecture_option_comparison` | Analysis | Compares alternatives against criteria | Trade-off Agent |

---

## 🧪 Experimentation

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `validation_strategy_selection` | Experimentation | Chooses validation type (PoC, spike, benchmark, etc.) | Technical Plan Agent |
| `experiment_design` | Experimentation | Defines experiment scope, tasks, architecture | Technical Plan Agent |
| `success_criteria_definition` | Experimentation | Defines measurable success/failure criteria | Technical Plan Agent |
| `evidence_collection_strategy` | Experimentation | Defines metrics/logs/data to collect | Technical Plan Agent |
| `pattern_classification` | Experimentation | Maps hypothesis to ArchHypo architectural patterns | Architectural Patterns Agent |
| `poc_execution` | Experimentation | Executes experiment/PoC | Experiment Agent |

---

## 📚 Learning

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `evidence_collection` | Learning | Collects raw experiment outputs (logs, metrics) | Evidence Collection Agent |
| `evidence_consolidation` | Learning | Aggregates evidence into structured view | Learning Agent |
| `learning_extraction` | Learning | Extracts lessons learned | Learning Agent |
| `knowledge_update` | Learning | Updates memory/context with learnings | Learning Agent |

---

## 🎯 Decision

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `decision_evaluation` | Decision | Evaluates hypothesis vs evidence | Decision Agent |
| `decision_classification` | Decision | Classifies outcome: confirm / refute / postpone | Decision Agent |
| `decision_reasoning` | Decision | Explains rationale from evidence | Decision Agent |
| `adr_drafting` | Decision | Generates ADR (context, decision, consequences) | Documentation Agent |
| `continuous_architecture_planning` | Decision | Suggests postponed decisions and backlog evolution | Continuous Architecture Agent |
| `rollout_guidance_generation` | Decision | Suggests rollout/migration/rollback strategies | Continuous Architecture Agent |

---

## 🧩 Support / Cross-cutting

| Skill | Category | What it does | Primary agents |
|---|---|---|---|
| `architecture_pattern_matching` | Support | Suggests patterns for given hypothesis | Hypothesis / Trade-off |
| `architecture_smell_detection` | Support | Detects architectural smells and inconsistencies | Discovery / Impact |
| `traceability_linking` | Support | Links hypothesis → experiment → evidence → decision (audit trail) | All |
| `context_enrichment` | Support | Enriches context with external/internal knowledge | Discovery / Learning |

