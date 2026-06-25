# ArchWISE

<img width="1693" height="1361" alt="image" src="https://github.com/user-attachments/assets/87baa06d-f5e8-44ba-a685-d97836d34717" />

## Agents Catalog

| Agente                        | Tipo              | Descrição                                                   | Input                      | Output                   |
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


# Skill Catalog v2

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


## Core Agent

<img width="1062" height="1441" alt="image" src="https://github.com/user-attachments/assets/7d6447d0-39da-4393-b48f-fe3038d5066d" />

