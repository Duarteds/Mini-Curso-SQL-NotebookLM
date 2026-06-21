# <h1>Mini-Curso-SQL-NotebookLM</h1>

# <H4>Curso de orientação de estudos em SQL utilizando o NotebookLM. Com objetivo de manter atualizado sobre o conteúdo e também de orientar outras pessoas que estão querendo aprender ou que estão com alguma dificuldade pra realizar uma tarefa relacionada a este assunto.</H4>

<h2>  Sobre </h2>

<p> Este conteúdo estruturado apresenta os conceitos fundamentais de banco de dados, modelagem e a linguagem SQL, com base nos materiais fornecidos. </p>

<div>
<p> 1 PROMPT: Faça um resumo explicando sobre modelagem de dados
    2 PROMPT: Me dê mais detalhes sobre a metodologia de modelagem
	3 PROMPT: Como a normalização ajuda na integridade das informações?
	4 PROMPT: Explique a diferença entre chaves primarias e estrangeiras no sql
	5 PROMPT: Mostre exemplos dos principais comandos DML em sql
	6 PROMPT: A partir desses exemplos mostre agora como consultar registros em várias tabelas utilizando joins
	7 PROMPT: Como funcionam as sub-consultas em relação aos Joins?
	8 PROMPT: Quais são as funções de agregação e como usá-las?
</p>
</div>

<div>
<p> Resumo:
	Este resumo estruturado apresenta os conceitos fundamentais de banco de dados, modelagem e a linguagem SQL**, com base nos materiais fornecidos.

### 1. Fundamentos de Banco de Dados
Um banco de dados é um **conjunto organizado de informações** que permite a recuperação eficiente de dados, podendo ser manual ou computadorizado. O objetivo principal é fornecer aos usuários uma visão abstrata, escondendo detalhes técnicos de armazenamento.
*   **SGBD (Sistema Gerenciador de Banco de Dados):** É o software responsável por gerenciar o banco, garantindo segurança, integridade e acesso padronizado.
*   **SQL (Structured Query Language):** É a linguagem padrão mundial para definição e manipulação de dados em bancos relacionais.

### 2. Metodologia de Modelagem de Dados
A modelagem traduz as regras de negócio para uma estrutura digital através de quatro etapas:
1.  **Análise de Requisitos:** Levantamento das necessidades do software.
2.  **Modelo Conceitual:** Visão de alto nível que foca no entendimento do negócio, resultando no **Diagrama de Entidade Relacionamento (DER)**.
3.  **Modelo Lógico:** Detalhamento de entidades e atributos, onde ocorre a **Normalização**.
4.  **Modelo Físico:** Implementação prática no SGBD escolhido (ex: MySQL, PostgreSQL) usando comandos SQL.

### 3. O Modelo Relacional e Normalização
Os dados são organizados em **tabelas (relações)** compostas por **linhas (tuplas)** e **colunas (atributos)**.
*   **Chave Primária (PK):** Identificador exclusivo de cada registro em uma tabela.
*   **Chave Estrangeira (FK):** Atributo que aponta para a PK de outra tabela, estabelecendo o relacionamento e garantindo a **integridade referencial**.
*   **Normalização:** Técnica para reduzir redundâncias e inconsistências.
    *   **NF1:** Atributos devem ser únicos (atômicos), sem valores multivalorados.
    *   **NF2:** Atributos não-chave devem depender inteiramente da chave primária.
    *   **NF3:** Atributos não-chave devem ser independentes entre si.

### 4. Linguagem SQL
A linguagem é dividida principalmente em:
*   **DDL (Definição):** Comandos como `CREATE`, `ALTER` e `DROP` para estruturar o banco.
*   **DML (Manipulação):** Comandos para lidar com os dados:
    *   **SELECT:** Recupera informações.
    *   **INSERT:** Adiciona novos registros.
    *   **UPDATE:** Modifica registros existentes.
    *   **DELETE:** Remove registros.

### 5. Consultas Avançadas
*   **Joins (Junções):** Permitem relacionar múltiplas tabelas. O **Inner Join** (ou junção via `WHERE`) traz apenas correspondências; o **Outer Join** (`LEFT` ou `RIGHT`) garante a exibição de todos os dados de um dos lados, mesmo sem par correspondente.
*   **Funções de Agregação:** Operam em grupos de linhas para retornar um valor único, como `avg` (média), `sum` (soma), `count` (contagem), `min` e `max`. São frequentemente usadas com a cláusula **GROUP BY**.
*   **Subconsultas:** Comandos `SELECT` aninhados dentro de outros, úteis para filtros complexos ou criação de colunas temporárias.
*   **Operações de Conjunto:** `UNION` (une resultados), `INTERSECT` (interseção) e `MINUS` (diferença).

### 6. SQL vs NoSQL
*   **SQL:** Bancos relacionais com esquemas (schemas) rígidos, focados em relações complexas e consistência.
*   **NoSQL:** Bancos não relacionais com esquemas flexíveis (como documentos JSON), ideais para performance e grandes volumes de dados (**Big Data**). </p>
</div>

<div>
<p> Glossário:
	Com base nos materiais, preparei um **glossário** com os termos fundamentais de modelagem de dados e SQL aprendidos até aqui:

### **Conceitos Fundamentais**
*   **Banco de Dados:** Um conjunto de informações organizadas e relacionadas entre si que representam aspectos do mundo real, podendo ser manual ou computadorizado.
*   **SGBD (Sistema Gerenciador de Banco de Dados):** Software responsável por gerenciar todo o banco de dados, permitindo criar, manipular e manter os dados de forma segura e organizada.
*   **SQL (Structured Query Language):** Linguagem padrão mundial utilizada para trabalhar com bancos de dados relacionais, realizando definições, manipulações e consultas (queries).
*   **NoSQL (Not Only SQL):** Bancos de dados não relacionais que utilizam esquemas flexíveis (dinâmicos), ideais para performance em grandes volumes de dados (Big Data).

### **Estrutura de Dados**
*   **Tabela (Relação):** Unidade básica de armazenamento de dados em um banco relacional, composta por um conjunto de colunas e linhas.
*   **Atributo (Coluna/Campo):** Representa uma característica ou propriedade de uma entidade (ex: nome, idade, e-mail).
*   **Tupla (Linha/Registro):** Um conjunto de atributos que formam um registro individual e único dentro de uma tabela.
*   **Domínio:** O conjunto de valores válidos que um atributo pode assumir.
*   **Nulo (NULL):** Um valor especial que indica que o conteúdo de um campo é desconhecido ou não foi designado.

### **Modelagem e Relacionamentos**
*   **Entidade:** Conceitos do mundo real ou do negócio sobre os quais se deseja armazenar informações (ex: Alunos, Vendas).
*   **DER (Diagrama de Entidade Relacionamento):** Representação visual que detalha as entidades, seus atributos e como elas se conectam.
*   **Cardinalidade:** Define a quantidade de ocorrências de uma entidade que podem estar associadas a outra (ex: 1 para 1, 1 para muitos, muitos para muitos).
*   **Chave Primária (PK):** Um identificador exclusivo que garante que cada registro em uma tabela seja único e não nulo.
*   **Chave Estrangeira (FK):** Um atributo em uma tabela que aponta para a chave primária de outra, estabelecendo um relacionamento entre elas.

### **Normalização**
*   **Normalização:** Técnica de otimização das tabelas para reduzir redundâncias, duplicações e evitar inconsistências nos dados.
*   **Primeira Forma Normal (NF1):** Regra que exige que a tabela possua apenas atributos únicos (atômicos), sem valores multivalorados ou compostos.
*   **Segunda Forma Normal (NF2):** Determina que todos os atributos não-chave devem depender inteiramente da chave primária.
*   **Terceira Forma Normal (NF3):** Estabelece que os atributos não-chave devem ser independentes entre si.

### **Linguagem SQL**
*   **DDL (Data Definition Language):** Conjunto de comandos para definir e modificar a estrutura do banco (ex: `CREATE`, `ALTER`, `DROP`).
*   **DML (Data Manipulation Language):** Conjunto de comandos para manipular os dados internos (ex: `SELECT`, `INSERT`, `UPDATE`, `DELETE`).
*   **Joins (Junções):** Operações que permitem relacionar e consultar dados de múltiplas tabelas simultaneamente.
*   **Funções de Agregação:** Ferramentas que realizam cálculos sobre um grupo de registros, devolvendo um valor único (ex: `SUM`, `AVG`, `COUNT`, `MAX`, `MIN`).
*   **Subconsultas:** Comandos `SELECT` aninhados dentro de outros comandos para obter resultados intermediários.
*   **Visão (View):** Uma tabela virtual cujo conteúdo é definido pelo resultado de uma consulta, sem armazenar os dados fisicamente. </p>
</div>

## Tecnologias
<div>
<p> NotebookLM </p>
</div>

## Time
Diógenes Duarte

