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
- Conhecimento sobre o [Guia do Usuário](README-tutorial.md) do ArchHypo Trello Plugin.
- Conhecimento sobre os [Padrões ArchHypo](README-padroes.md).

### B) Configuração
O experimento será realizado diretamente no Trello, utilizando o plugin ArchHypo.AI. 
Não é necessário instalar software adicional.

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

1) Criar um Board Template com as colunas recomendadas, confura no item 1 do [Como usar (passo a passo)](#e--como-usar-passo-a-passo):
   - INCERTEZA
   - ITEM PLANO TÉCNICO
   - A FAZER
   - EM ANDAMENTO
   - CONCLUÍDO
2) Registrar uma Incerteza e observar a sugestão automática de hipótese e classificação.
3) Adicionar Métricas usando labels para categorizar hipóteses e itens técnicos.
4) Gerar Plano Técnico com base na hipótese registrada.
5) Visualizar Métricas por meio dos gráficos disponíveis no plugin.

### E) Exemplo de Uso 

Utilizar o plugin para identificar incertezas arquiteturais no email e criar hipóteses técnicas no Trello, com planos de validação.

Passos:
1) Leitura do Email
   O participante deve ler o email abaixo e identificar as incertezas.

> **De:** equipe@sistema.com.br
> 
> **Para:** desenvolvimento@sistema.com.br
> 
> **Assunto:** Dúvidas sobre funcionalidades e arquitetura do sistema  
>  
> Olá equipe,  
>  
> Estamos avançando com o desenvolvimento do sistema e surgiram algumas dúvidas importantes que precisamos esclarecer tecnicamente.  
>  
> Uma das preocupações é se conseguiremos processar lotes de 1GB por minuto utilizando apenas um servidor.
> Isso pode impactar diretamente a arquitetura, pois talvez seja necessário distribuir a aplicação.
>Estamos usando os dados do ano anterior como referência e projetando para este ano com apoio do cliente. 
>  
> Outra questão é se os componentes que estamos utilizando são compatíveis com o protocolo de autenticação Single Sign-On do governo.
> A plataforma GeneXus oferece integração com alguns protocolos, mas ainda não temos certeza se o protocolo específico do governo é compatível.
>
> Por fim, precisamos garantir que o sistema seja compatível com o formato de dados antigo e o novo.
> O cliente quer manter os dados históricos no formato original, sem migração.
> Ainda não sabemos qual seria a melhor forma de fazer isso dentro da GeneXus  
>  
> Atenciosamente,
> 
> Equipe de Desenvolvimento 


2) Criação de Hipóteses no Trello com ArchHypo Plugin
   Para cada incerteza, o participante deve usar o plugin para criar uma hipótese com os seguintes campos:

- Título da Hipótese (ex: H1. Processamento de 1GB/min com 1 servidor)
- Descrição da Incerteza
- Requisito Não Funcional (Performance, Segurança, Flexibilidade e etc)
- Nível de Incerteza (Alto)
- Nivel de Impacto (Alto)

Gerenciamento no Trello
O plugin deve criar os cartões no board configurado, com etiquetas correspondentes às categorias e campos preenchidos conforme o plano técnico.

3) Gerar Plano Técnico:
   Para cada hipótese, o participande deve gerar um Itens de um Plano Técnico com os seguintes campos:

- Título da Item do Plano Tenico (ex: H1 - TPI 1. Analisar o esquema do banco de dados)
- Objetivo
- Descrição
- Padrão ArchHypo (Paln for Preparation)
- Tradeoff

💡 Resultado Esperado
Após o uso do plugin, o board do Trello deve conter:

- **3 cartões de hipóteses:**
    - H1: 
    - H2: 
    - H3: 

- **Pelo menos 3 cartões de Itens do Plano Técnico:**
    - H1 - TP1: 
    - H2 - TP1: 
    - H3 - TP1: 

**Obs: Todos os cards devem ser categorizados pelas labels/métricas.**

### F) Finalização

Agradecemos sua participação no teste do ArchHypo Plugin para Trello!

Este experimento tem como propósito:

 - Avaliar a usabilidade e eficácia do ArchHypo Plugin
 - Identificar e desativar recursos não essenciais
 - Propor melhorias funcionais e técnicas no plugin
 - Contribuir para uma execução mais eficiente e sustentável no desenvolvimento de software

📋 Após concluir as tarefas, preencha o formulário disponível em: [Link do Formulário](https://forms.gle/SzHdND58MWyCouZr8)

Seu retorno é essencial para evoluirmos o ArchHypo Plugin e promovermos práticas mais inteligentes e sustentáveis na engenharia de software.

Muito obrigado pela sua colaboração!

--------------------------------------------------------------------------------------------------------------------

ArchHypo.AI Plugin

Equipe de Pesquisa e Desenvolvimento

[https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)


