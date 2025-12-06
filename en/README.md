# ArchHypo Trello Plugin Experiment
📝 INFORMED CONSENT FORM

You are invited to participate in a study aimed at exploring the use of LLMs (Large Language Models) to support architectural decisions in software projects, through the management of hypotheses and technical plans directly in Trello.

## Participation

This experiment is divided into stages. You will be required to perform specific tasks using the ArchHypo.AI plugin available in Trello.
After completing the tasks, keep the data on the Trello board as the Plugin will be evaluated later.
Detailed instructions for each stage are described in the following sections.

## Confidentiality and Anonymity
All information collected during this study will be kept strictly confidential.
Any data disclosed in scientific events or publications will be used exclusively for academic purposes, without any identification of participants, except among the researchers directly involved, ensuring complete privacy.

## Contact
During the study, you may ask questions or request clarifications at any time via email: [jonathan.carvalho@unifesp.br](mailto:jonathan.carvalho@unifesp.br).

## Voluntary Participation
Participation in this study is entirely voluntary. You may refuse or withdraw from the experiment at any time without any penalty or negative consequences.
The experiment may also have educational purposes in development contexts, and sharing data for research purposes is optional.

## Data Retention
All collected data will be securely stored for a period of 2 years after the project completion.

## Consent Registration
As the questionnaire will be completed through an online form, you must indicate your agreement by selecting the appropriate option.
A signed copy of this document by the research team can be provided upon request.

### A) Prerequisites
To participate in the experiment, it is recommended:

- Active Trello account.
- Familiarity with software architecture concepts and non-functional requirements.
- Interest in performing and learning during the experiment, based on the following support materials:
   - [ArchHypo Patterns](README-patterns.md): It is recommended to read the introductory document about the patterns used.
   - [User Guide](README-tutorial.md) of the ArchHypo.AI Plugin: reference material that can be consulted throughout the experiment.

### B) Setup

The experiment will be conducted directly in Trello using the ArchHypo.AI plugin.
No additional software installation is required.

#### Environment
- Updated browser (Chrome, Firefox, Edge, etc.)
- Internet access
- Trello account

### C) Context
Architectural decisions in software projects involve uncertainties that directly impact non-functional requirements. ArchHypo.AI proposes an LLM-assisted approach to:

- Identify hypotheses from recorded uncertainties
- Suggest technical plans and architectural patterns
- Categorize and visualize impact and uncertainty metrics
- This experiment evaluates how the use of LLMs can support architectural decision-making, promoting traceability and organization directly in Trello boards.

### D) Training – ArchHypo.AI

Before starting your participation in the experiment, it is recommended to undergo introductory training on using the ArchHypo AI tool.
To do this, follow the step-by-step instructions described in the [User Guide](README-tutorial.md), which presents the plugin's features and practical guidance for its use in Trello.

During training, participants should perform the following activities:

1) **Access the link corresponding to the designated group**, as listed below:
   - Group 1: [link](https://trello.com/invite/b/693462ed57177c7a77e7bd22/ATTI60533275a87bed686f2759dbf6813972321A2425/archhypo-v020-group-1)
   - Group 2: [link](https://trello.com/invite/b/69346306d493d4db06a60c25/ATTIe5a6c8b2de33130d63f789434e96e5a00230882A/archhypo-v020-group-2)
   - Group 3: [link](https://trello.com/invite/b/69346316e3f97f4d8777ce7f/ATTI47a47b7a21fc96fbf56c70afd53d4f080D273054/archhypo-v020-group-3)
   - Group 4: [link](https://trello.com/invite/b/693463283c2d644ee9ff0678/ATTIbd0c03915309d53550d6d59ae372205dDBC4E09E/archhypo-v020-group-4)
   - Group 5: [link](https://trello.com/invite/b/69346337829bfce748fdff67/ATTI6562eefcb7d023816148d7129f47d4d7F1E7AF10/archhypo-v020-group-5)
   - Group 6: [link](https://trello.com/invite/b/693463547df100065d0f2e3d/ATTI466d851c723fe37da3c99cb6673417442836BECD/archhypo-v020-group-6)
   - Group 7: [link](https://trello.com/invite/b/693463441f7152da293f1ded/ATTIaccda511893ad8933f58f1b593b284296D2AB2C8/archhypo-v020-group-7)

2) Register an uncertainty in the system and observe:

    - **The hypothesis automatically generated** by the language model (LLM)
    - **The automatic classification suggestions** for the generated hypothesis.
    - **The justifications provided** for each classification assigned to the hypothesis.

3) **Add metrics to hypotheses and technical items**, using _labels_ for proper categorization.
4) **Generate a technical plan** based on the registered hypothesis.
5) **Classify the technical plan items** according to the [ArchHypo Patterns](README-patterns.md).
6) **Visualize the metrics** through the charts available in the plugin.

### E) Experiment Tasks

The main objective of the experiment is to use the ArchHypo.AI plugin to identify architectural uncertainties present in the email below and, from them, develop technical hypotheses in Trello, accompanied by validation technical plans.

#### Steps:

**1) Access the link corresponding to the previously designated group, as listed in the [Training - ArchHypo.AI](#d-training--archhypoai) section.**

**2) Identify the Uncertainties:**

This step consists of carefully reading the provided email. From this reading, the participant should identify **three architectural uncertainties** present in the content.

These uncertainties represent doubts, gaps, or undefined aspects that may impact technical decisions in the project. They will serve as the basis for creating technical hypotheses in the following steps.

💡 Tip:
Look for parts of the email that indicate lack of clarity, pending decisions, vague requirements, or technical concerns. These elements usually point to uncertainties that need to be explored and validated.


> **From:** equipe@sistema.com.br  
> **To:** desenvolvimento@sistema.com.br  
> **Subject:** Questions about system features and architecture  
> 
> Hello Development Team,
> 
> As we progress through the development stages of the document management system for public
> agencies — whose main function is to organize, store, and digitally provide administrative and 
> legal documents — some technical observations have emerged that we would like to share for 
> alignment.
> 
> The project is being conducted in partnership with the client, who has been providing 
> operational data and functional and non-functional requirements over the past few weeks.
> 
> During recent meetings, we discussed the storage structure and data flow, especially 
> considering the projected volumes for this year. The system must handle different data formats, 
> including legacy XML files and recent JSON documents. The client expressed interest in 
> preserving historical data in its original format, which may impact how the reading and 
> persistence components are structured. This coexistence of formats may require special 
> attention in how we structure the reading and storage components.
> 
> The development team has been using operational records from the previous cycle as a basis to 
> estimate system behavior, especially regarding the volume of processed documents. Although this 
> data provides a good initial reference, the client projects a considerable increase in load for 
> this year, which may significantly change usage patterns during peak hours. In some internal 
> simulations, we observed that document batches could reach volumes close to 1GB per minute, 
> prompting us to review the current infrastructure strategy, still centered on a single server, 
> to assess whether it will be sufficient to meet new demands.
> 
> Another point that arose is the need for integration with the authentication system used by 
> government platforms, which operate with Single Sign-On. Since we are using a cross-platform 
> framework, it is important to verify whether the current components offer adequate support or 
> if some adaptation will be necessary to ensure compliance with the required protocols.
> 
> We remain available to discuss these points in more depth and evaluate possible technical 
> approaches.
> 
> Best Regards,  
> Product Manager

---

## 3) Creating Hypotheses in Trello with ArchHypo.AI

In this step, the participant must use ArchHypo.AI in Trello to transform the identified uncertainties into technical hypotheses. Each hypothesis will be recorded as a card in Trello, filling in the following fields:

- **Hypothesis Title:** a short sentence summarizing the hypothesis following the pattern: _(H1: Hypothesis Title)_.
- **Uncertainty Description:** briefly explain what is uncertain or unknown.
- **Non-Functional Requirement:** select the type of requirement related to the hypothesis _(Performance, Security, Reliability, Flexibility, Usability, or Productivity)_.
- **Uncertainty Level:** indicate the degree of uncertainty _(Very Low, Low, Medium, High, or Very High)_.
- **Impact Level:** indicate the potential impact of the hypothesis on the system _(Very Low, Low, Medium, High, or Very High)_.

💡 **Expected Result**

At the end of this step, the Trello board should contain three hypothesis cards, filled out according to the fields above:

_H1: [Title of the first hypothesis]_  
_H2: [Title of the second hypothesis]_  
_H3: [Title of the third hypothesis]_

---

## 4) Generate Technical Plan

For each recorded hypothesis, the participant must use ArchHypo.AI to create items for a Technical Plan. Each item must contain the following fields:

- **Technical Plan Item Title:** a sentence describing the technical action related to the hypothesis following the pattern: _(H1 - TP1: Technical Plan Item Title)_.
- **Objective:** describe the purpose of the technical action.
- **Description:** provide details about what will be done.
- **ArchHypo Pattern:** classify the item using the [ArchHypo Patterns](README-patterns.md).
- **Tradeoff:** describe possible advantages and disadvantages of the proposed action.

💡 **Expected Result**

At the end of this step, the Trello board should contain at least three Technical Plan Item cards for each hypothesis:

_H1 – TP1: [Item 1 related to hypothesis H1]_  
_H1 – TP2: [Item 2 related to hypothesis H1]_  
_H1 – TP3: [Item 3 related to hypothesis H1]_

---

_H2 – TP1: [Item 1 related to hypothesis H2]_  
_H2 – TP2: [Item 2 related to hypothesis H2]_  
_H2 – TP3: [Item 3 related to hypothesis H2]_

---

_H3 – TP1: [Item 1 related to hypothesis H3]_  
_H3 – TP2: [Item 2 related to hypothesis H3]_  
_H3 – TP3: [Item 3 related to hypothesis H3]_

Note: All cards must be categorized with labels/metrics, as instructed in the [Training - ArchHypo.AI](#d-training--archhypoai) section.

---

## F) Finalization

Thank you for participating in the ArchHypo Plugin test for Trello!

This experiment aims to:

- Evaluate the usability and effectiveness of the ArchHypo Plugin  
- Identify and disable non-essential features  
- Propose functional and technical improvements to the plugin  
- Contribute to a more efficient and sustainable software development process

📋 After completing the tasks, please fill out the form available at: [Form Link](https://forms.gle/GHojjXuqTKVVCwjp8)

Your feedback is essential for improving the ArchHypo Plugin and promoting smarter and more sustainable practices in software engineering.

Thank you very much for your collaboration!

---

ArchHypo.AI Plugin  

Developed by the Research and Development Team  

[🔗 GitHub Repository](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)
