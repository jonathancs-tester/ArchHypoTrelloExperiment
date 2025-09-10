# Padrões do ArchHypo

# 📑 Sumário
- [Architectural Spike](#architectural-spike)
- [Architectural Trigger](#architectural-trigger)
- [Bring the Specialist](#bring-the-specialiste)
- [Continuous Inspection](#continuous-inspection)
- [Learning from Experiments](#learning-from-experiments)
- [Plan for Preparation](#plan-for-preparation)
- [Postpone Uncertain Decisions](#postpone-uncertain-decisions)
- [Protective Guideline](#protective-guideline)
- [Quality Checkpoint](#quality-checkpoint)
- [Software Analytics (What You Need to Know)](#software-analytics-what-you-need-to-know) 
- [Technical Debt Management](#technical-debt-management)
- [Tracer Bullets](#tracer-bullets)

---
## Architectural Spike
**Explicação:**

Utilizado quando há incerteza técnica sobre uma solução arquitetural. Consiste em desenvolver uma implementação mínima e temporária para explorar a viabilidade de uma tecnologia ou abordagem, permitindo aprendizado rápido sem comprometer o projeto principal.

**Exemplo:**

Antes de adotar WebAssembly para acelerar partes de um sistema web, a equipe cria um protótipo simples que executa uma função crítica e mede o desempenho comparado ao JavaScript.

---

## Architectural Trigger
**Explicação:**

Esse padrão identifica eventos ou mudanças que exigem uma reavaliação ou tomada de decisão arquitetural. Pode ser uma mudança de requisitos, aumento de escala, nova regulamentação ou adoção de tecnologia emergente. Reconhecer esses gatilhos ajuda a manter a arquitetura alinhada com os objetivos do negócio.

**Exemplo:**

A entrada em vigor da LGPD obriga a equipe a revisar a arquitetura de dados para garantir anonimização e consentimento explícito, disparando uma decisão sobre o uso de serviços de gerenciamento de privacidade.

--- 

## Bring the Specialist
**Explicação:**

Quando a equipe enfrenta uma decisão arquitetural complexa ou fora de sua expertise, esse padrão recomenda envolver especialistas — seja em segurança, IA, redes, ou domínio de negócio — para garantir decisões bem fundamentadas e evitar riscos técnicos.

**Exemplo:**

Ao projetar uma solução de reconhecimento facial para controle de acesso, a equipe convida um especialista em visão computacional para definir os requisitos de precisão e evitar vieses algorítmicos.

---
  
## Continuous Inspection
**Explicação:**

Esse padrão promove a revisão contínua da arquitetura ao longo do ciclo de vida do projeto. Ele ajuda a identificar desvios, riscos emergentes e oportunidades de melhoria, mantendo a arquitetura saudável e adaptável.

**Exemplo:**

Se implementarmos monitoramento contínuo na arquitetura, com análise automática de qualidade de código, vulnerabilidades de segurança e desempenho, então seremos capazes de identificar problemas arquiteturais, técnicos e operacionais de forma antecipada, evitando débitos técnicos e falhas em produção.
---
  
## Learning from Experiments
**Explicação:**

Sugere que decisões arquiteturais sejam precedidas por experimentos controlados, que gerem dados e aprendizados reais. Isso reduz riscos e aumenta a confiança na escolha feita.

**Exemplo:**

A equipe testa três modelos de recomendação de produtos em ambientes de teste com dados reais para decidir qual oferece melhor precisão e tempo de resposta.

---

## Plan for Preparation
**Explicação:**

Esse padrão incentiva preparar a arquitetura para decisões futuras, mesmo que elas ainda não estejam maduras. Isso inclui criar flexibilidade, modularidade e abstrações que permitam mudanças com baixo custo.

**Exemplo:**

Se definirmos antecipadamente todas as atividades, recursos, ferramentas e responsabilidades necessárias para iniciar o projeto, então poderemos garantir uma preparação eficiente que minimizará riscos, atrasos e incertezas durante a fase de execução.

---

## Postpone Uncertain Decisions
**Explicação:**

Quando uma decisão envolve muitas variáveis desconhecidas ou riscos altos, esse padrão recomenda adiá-la até que mais informações estejam disponíveis. Isso evita decisões precipitadas e permite aprendizado incremental.

**Exemplo:**

A equipe evita escolher entre containers ou serverless para o backend até que o volume de requisições e o perfil de uso estejam mais claros após o MVP.

---

## Protective Guideline
**Explicação:**

Estabelece diretrizes arquiteturais que protegem o projeto contra decisões inconsistentes, técnicas inadequadas ou violações de padrões. Essas diretrizes funcionam como guardrails para manter a integridade da arquitetura.

**Exemplo:**

A equipe define que todos os serviços devem usar autenticação OAuth2 e que nenhuma biblioteca externa pode ser usada sem revisão de segurança, evitando vulnerabilidades.

---

## Quality Checkpoint
**Explicação:**

Cria momentos específicos para avaliar se a arquitetura está atendendo aos atributos de qualidade definidos (como desempenho, segurança, escalabilidade). Esses checkpoints ajudam a garantir que os objetivos técnicos não sejam comprometidos.

**Exemplo:**

A cada entrega de sprint, a equipe executa testes de carga e segurança automatizados para validar que o sistema continua dentro dos limites aceitáveis de latência e vulnerabilidades.

---

## Software Analytics (What You Need to Know)
**Explicação:**

Esse padrão foca em identificar lacunas de conhecimento que impedem decisões arquiteturais. Ele incentiva a busca ativa por informações críticas, seja por pesquisa, entrevistas ou análise de dados.

**Exemplo:**

Antes de definir a arquitetura de cache, a equipe precisa saber o tempo médio de acesso e o volume de dados por sessão. Eles coletam essas métricas com o time de produto e usuários reais.

---

## Technical Debt Management
**Explicação:**

Esse padrão trata da identificação, priorização e mitigação da dívida técnica acumulada ao longo do projeto. Ignorar essas dívidas pode comprometer a evolução da arquitetura e aumentar o custo de manutenção.

**Exemplo:**

A equipe mantém um quadro com dívidas técnicas categorizadas por impacto e esforço, e reserva parte do tempo de desenvolvimento para eliminar as mais críticas, como duplicação de lógica ou ausência de testes.

---

## Tracer Bullets
**Explicação:**

Implementações mínimas que percorrem o sistema de ponta a ponta, usadas para validar fluxos, integração e arquitetura geral. São úteis para testar hipóteses rapidamente e garantir que os componentes se comunicam corretamente.

**Exemplo:**

Antes de desenvolver todos os módulos de um sistema de reservas, a equipe cria um fluxo básico que vai do front-end até o banco de dados, passando por autenticação e API, validando a arquitetura geral.

---

ArchHypo.AI Plugin

Equipe de Pesquisa e Desenvolvimento

[https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)
