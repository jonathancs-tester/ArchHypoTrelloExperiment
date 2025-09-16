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

- Conta ativa no Trello.
- Familiaridade com conceitos de arquitetura de software e requisitos não funcionais.
- Interesse em realizar leitura e aprendizado durante o experimento, com base nos seguintes materiais de apoio:
   - Padrões ArchHypo: documento introdutório sobre os padrões utilizados. Recomenda-se a leitura introdutória disponível em: [Padrões ArchHypo](README-padroes.md).
   - [Guia do Usuário](README-tutorial.md) do ArchHypo Trello Plugin: material de referência que poderá ser consultado ao longo do experimento.

### B) Configuração

O experimento será realizado diretamente no Trello, utilizando o plugin ArchHypo.AI. 
Não é necessário instalar software adicional.

#### Ambiente
- Navegador atualizado (Chrome, Firefox, Edge, etc.)
- Acesso à internet
- Conta no Trello

### C) Contexto
Decisões arquiteturais em projetos de software envolvem incertezas que impactam diretamente requisitos não funcionais. O ArchHypo.AI propõe uma abordagem assistida por LLMs para:

- Identificar hipóteses a partir de incertezas registradas
- Sugerir planos técnicos e padrões arquiteturais
- Categorizar e visualizar métricas de impacto e incerteza
- Este experimento avalia como o uso de LLMs pode apoiar a tomada de decisão arquitetural, promovendo rastreabilidade e organização diretamente em boards Trello.

### D) Treinamento – ArchHypo.AI

Antes de iniciar sua participação no experimento, recomenda-se a realização de um treinamento introdutório sobre o uso da ferramenta ArchHypo AI. 
Para isso, siga o passo a passo descrito no [Guia do Usuário](README-tutorial.md), que apresenta as funcionalidades do plugin e orientações práticas para sua utilização no Trello. 

Durante o treinamento, os(as) participantes deverão realizar as seguintes atividades:

1) Acesse o link correspondente ao grupo selecionado no seguinte endereço:
   - Grupo 1: https://trello.com/b/sEjDHKsg/archhypo-grupo-1
   - Grupo 2: https://trello.com/b/ERv4woXX/archhypo-grupo-2
   - Grupo 3: https://trello.com/b/4Pml3c4v/archhypo-grupo-3
   - Grupo 4: https://trello.com/b/AwkCCm1Q/archhypo-grupo-4
   - Grupo 5: https://trello.com/b/9hxIsJep/archhypo-grupo-5
   - Grupo 6: https://trello.com/b/ldgHNjDR/archhypo-grupo-6
   - Grupo 7: https://trello.com/b/82bNxSjT/archhypo-grupo-7
2) Registrar uma incerteza e observar a sugestão automática de hipótese e sua respectiva classificação.
3) Adicionar métricas utilizando labels para categorizar hipóteses e itens técnicos.
4) Gerar um plano técnico com base na hipótese registrada.
5) Classificar os itens do plano técnico utilizando os [Padrões ArchHypo](README-padroes.md).
6) Visualizar métricas por meio dos gráficos disponíveis no plugin.

### E) Tarefas do Experimento

O objetivo principal do experimento é utilizar o plugin ArchHypo.AI para identificar incertezas arquiteturais presentes no e-mail e, a partir delas, elaborar hipóteses técnicas no Trello, acompanhadas de planos técnicos de validação.

Passos:

1) Acesse o link correspondente ao grupo previamente designado, conforme listado na seção de [Treinamento - ArchHypo.AI](#d-treinamento--archhypoai).

2) Leitura do Email
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

3) Identifique as Incertezas

Com base no conteúdo do e-mail fornecido anteriormente, o(a) participante deverá identificar **três incertezas** arquiteturais. Essas incertezas representam aspectos do sistema que ainda não estão totalmente definidos, compreendidos ou validados, e que podem impactar decisões técnicas futuras.

💡 O que é uma incerteza arquitetural?

É uma dúvida ou lacuna de conhecimento relacionada à arquitetura do sistema, como desempenho esperado, segurança, escalabilidade, integração entre componentes, entre outros.

4) Criação de Hipóteses no Trello com o Plugin ArchHypo
   
Nesta etapa, o(a) participante deverá utilizar o ArchHypo.AI no Trello para transformar as incertezas identificadas em hipóteses técnicas. Cada hipótese será registrada como um cartão no Trello, preenchendo os seguintes campos:

- **Título da Hipótese:** uma frase curta que resume a hipótese _(exemplo: H1: Processamento de 1GB/min com 1 servidor)_.
- **Descrição da Incerteza:** explique brevemente o que está incerto ou desconhecido.
- **Requisito Não Funcional:** selecione o tipo de requisito relacionado à hipótese _(ex: Desempenho, Segurança, Confiabilidade, Flexibilidade, Usabilidade ou Produtividade)_.
- **Nível de Incerteza:** indique o grau de incerteza _(ex: Muito Baixo, Baixo, Médio, Alto ou Muito Alto)_.
- **Nível de Impacto:** indique o impacto potencial da hipótese no sistema _(ex: Muito Baixo, Baixo, Médio, Alto ou Muito Alto)_.

  
💡 Resultado Esperado

Ao final desta etapa, o quadro do Trello deve conter três cartões de hipóteses, preenchidos conforme os campos acima:

H1: [Título e informações da primeira hipótese]

H2: [Título e informações da segunda hipótese]

H3: [Título e informações da terceira hipótese]


5) Gerar Plano Técnico

Para cada hipótese registrada, o(a) participante deverá utilizar o ArchHypo.AI para criar itens de um Plano Técnico. Cada item deve conter os seguintes campos:

- **Título do Item do Plano Técnico:** uma frase que descreve a ação técnica relacionada à hipótese _(ex: H1 – TP1: Analisar o esquema do banco de dados)_.
- **Objetivo:** descrever o propósito da ação técnica.
- **Descrição:** descrever detalhes sobre o que será feito.
- **Padrão ArchHypo:** classificar o item utilizando os [Padrões ArchHypo](README-padroes.md).
- **Tradeoff:** descrever possíveis vantagens e desvantagens da ação proposta.

💡 Resultado Esperado

Ao final desta etapa, o quadro do Trello deve conter pelo menos três cartões de Itens do Plano Técnico para cada hipótese:

H1 – TP1: [Item relacionado à hipótese H1]
H1 – TP2: [Item relacionado à hipótese H1]
H1 – TP3: [Item relacionado à hipótese H1]

H2 – TP1: [Item relacionado à hipótese H2]
H2 – TP2: [Item relacionado à hipótese H2]
H2 – TP3: [Item relacionado à hipótese H2]

H3 – TP1: [Item relacionado à hipótese H3]
H3 – TP2: [Item relacionado à hipótese H3]
H3 – TP3: [Item relacionado à hipótese H3]

Obs.: Todos os cartões devem ser categorizados com labels/métricas, conforme orientações do [Treinamento - ArchHypo.AI](#d-treinamento--archhypoai).

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


