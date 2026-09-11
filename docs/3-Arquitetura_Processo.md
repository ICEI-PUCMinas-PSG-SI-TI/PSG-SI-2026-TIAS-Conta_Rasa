# 3. Contexto do Negócio e Arquitetura de Processos

Nesta etapa do trabalho, o objetivo é entender **o mundo real** antes de pensar em código ou telas de software. Aqui vocês vão documentar quem sofre com o problema atual, quais são as entradas e saídas do sistema de trabalho e como esse processo se encaixa na engrenagem da empresa.

---

## 3.1. Investigação e Fontes Ouvidas
Os problemas e gargalos do projeto **não podem ser inventados**. Eles precisam vir de conversas reais, observações ou cenários fundamentados.

* **O que preencher aqui:**
  * **Método:** Como vocês coletaram os dados? (Ex: Entrevista com gestores, observação do fluxo de atendimento, análise de planilhas antigas).
  * **Quem foi ouvido:** Cargos ou perfis consultados (Ex: *Gerente de Operações, Atendente de Portaria, Cliente final*).
  * **A grande dor descoberta:** Resuma em 1 ou 2 parágrafos o principal problema atual.
  * *Exemplo:* "Após conversar com a equipe de portaria, identificamos que o controle de visitantes é feito totalmente em papel. Isso gera filas na entrada, perda de dados de contato e dificulta a auditoria em caso de incidentes."

---

> ✏️ **[Atenção aluno: Apague este bloco e escreva o seu texto aqui]**
> 
> *Descreva neste espaço como a sua equipe realizou a investigação, quais fontes foram ouvidas e qual foi a principal dor de negócio descoberta no cenário real de vocês.*

---

## 3.2. Visão Geral do Processo (Entrada, Processo e Saída)
Antes de destrinchar a hierarquia, é importante entender os limites do processo mapeando o que entra (insumos, normas, recursos) e o que ele entrega como resultado (saída).

* **Exemplo prático baseado em processos reais:**
  * **Entrada:** Visitante, Normas de Segurança, Recursos Humanos e Materiais.
  * **Processo:** Controle de Acesso.
  * **Saída:** Visitante liberado, portando crachá de identificação e acompanhado conforme as normas.
    
  ![EXEMPLO de Ilustração de Processos da Gestão Patromonial](https://via.eng.br/wp-content/uploads/2021/09/entrada-processo-saida.jpg)
---

> ✏️ **[Atenção aluno: Apague este bloco e escreva o seu texto aqui ou desenhe o seu modelo de hierarquia conforme visto nas notas de aula e insira a imagem aqui]**
> 

---

## 3.3. Arquitetura de Processos (Do Macro à Tarefa)
Para o projeto não ficar perdido, utilizamos a hierarquia de processos. Pensem nisso como um "zoom" que vai do panorama geral até a menor atividade, estruturando a decomposição do negócio:

Preencham os níveis abaixo com base no tema do grupo (exemplo inspirado em fluxos de segurança patrimonial):

1. **Macroprocesso:** O grande segmento da organização. *(Ex: Segurança Patrimonial)*
2. **Processos:** As divisões funcionais principais. *(Ex: Controle de Acesso / Serviço de Inteligência)*
3. **Subprocessos:** Os conjuntos de atividades agrupadas. *(Ex: Serviços de Portaria / Central de Monitoramento)*
4. **Atividades:** A execução específica dentro do subprocesso. *(Ex: Identificação do Visitante)*
5. **Tarefas:** A ação operacional detalhada que compõe a atividade (que virará a caixinha no BPMN). *(Ex: Recepcionar, identificar, checar autorização, cadastrar e fornecer crachá).*

   ![EXEMPLO de Ilustração de Hieraquia dos Processos da Gestão Patromonial](https://via.eng.br/wp-content/uploads/2021/09/etapas-do-processo-de-seguranca-e1632243738770.jpg)
---

> ✏️ **[Atenção aluno: Apague este bloco e escreva o seu texto aqui ou desenhe o seu modelo de hierarquia conforme visto nas notas de aula e insira a imagem aqui]**
> 
---

## 3.3. Personas de Negócio e do Sistema

### O que é uma Persona?
Uma **persona** é um personagem semi-fictício, baseado em pesquisas e dados reais, que representa um participante do processo ou usuário do sistema. Ela deve refletir com exatidão a quantidade e os papéis reais existentes na organização estudada.

### Por que defini-la antes do desenvolvimento?
* **Foco no usuário:** Direciona o redesenho de fluxos e funções para resolver dores reais, eliminando achismos.
* **Otimização de recursos:** Evita o desperdício de tempo e esforço no desenvolvimento de funcionalidades desnecessárias.
* **Melhor experiência:** Facilita a criação de telas e interações mais simples e intuitivas.
* **Alinhamento da equipe:** Mantém todo o time ciente de quem realmente utilizará a solução.

---

### Os Dois Olhares da Disciplina
Para conectar o mundo de processos ao desenvolvimento de software, analisamos as personas sob duas perspectivas:

1. **Persona de Negócio:** O profissional que atua no dia a dia da empresa e sofre diretamente com os gargalos, lentidão e retrabalho do processo atual (*AS-IS*).
2. **Persona do Sistema:** O usuário final que vai interagir diretamente com as telas e funcionalidades da aplicação que vocês desenvolverão para apoiar o processo redesenhado (*TO-BE*).

---

### Exemplo de Preenchimento:

* **Persona 1: O Operacional / Solicitante**
  * **Nome e Perfil:** Carlos Eduardo, 34 anos — Porteiro / Atendente de Portaria.
  * **Papel na Organização:** Responsável pelo primeiro contato com visitantes e liberação manual de acessos.
  * **Dores no Processo Atual (AS-IS):** Perde muito tempo preenchendo fichas de papel, gerando filas na entrada e sofrendo com anotações ilegíveis.
  * **Expectativas no Sistema (TO-BE):** Uma interface rápida para consultar autorizações prévias e registrar a entrada de visitantes em poucos segundos.

* **Persona 2: A Gestão / Controle**
  * **Nome e Perfil:** Mariana Souza, 45 anos — Coordenadora de Segurança Patrimonial.
  * **Papel na Organização:** Responsável por auditar as entradas/saídas e reportar incidentes para a diretoria.
  * **Dores no Processo Atual (AS-IS):** Dificuldade para consolidar relatórios mensais e ausência de histórico confiável em caso de auditoria.
  * **Expectativas no Sistema (TO-BE):** Painel gerencial (*dashboard*) com relatórios de fluxo e alertas de permanência em tempo real.

---

> ✏️ **[Atenção aluno: Apague este bloco e detalhe as personas do seu projeto aqui]**
> 
> *Descreva as personas identificadas no contexto da sua equipe (lembre-se de cobrir todos os papéis reais mapeados nas entrevistas), detalhando perfil, dores no processo atual (AS-IS) e o que esperam da futura aplicação (TO-BE).*
