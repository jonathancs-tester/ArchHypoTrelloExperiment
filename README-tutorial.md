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
   - 💡 O LLM sugere hipótese + motivo (você pode editar).
  
     Ao registrar uma **Incerteza**, o LLM sugere uma **Hipótese** e sua classificação (pode ser ajustada pelo usuário).

![Nova Incerteza](img/image-2.png)

![Nova Inceteza 2](img/image-3.png)

![Hipotese](img/image-4.png)

![NFR](img/image-5.png)

![Incerteza](img/image-6.png)

![Impacto](img/image-7.png)

![Card Criado](img/image-8.png)
  
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


