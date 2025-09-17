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

---

**1) Descreva a Incerteza:**

DIgite a incerteza arquitetural identificada com maior detalhamento possivel

![Nova Inceteza 2](img/image-3.png)

---

**2)Hipótese:**

O modelo de linguagem (LLM) sugere automaticamente uma hipótese técnica relacionada à incerteza descrita e a justificativa.
Exemplo de hipótese sugerida:
_"A principal incerteza reside em como garantir a eficácia e a colaboração fluída entre os Agentes LLM..."_

![Hipotese](img/image-4.png)

⚠️**Atenção:** Ao retornar a uma etapa anterior, os valores sugeridos pelo LLM podem ser perdidos e precisarão ser reeditados.

⚠️**Atenção:** O usuário pode editar qualquer informação sugerido pelo LLM porém o ArchHypo.AI Plugin solicitará uma justificativa para ser utilizada no aprendizado do LLM.


---

**3) Requisito Não Funcional (NFR):**


O sistema solicita que o usuário selecione ou justifique o **Requisito Não Funcional** relacionado à hipótese. Exemplos incluem:

- Desempenho
- Segurança
- Confiabilidade
- Flexibilidade
- Usabilidade
- Produtividade

![NFR](img/image-5.png)

⚠️**Atenção:** Ao retornar a uma etapa anterior, os valores sugeridos pelo LLM podem ser perdidos e precisarão ser reeditados.

⚠️**Atenção:** O usuário pode editar qualquer informação sugerido pelo LLM porém o ArchHypo.AI Plugin solicitará uma justificativa para ser utilizada no aprendizado do LLM.


---

**4)Avaliação da Incerteza:**

Nesta etapa, o usuário deve classificar o **nível de incerteza** associado à hipótese. Os níveis disponíveis são:

- Muito Alto
- Alto  
- Médio  
- Baixo
- Muito Baixo

  ![Incerteza](img/image-6.png)

Essa classificação representa o grau de desconhecimento ou risco técnico envolvido.

⚠️**Atenção:** Ao retornar a uma etapa anterior, os valores sugeridos pelo LLM podem ser perdidos e precisarão ser reeditados.

⚠️**Atenção:** O usuário pode editar qualquer informação sugerido pelo LLM porém o ArchHypo.AI Plugin solicitará uma justificativa para ser utilizada no aprendizado do LLM.

---

**5)Avaliação do Impacto:**

O sistema também solicita que o usuário avalie o **impacto potencial** da hipótese na arquitetura do sistema. Os níveis disponíveis são:

- Muito Alto
- Alto  
- Médio  
- Baixo
- Muito Baixo
  
  ![Impacto](img/image-7.png)
  
O impacto deve ser avaliado com base em critérios como:

- Complexidade de implementação  
- Riscos para desempenho, segurança ou interoperabilidade  
- Dependência entre componentes

⚠️**Atenção:** Ao retornar a uma etapa anterior, os valores sugeridos pelo LLM podem ser perdidos e precisarão ser reeditados.

⚠️**Atenção:** O usuário pode editar qualquer informação sugerido pelo LLM porém o ArchHypo.AI Plugin solicitará uma justificativa para ser utilizada no aprendizado do LLM.


---

Após preencher todos os campos, o plugin cria automaticamente um **card no Trello** com as informações da incerteza e da hipótese.

![Card Criado](img/image-8.png)

---

#### 🏷️ Add/Atualizar Métricas  

Para adicionar ou atualizar as métricas nos cards do Trello, o usuário deve acessar o card de Hipótese ou o Item do Plano Técnico e utilizar o botão conforme ilustrado abaixo:

![Botao Power UP](img/image-9.png)

Em seguida, clique em "Add/Atualizar Métricas" para incluir ou modificar os labels correspondentes:

![Add/Atualizar Métrica](img/image-10.png)

As métricas adicionadas variam conforme o tipo de card:

- Hipóteses → *Nível de Incerteza, Impacto e Requisito Não Funcional*
- Itens do Plano Técnico → *Padrões ArchHypo*

Após a ação, os labels serão exibidos conforme o exemplo:

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

Utilize o recurso *ArchHypo Métricas* para acompanhar a quantidade de cards classificados conforme descrito na seção Adicionar ou Atualizar Métricas.

Para acessar, clique no botão indicado na imagem abaixo:

![Botao Métricas](img/image-18.png)

O painel apresenta diferentes tipos de gráficos, como:

- Quantidade de hipóteses com Nível de Incerteza e Impacto
- Quantidade de hipóteses com Requisitos Não Funcionais (NFR)
- Quantidade de itens do plano técnico com o [Padrões ArchHypo](README-padroes.md)

  
![Métricas](img/image-19.png)


--------------------------------------------------------------------------------------------------------------------

ArchHypo.AI Plugin

Equipe de Pesquisa e Desenvolvimento

[https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)


