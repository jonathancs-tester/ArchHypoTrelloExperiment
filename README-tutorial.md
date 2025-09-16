# 📑 Sumário
- [📖 User Guide](#-user-guide)
  - [Como Usar (Passo a Passo)](#-como-usar-passo-a-passo)
    - [Criar um Board Template](#%EF%B8%8F-criar-um-board-template)
    - [Criar uma Incerteza](#-criar-uma-incerteza)
    - [Add/Atualizar Métricas](#%EF%B8%8F-addatualizar-métricas)
    - [Criar Plano Técnico](#-criar-plano-técnico)
    - [Visualizar Métricass](#-visualizar-métricas)
  
## 📖 User Guide

### 🚀 Como Usar (Passo a Passo)

#### #### 🗂️ Criar um Board Template

❗❗❗ **IMPORTANTE:** Os quadros compartilhados já foram previamente configurados com as colunas necessárias. Caso esteja criando um board do zero, siga as instruções abaixo. ❗❗❗

Para utilizar o plugin ArchHypo.AI corretamente, é essencial que o quadro do Trello esteja estruturado com as colunas adequadas para o fluxo de trabalho de gestão de incertezas e decisões arquiteturais.

1. Clique no ícone de **Board** na barra lateral do Trello, conforme mostrado na imagem abaixo:

   ![Add Board Template](img/image-1.png)

2. Crie as seguintes colunas no seu quadro:

   - `INCERTEZA`
   - `ITEM PLANO TÉCNICO`
   - `A FAZER`
   - `EM ANDAMENTO`
   - `CONCLUÍDO`

   Essas colunas organizam o processo desde a identificação de incertezas até a execução e acompanhamento das ações técnicas.

![Board Template](img/image.png)

💡 *Dica:* Você pode adicionar colunas personalizadas conforme as necessidades específicas do seu projeto ou equipe.


#### ❓ Criar uma Incerteza
Clique em *"Criar uma Incerteza"* para iniciar o fluxo de criação da Incerteza.

![Nova Incerteza](img/image-2.png)

**1) Descreva a Incerteza:**

DIgite a incerteza arquitetural identificada com maior detalhamento possivel

![Nova Inceteza 2](img/image-3.png)

---

**2)Hipótese:**

O modelo de linguagem (LLM) sugere automaticamente uma hipótese técnica relacionada à incerteza descrita e a justificativa.
Exemplo de hipótese sugerida:
_"A principal incerteza reside em como garantir a eficácia e a colaboração fluída entre os Agentes LLM..."_

![Hipotese](img/image-4.png)

O usuário pode editar a hipótese sugerida e o ArchHypo.AI Plugin solicitará uma justificativa para ser utilizada no aprendizado do LLM.

---

**3) Requisito Não Funcional (NFR):**

O sistema solicita que o usuário selecione ou justifique o requisito não funcional relacionado à hipótese (ex: desempenho, segurança, interoperabilidade).
![NFR](img/image-5.png)

---

**4)Avaliação da Incerteza:**

A incerteza é classificada em termos de nível (ex: Alto, Médio, Baixo), o que representa o grau de desconhecimento ou risco associado àquela questão.

![Incerteza](img/image-6.png)

---

**5)Avaliação do Impacto:**

Após a sugestão da hipótese, o sistema solicita que o usuário avalie o impacto que essa hipótese pode ter na arquitetura do sistema.

![Impacto](img/image-7.png)

O impacto refere-se às consequências técnicas caso a hipótese se confirme ou não.
O usuário pode selecionar o nível de impacto (ex: Alto, Médio, Baixo), considerando fatores como:
 - Complexidade da implementação
 - Riscos para desempenho, segurança ou interoperabilidade
 - Dependência entre componentes


---

Ao finalizar esses passos os card é criado com sucesso conforme a imagem abaixo:

![Card Criado](img/image-8.png)

**Navegação:**

Botões "Anterior" e "Próximo" permitem navegar entre as etapas do fluxo. Porém o não mantem o valor sugerido pelo LLM caso volte a etapa

---
  
#### 🏷️ Add/Atualizar Métricas  
Clique em *"Add/Atualizar Métricas"* para configurar os labels.
  - Hipóteses → *Nível de Incerteza, Impacto e Requisito Não Funcional*  
  - Itens do Plano Técnico → *Padrões ArchHypo*  

![Botao Power UP](img/image-9.png)

![Add/Atualizar Métrica](img/image-10.png)

![Metricas Adicionado](img/image-11.png)

#### 📋 Criar Plano Técnico  
   - Abra o card da hipótese criada.  
   - Clique em *"Plano Técnico"* → *"Gerar Plano Técnico"*.  
   - Selecione os itens sugeridos para editar ou gerar padrões ArchHypo.  
   - 💡 O LLM sugere informações + justificativas (editáveis).

![Botao Power Up](img/image-9.png)

![Bottao Plano Tecnico](img/image-12.png)

![Gerar](img/image-13.png)

![Editar](img/image-14.png)

![Padrao](img/image-15.png)

![Plano Criar](img/image-16.png)

   - Os itens são adicionados na coluna **ITEMS PLANO TÉCNICO**, com IDs no formato:  
     - `H1` → Hipótese 1  
     - `TPI1` → Tech Plan Item 1

   ![Plano Board](img/image-17.png)
   
#### 📊 **Visualizar Métricas** 

Use *ArchHypo Métricas* para acompanhar evolução em gráficos e gerenciar as métricas e labels de categorização de Hipóteses e Itens de Plano Técnico.

![Botao Métricas](img/image-18.png)

![Métricas](img/image-19.png)


--------------------------------------------------------------------------------------------------------------------

ArchHypo.AI Plugin

Equipe de Pesquisa e Desenvolvimento

[https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)


