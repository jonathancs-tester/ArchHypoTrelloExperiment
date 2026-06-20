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


## Core Agent


<img width="1062" height="1441" alt="image" src="https://github.com/user-attachments/assets/92f94edf-862e-4d33-9fa5-2bff1a8626b4" />
