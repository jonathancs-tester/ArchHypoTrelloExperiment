# ArchWISE

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


```mermaid
flowchart TB

subgraph Discovery["Discovery"]
    U[Uncertainty Discovery]
    H[Hypothesis Formulation]
end

subgraph Analysis["Analysis"]
    NFR[NFR ]
    IA[Impact Assessment ]
    UA[Uncertainty Assessment ]
    TA[Trade-offs]
end

subgraph Experimentation["Experimentation"]
    TP[Technical Plan]
    AP[ArchHypo Pattern]
    S[Spike]
    P[PoC]
    EX[Experiment]
end

subgraph Learning["Learning"]
    EC[Evidence Collection]
    LA[Learning]
end

subgraph Decision["Decision"]
    DA[Decision]
    ADR[ADR]
end

subgraph Governance["Governance"]
    TR[Traceability]
    PR[Portfolio Risk]
end

U --> H

H --> NFR
H --> IA
H --> UA
H --> TA

NFR --> TP
IA --> TP
UA --> TP
TA --> TP

TP --> AP
TP --> S
TP --> P
TP --> EX

AP --> EC
S --> EC
P --> EC
EX --> EC

EC --> LA

LA --> DA

DA --> ADR
DA --> TR

TR --> PR

%% Cross-cutting concern
KB[(Knowledge Base)]

KB -.-> U
KB -.-> H
KB -.-> TP
KB -.-> DA
KB -.-> TR
```

## Core Agent

### Mandatory Components

| Componente           | Responsabilidade              |
| -------------------- | ----------------------------- |
| Agent Orchestrator   | Coordena agentes              |
| Agent Registry       | Disponibiliza os agentes   |
| Memory Layer         | Contexto compartilhado        |
| Knowledge Layer      | ADRs, requisitos, arquitetura (RAG)|
| Governance Layer     | Permissões e auditoria        |
| Evaluation Layer     | Qualidade/Padronização das respostas       |
| Observability Layer  | Métricas dos agentes          |
| Tool Connector Layer | Integrações externas    (Opcional)      |


```mermaid
flowchart TB

    subgraph Platform["ArchHypo Agent Framework"]

        ORCH[Agent Orchestrator]

        subgraph Foundation["Foundation Services"]

            REG[Agent Registry]
            MEM[Memory Layer]
            KNOW[Knowledge Layer]
        end

        subgraph Governance["Governance Services"]

            GOV[Governance Layer]
            EVAL[Evaluation Layer]
            OBS[Observability Layer]
        end

        subgraph Integration["Integration Services"]

            TOOL[Tool Connector Layer]
        end

    end

    ORCH <--> REG

    ORCH <--> MEM
    ORCH <--> KNOW

    ORCH --> GOV
    ORCH --> EVAL
    ORCH --> OBS

    ORCH --> TOOL
  ```
