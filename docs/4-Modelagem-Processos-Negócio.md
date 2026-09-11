# 4. Modelagem dos Processos de Negócio
O Gerenciamento de Processos de Negócio (BPM) não se restringe a uma ação pontual, mas constitui um ciclo contínuo de melhoria e eficiência. Deste modo, o presente trabalho abrange as etapas de **diagnóstico e arquitetura** (Seção 2) e o **redesenho da situação futura (TO-BE)** deste capítulo, estruturando a base necessária para a posterior **implementação do produto de software** nas próximas fases da disciplina.

---

## 4.1. Diagnóstico da Situação Atual (Modelo AS-IS Descritivo)
*(Conforme alinhado com a disciplina, o modelo AS-IS não precisa ser desenhado em BPMN. Apenas descreva textualmente como o processo funciona hoje).*


> ✏️ **[Atenção aluno: Apague este bloco e descreva o processo AS-IS]**
> 
> *Explique o passo a passo de como a atividade é realizada atualmente (ex: uso de papel, planilhas isoladas, trocas manuais de e-mails) eponha claramente os gargalos, a lentidão, os erros e os desperdícios que justificam a criação do novo sistema.*

---

## 4.2. A Solução Proposta e Elementos da Notação BPMN (Modelo TO-BE)
O modelo **TO-BE** representa o processo redesenhado, otimizado e focado na eficiência tecnológica. Para representá-lo graficamente, utilizamos a notação BPMN aplicando os seguintes elementos:
* **Raias (Pools e Swimlanes):** Delimitam claramente os papéis e responsabilidades de cada ator (ex: Atendente vs. Sistema vs. Gestor).
* **Tarefas (Activities):** As ações executadas no fluxo (destacando aquelas que serão automatizadas pela aplicação).
* **Portas Lógicas (Gateways):** Representam as tomadas de decisão e os desvios condicionais do processo (ex: "Se o cadastro for aprovado, segue para a etapa X; caso contrário, retorna").
* **Objetos de Dados (Data Objects):** Indicam os documentos, formulários ou informações que entram e saem durante a execução das tarefas.

---

## 4.3. Diagrama do Processo TO-BE dos Processos Propostos (Cenário Real)
Nesta seção, vocês deverão elaborar o fluxograma TO-BE na ferramenta BPMN — separando-o por Processo 1, Processo 2, etc. — e inserir a imagem do modelo correspondente.
Apresente uma breve descrição explicativa sobre o que o processo modelado representa. Dica: Os quadros e o detalhamento das atividades representados nestes fluxos serão extremamente úteis para a estruturação das tabelas de banco de dados e dos requisitos nas próximas etapas do Projeto da Solução.


### Processo 1 — [Nome do Processo, ex: Gerenciar Veículos / Solicitar Atendimento]

> ✏️ **[Atenção aluno: Insira a imagem do fluxograma BPMN TO-BE deste processo específico abaixo]**
> 
> `![Diagrama TO-BE do Processo 1](../images/processo-1-to-be.png)`

**Descrição e Oportunidades de Melhoria:**
> ✏️ **[Atenção aluno: Apague este bloco e redija o texto explicativo do processo, seguindo o modelo abaixo]**
> 
> *Exemplo:* "Processo utilizado para **[descrever a finalidade do processo]** de forma automatizada, no qual os atores podem **[citar ações como consultar dados, alterar status e inserir registros]** em um sistema integrado, reduzindo o tempo gasto para a realização dessas tarefas e eliminando a necessidade de lidar com papéis e planilhas desconectadas para manter essas informações."


**Nome da atividade 1**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| [Nome do campo] | [tipo de dados]  |                |                   |
| ***Exemplo:***  |                  |                |                   |
| login           | Caixa de Texto   | formato de e-mail |                |
| senha           | Caixa de Texto   | mínimo de 8 caracteres |           |

| **Comandos**         |  **Destino**                   | **Tipo** |
| ---                  | ---                            | ---               |
| [Nome do botão/link] | Atividade/processo de destino  | (default/cancel/  ) |
| ***Exemplo:***       |                                |                   |
| entrar               | Fim do Processo 1              | default           |
| cadastrar            | Início do proceso de cadastro  |                   |


**Nome da atividade 2**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| [Nome do campo] | [tipo de dados]  |                |                   |
|                 |                  |                |                   |

| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| [Nome do botão/link] | Atividade/processo de destino  | (default/cancel/  ) |
|                      |                                |                   |
---

### Processo 2 — [Nome do Segundo Processo, se houver]

> ✏️ **[Atenção aluno: Insira a imagem do fluxograma BPMN TO-BE deste segundo processo abaixo]**
> 
> `![Diagrama TO-BE do Processo 2](../images/processo-2-to-be.png)`

**Descrição e Oportunidades de Melhoria:**
> ✏️ **[Atenção aluno: Apague este bloco e redija o texto explicativo do segundo processo]**
> 
> *Descreva aqui como este segundo fluxo opera de forma otimizada com o uso do sistema.*

_Apresente aqui uma descrição da sua proposta abordando seus limites e suas ligações com as estratégias e objetivos do negócio. Apresente aqui as oportunidades de melhorias._

**Nome da atividade 1**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| [Nome do campo] | [tipo de dados]  |                |                   |
| ***Exemplo:***  |                  |                |                   |
| login           | Caixa de Texto   | formato de e-mail |                |
| senha           | Caixa de Texto   | mínimo de 8 caracteres |           |

| **Comandos**         |  **Destino**                   | **Tipo** |
| ---                  | ---                            | ---               |
| [Nome do botão/link] | Atividade/processo de destino  | (default/cancel/  ) |
| ***Exemplo:***       |                                |                   |
| entrar               | Fim do Processo 1              | default           |
| cadastrar            | Início do proceso de cadastro  |                   |


**Nome da atividade 2**

| **Campo**       | **Tipo**         | **Restrições** | **Valor default** |
| ---             | ---              | ---            | ---               |
| [Nome do campo] | [tipo de dados]  |                |                   |
|                 |                  |                |                   |

| **Comandos**         |  **Destino**                   | **Tipo**          |
| ---                  | ---                            | ---               |
| [Nome do botão/link] | Atividade/processo de destino  | (default/cancel/  ) |
|                      |                                |                   |



### Exemplos anteriores

[PROCESSO 1 - Nome do Processo](./processos/processo-1-nome-do-processo.md "Detalhamento do Processo 1.")

[PROCESSO 2 - Nome do Processo](./processos/processo-2-nome-do-processo.md "Detalhamento do Processo 2.")
