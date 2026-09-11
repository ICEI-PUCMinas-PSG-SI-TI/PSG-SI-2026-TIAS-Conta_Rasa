
# 5. Arquitetura e Projeto da Solução

<span style="color:red">Pré-requisitos: <a href="04-Modelagem do Processo de Negocio.md"> Modelagem do Processo de Negocio</a></span>

Nesta etapa, a equipe traduzirá os processos e requisitos mapeados anteriormente em uma arquitetura de software funcional, definindo o ecossistema tecnológico, a interface com o usuário, o modelo de dados e a infraestrutura do projeto.

---

## 5.1. Tecnologias Utilizadas
Descreva o ecossistema tecnológico adotado pela equipe para implementar a solução (linguagens, frameworks, bibliotecas, SGBD, ferramentas de versionamento e IDEs). 


| Dimensão | Tecnologia / Ferramenta |
| :--- | :--- |
| **SGBD** | MySQL / PostgreSQL |
| **Front-end** | HTML, CSS, JavaScript (ou Framework escolhido) |
| **Back-end** | Java Spring Boot / Node.js / Python |
| **Deploy / Hospedagem** | GitHub Pages / Render / Vercel |
| **Gerenciamento de Projeto** | GitHub Projects (Sprints) |

---

## 5.2. Arquitetura da Solução
A arquitetura da solução descreve a organização estrutural do sistema, detalhando os módulos, componentes e a forma como eles se comunicam com base nas tecnologias escolhidas.

![Exemplo de um modelo de arquitetura do Site](https://miro.medium.com/v2/resize:fit:1400/1*WjQdDCRWq609T-krfFL6gA.png)

> 💡 **Inspiração e Alinhamento Esperado:** 
> O diagrama de arquitetura apresentado abaixo serve como principal referência e modelo inspirador para o desenvolvimento do projeto de vocês. **O motivo é estratégico:** este modelo está estruturalmente muito próximo do que a docência da disciplina espera e avalia. Ele contempla de forma clara a integração entre as camadas, a descrição do banco de dados utilizado, as ferramentas de suporte, as linguagens de programação e a infraestrutura envolvida. 


> ✏️ **[Atenção aluno: Utilize a estrutura da figura abaixo como inspiração para desenhar a arquitetura da sua equipe, apague a imagem de exemplo para manter a documentação limpa e discorra textualmente sobre ela]**
> 


---

## 5.3 Requisitos do Software

Esta seção apresenta os requisitos funcionais e não funcionais levantados para o desenvolvimento do sistema, detalhando as funcionalidades esperadas e os atributos de qualidade da solução.

### 5.3.1 Requisitos Funcionais

A tabela abaixo relaciona os Requisitos Funcionais (RF) do sistema, indicando suas descrições e níveis de prioridade. 

| ID | Descrição do Requisito | Prioridade |
| :--- | :--- | :---: |
| **RF-01** | O sistema deve permitir que os usuários criem uma conta informando nome, e-mail, senha e endereço. | 🔴 ALTA |
| **RF-02** | O sistema deve permitir que os usuários adicionem produtos ao carrinho de compras. | 🟡 MÉDIA |
| **RF-03** | O sistema deve permitir que o cliente realize o pagamento do pedido utilizando cartão de crédito ou Pix. | 🔴 ALTA |
| **RF-04** | O sistema deve permitir que o administrador cadastre, edite e remova produtos do catálogo. | 🔴 ALTA |

---
### 5.3.2 Requisitos Não Funcionais

Os Requisitos Não Funcionais (RNF) definem as características de qualidade, restrições e atributos técnicos que garantem o bom funcionamento e a confiabilidade da solução.

| ID | Descrição do Requisito | Prioridade |
| :--- | :--- | :---: |
| **RNF-01** | O sistema deve carregar as páginas principais em até 3 segundos sob condições normais de rede. | 🟡 MÉDIA |
| **RNF-02** | O sistema deve proteger as informações confidenciais dos clientes (como senhas e dados de pagamento) por meio de criptografia forte (ex: HTTPS/TLS e bcrypt). | 🔴 ALTA |
| **RNF-03** | O sistema deve ser compatível e responsivo para acesso via navegadores modernos de desktops, tablets e smartphones. | 🔴 ALTA |


---
## 5.4. Wireframes (Esquemáticas de Tela)
Os wireframes estruturam o layout, a disposição dos elementos e a experiência de uso (*User Experience*), definindo de forma esquemática a interface visual antes de iniciar a codificação. Eles devem refletir as interações necessárias para atender às Histórias de Usuário e aos Requisitos Funcionais, materializando graficamente o fluxo que a persona executará no sistema.

![Exemplo de Wireframe tela de Login referente ao RF 01](https://fga-eps-mds.github.io/2020.1-eSaudeUnB-Wiki/img/TelaLogin.png)

> ✏️ **[Atenção aluno: Insira os protótipos/wireframes das principais telas da aplicação abaixo. Aluno você deve apagar a Figura de Exemplo para evitar poluição visual da documentação.]**
> 
> *Lembre-se de informar qual Requisito Funcional corresponde a tela (wiereframe apresentada na documentação).*
> 


---

## 5.5. Modelo de Dados
O desenvolvimento da solução requer uma base de dados integrada que permita efetuar cadastros e controles associados aos processos mapeados. 

### 5.5.1. Modelo Entidade-Relacionamento (MER)
O Modelo ER representa graficamente como as entidades (objetos de negócio) se relacionam entre si na aplicação.

![Exemplo de Modelo ER](https://leonardofonseca.com.br/wp-content/uploads/2021/04/image.png?w=421)

> ✏️ **[Atenção aluno: Insira a imagem do Diagrama Entidade-Relacionamento (DER) integrado aqui. Aluno você deve apagar a Figura de Exemplo para evitar poluição visual da documentação]**
> 


### 5.5.2. Esquema Relacional
O Es5quema Relacional corresponde à representação estruturada dos dados em tabelas, especificando chaves primárias e estrangeiras.
![Exemplo de um modelo relacional](images/modeloRelacional.png "Exemplo de Modelo Relacional.")

> ✏️ **[Atenção aluno: Insira o diagrama ou a representação textual do Esquema Relacional aqui. Aluno você deve apagar a Figura de Exemplo para evitar poluição visual da documentação]**

### 5.5.3. Modelo Físico (Script SQL)
O script de criação das tabelas do banco de dados deve ser versionado no diretório `src/bd/` do repositório.

> ✏️ **[Atenção aluno: Insira o script SQL ou a referência do arquivo abaixo]**

```sql
-- Exemplo de Script SQL Base
CREATE TABLE Usuario (
    UsuId INT AUTO_INCREMENT PRIMARY KEY,
    UsuNome VARCHAR(100) NOT NULL,
    UsuEmail VARCHAR(100) UNIQUE NOT NULL
);



