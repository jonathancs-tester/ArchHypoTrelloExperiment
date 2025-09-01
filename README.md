# ArchHypo Trello Plugin Experiment
📝 TERMO DE CONSENTIMENTO INFORMADO

Você está convidado a participar de um estudo que visa explorar o uso de LLMs (Modelos de Linguagem de Grande Escala) para apoiar decisões arquiteturais em projetos de software, por meio da gestão de hipóteses e planos técnicos diretamente no Trello.

## Participação

Este experimento está dividido em etapas. Você deverá realizar tarefas específicas utilizando o plugin ArchHypo.AI disponível no Trello.
Após concluir as tarefas, manter os dados no quadro do Trello pois será feita uma avaliação do Plugin posterirmente.
As instruções detalhadas para cada etapa estão descritas nas seções seguintes.

## Confidencialidade e Anonimato
Todas as informações coletadas durante este estudo serão mantidas em sigilo absoluto. 
Os dados eventualmente divulgados em eventos científicos ou publicações serão utilizados exclusivamente para fins acadêmicos, sem qualquer identificação dos participantes, exceto entre os pesquisadores diretamente envolvidos, garantindo total privacidade.

## Contato
Durante o estudo, você pode tirar dúvidas ou solicitar esclarecimentos a qualquer momento pelo e-mail: [jonathan.carvalho@unifesp.br](jonathan.carvalho@unifesp.br).

## Participação Voluntária
A participação neste estudo é totalmente voluntária. Você pode recusar ou desistir do experimento a qualquer momento, sem qualquer penalidade ou consequência negativa.
O experimento também pode ter fins educacionais em contextos de desenvolvimento, sendo opcional o compartilhamento dos dados para fins de pesquisa.

## Retenção de Dados
Todos os dados coletados serão armazenados de forma segura por um período de 2 anos após a conclusão do projeto.

## Registro de Consentimento
Como o questionário será preenchido por meio de um formulário online, você deverá indicar sua concordância selecionando a opção apropriada. 
Uma cópia assinada deste documento pela equipe de pesquisa pode ser fornecida mediante solicitação.

### A) Pré-requisitos
Para participar do experimento, recomenda-se:

- Conhecimento básico sobre Trello e uso de Power-Ups.
- Familiaridade com conceitos de arquitetura de software e requisitos não funcionais.
- Conta ativa no Trello.

### B) Configuração
O experimento será realizado diretamente no Trello, utilizando o plugin ArchHypo.AI. Não é necessário instalar software adicional além do Power-Up.

#### Ambiente
- Navegador atualizado (Chrome, Firefox, Edge, etc.)
- Acesso à internet
- Conta no Trello com permissão para adicionar Power-Ups

### C) Contexto
Decisões arquiteturais em projetos de software envolvem incertezas que impactam diretamente requisitos não funcionais. O ArchHypo.AI propõe uma abordagem assistida por LLMs para:

- Identificar hipóteses a partir de incertezas registradas
- Sugerir planos técnicos e padrões arquiteturais
- Categorizar e visualizar métricas de impacto e incerteza
- Este experimento avalia como o uso de LLMs pode apoiar a tomada de decisão arquitetural, promovendo rastreabilidade e organização diretamente em boards Trello.

### D) Visão Geral do Experimento
Você deverá realizar as seguintes etapas:

1) Criar um Board Template com as colunas recomendadas:
   - INCERTEZA
   - ITEM PLANO TÉCNICO
   - A FAZER
   - EM ANDAMENTO
   - CONCLUÍDO
2) Registrar uma Incerteza e observar a sugestão automática de hipótese e classificação.
3) Adicionar Métricas usando labels para categorizar hipóteses e itens técnicos.
4) Gerar Plano Técnico com base na hipótese registrada.
5) Visualizar Métricas por meio dos gráficos disponíveis no plugin.

### E) 🚀 Como usar (passo a passo)

1. 🗂️ **Criar Board Template** → Clique em *"Criar um Board Template"* para começar.

Adicione as colunas obrigatórias necessárias (ex: INCERTEZA, ITEM PLANO TECNICO, A FAZER, EM ANDAMENTO CONCLUIDO) para utilizar a gestão de hipóteses e decisões arquiteturais .

![Add Board Template](img/image-1.png)

![Board Template](img/image.png)

Lembrando que você pode criar outras colunas personalizadas.

2. ❓ **Criar Incerteza** → Clique em *"Criar uma Incerteza"* e preencha as informações.  
   - 💡 O LLM sugere hipótese + motivo (você pode editar).
  
     Ao registrar uma **Incerteza**, o LLM sugere uma **Hipótese** e sua classificação (pode ser ajustada pelo usuário).

![Nova Incerteza](img/image-2.png)

![Nova Inceteza 2](img/image-3.png)

![Hipotese](img/image-4.png)

![NFR](img/image-5.png)

![Incerteza](img/image-6.png)

![Impacto](img/image-7.png)

![Card Criado](img/image-8.png)
  
3. 🏷️ **Adicionar Métricas** → Clique em *"Add/Atualizar Métricas"* para configurar os labels.
  - Hipóteses → *Nível de Incerteza, Impacto e Requisito Não Funcional*  
  - Itens do Plano Técnico → *Padrões ArchHypo*  

![Botao Power UP](img/image-9.png)

![Add/Atualizar Métrica](img/image-10.png)

![Metricas Adicionado](img/image-11.png)

4. 📋 **Gerar Plano Técnico**  
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


5.📋 **Gerenciar Itens do Plano Técnico**  
   - Os itens são adicionados na coluna **ITEMS PLANO TÉCNICO**, com IDs no formato:  
     - `H1` → Hipótese 1  
     - `TPI1` → Tech Plan Item 1

   ![Plano Board](img/image-17.png)
   
6. 📊 **Visualizar Métricas** → Use *ArchHypo Métricas* para acompanhar evolução em gráficos e gerenciar as métricas e labels de categorização de Hipóteses e Itens de Plano Técnico.

![Botao Métricas](img/image-18.png)

![Métricas](img/image-19.png)

### F) Finalização

Agradecemos sua participação no teste do ArchHypo Plugin para Trello!

Este experimento tem como objetivo avaliar como ajustes simples no código — como a desativação de recursos não essenciais — podem contribuir para uma execução mais eficiente, sem comprometer a funcionalidade principal do plugin.

📋 Após concluir as tarefas, preencha o formulário disponível em: [Link do Formulário](https://forms.gle/SzHdND58MWyCouZr8)

Seu retorno é fundamental para evoluirmos o ArchHypo e promovermos práticas mais sustentáveis no desenvolvimento de software.

--------------------------------------------------------------------------------------------------------------------

ArchHypo.AI Plugin

Equipe de Pesquisa e Desenvolvimento

[https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)


