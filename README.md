# <h1>Mini-Curso-SQL-NotebookLM</h1>
# Curso de orientação de estudos em SQL utilizando o NotebookLM. Com objetivo de manter atualizado sobre o conteúdo e também de orientar outras pessoas que estão querendo aprender ou que estão com alguma dificuldade pra realizar uma tarefa relacionada a este assunto.

<h2>  Sobre </h2>

<p> Este conteúdo estruturado apresenta os conceitos fundamentais de banco de dados, modelagem e a linguagem SQL, com base nos materiais fornecidos. </p>

<div>
<p> 1 PROMPT: Faça um resumo explicando sobre modelagem de dados
RESPOSTA:
	1 - A **modelagem de dados** é definida como uma coleção de ferramentas conceituais utilizadas para descrever os dados, seus relacionamentos, a semântica e as restrições envolvidas. Seu objetivo principal é replicar o funcionamento de um negócio real em uma estrutura digital profissional, permitindo a construção de soluções avançadas e a tomada de decisões estratégicas.

### Metodologia de Modelagem
O processo de modelagem geralmente segue quatro etapas fundamentais:
1.  **Análise de Requisitos:** Levantamento e análise das necessidades de negócio do software.
2.  **Modelo Conceitual:** Uma visão de alto nível que foca no entendimento geral dos dados e suas relações, frequentemente representada pelo **Diagrama de Entidade Relacionamento (DER)**.
3.  **Modelo Lógico:** Detalhamento das entidades, atributos e relacionamentos, incluindo o processo de **normalização** para garantir a consistência.
4.  **Modelo Físico:** A implementação prática do banco de dados em um Sistema Gerenciador de Banco de Dados (SGBD), utilizando linguagens como SQL.

### Componentes Principais do Modelo Relacional
No modelo relacional, os dados são organizados em tabelas que se conectam entre si. Os elementos centrais incluem:
*   **Entidades:** Conceitos do negócio sobre os quais se deseja armazenar informações (ex: Clientes, Vendas).
*   **Atributos (ou Campos):** As características específicas de cada entidade, como nome ou data.
*   **Relacionamentos:** Como as entidades interagem entre si, definidos por sua **cardinalidade** (ex: 1 para 1, 1 para muitos ou muitos para muitos).
*   **Chave Primária (PK):** Um identificador único para cada registro em uma tabela.
*   **Chave Estrangeira (FK):** Um atributo que estabelece uma ligação com a chave primária de outra tabela, garantindo a integridade referencial.

### Normalização
A normalização é uma técnica de otimização para reduzir redundâncias e evitar inconsistências nos dados. As principais formas são:
*   **Primeira Forma Normal (NF1):** Exige atributos únicos, sem valores multivalorados ou compostos na mesma célula.
*   **Segunda Forma Normal (NF2):** Determina que todos os atributos não-chave devem depender inteiramente da chave primária.
*   **Terceira Forma Normal (NF3):** Estabelece que os atributos não-chave devem ser independentes entre si.

### Tipos de Modelos de Dados
Existem diferentes abordagens dependendo da estrutura necessária:
*   **Modelos de Registro:** Incluem o **relacional** (baseado em tabelas), o de **rede** (organizado em grafos) e o **hierárquico** (organizado em árvores).
*   **SQL vs NoSQL:** O modelo **SQL** possui esquemas rígidos e é focado em relações complexas, enquanto o **NoSQL** possui esquemas flexíveis (como documentos JSON), sendo ideal para performance e grandes volumes de dados (Big Data). </p>
</div>

<div>
<p> 2 PROMPT: Me dê mais detalhes sobre a metodologia de modelagem
RESPOSTA:
	A metodologia de modelagem de dados é um processo estruturado que transforma as necessidades de um negócio em uma implementação técnica funcional. De acordo com os materiais, esse processo é dividido em quatro etapas fundamentais:

### 1. Análise de Requisitos
Esta é a fase inicial onde ocorre o **levantamento e a análise das necessidades de negócio** do software. O objetivo é entender quais informações o sistema precisa armazenar para cumprir seu propósito no mundo real.

### 2. Modelo Conceitual
Nesta etapa, foca-se na **concepção geral do negócio** através de uma visão de alto nível, independente de tecnologia. As atividades principais incluem:
*   **Definir Entidades:** Identificar conceitos do negócio que exigem armazenamento de informações (ex: Alunos, Cursos).
*   **Definir Atributos:** Listar as características de cada entidade (ex: nome, e-mail).
*   **Definir Relacionamentos:** Estabelecer como as entidades interagem entre si, definindo a **cardinalidade** (1 para 1, 1 para muitos, ou muitos para muitos).
*   **Construir o DER:** O resultado final desta fase é o **Diagrama de Entidade Relacionamento**, uma representação visual das entidades e suas conexões.

### 3. Modelo Lógico
Esta fase detalha as entidades e relacionamentos, preparando a estrutura para a implementação. O foco aqui é a **Normalização**, uma técnica de otimização para reduzir redundâncias e inconsistências. As três principais formas normais são:
*   **Primeira Forma Normal (NF1):** Garante que os atributos sejam únicos, sem valores multivalorados ou compostos (como endereços ou telefones misturados).
*   **Segunda Forma Normal (NF2):** Garante que todos os atributos não-chave dependam inteiramente da chave primária.
*   **Terceira Forma Normal (NF3):** Garante que os atributos não-chave sejam independentes entre si.

### 4. Modelo Físico
É a **implementação prática** do banco de dados em um Sistema Gerenciador de Banco de Dados (SGBD). Esta etapa envolve:
*   **Escolha da Tecnologia:** Decidir qual SGBD será usado (ex: MySQL, PostgreSQL, SQLite ou plataformas como Bubble).
*   **Criação via SQL:** Utilizar a linguagem SQL (comandos DDL como `CREATE TABLE`) para definir fisicamente as tabelas, tipos de dados (varchar, integer, date) e chaves (Primary Key e Foreign Key).
*   **Gestão e Manutenção:** Configurar as permissões de acesso e garantir o funcionamento contínuo do banco. </p>
</div>

<div>
<p> 3 PROMPT: Como a normalização ajuda na integridade das informações?
RESPOSTA:
	A **normalização** ajuda na integridade das informações principalmente ao **reduzir redundâncias, duplicações e inconsistências** nos dados armazenados. Ao organizar os dados de forma eficiente, ela garante que o modelo de dados seja mais consistente e organizado, facilitando a manutenção da precisão da informação ao longo do tempo.

De acordo com os materiais, a normalização contribui para a integridade através de regras específicas chamadas **Formas Normais**:

*   **Primeira Forma Normal (NF1):** Exige que a tabela possua apenas atributos únicos, eliminando atributos multivalorados ou compostos. Por exemplo, em vez de ter vários telefones em um único campo, eles são separados em registros individuais, evitando erros na recuperação e atualização.
*   **Segunda Forma Normal (NF2):** Determina que todos os atributos não-chave devem depender inteiramente da chave primária. Isso evita que informações de diferentes conceitos de negócio sejam misturadas na mesma tabela, o que poderia causar inconsistências se uma parte da informação fosse atualizada e a outra não.
*   **Terceira Forma Normal (NF3):** Estabelece que os atributos não-chave devem ser independentes entre si. Isso garante que a alteração de um dado não afete incorretamente outros campos que não deveriam ter relação direta com ele.

Além da normalização, o modelo relacional utiliza **restrições de integridade** para reforçar a validade dos dados:
*   **Chave Primária (PK):** Identifica cada registro de forma única, impedindo duplicidade.
*   **Chave Estrangeira (FK) e Integridade Referencial:** Garante que um valor em uma tabela obrigatoriamente exista na tabela relacionada. Por exemplo, não é permitido cadastrar uma venda para um curso que não existe no sistema.
*   **Cláusulas como NOT NULL e UNIQUE:** Previnem a entrada de informações vazias onde o preenchimento é obrigatório e evitam valores duplicados em campos específicos, como RG ou CPF.

Em suma, a normalização estrutura os dados para evitar que informações conflitantes existam no banco, enquanto as restrições de integridade do SGBD servem como "regras de segurança" para validar as operações de entrada e alteração. </p>
</div>

<div>
<p> 4 PROMPT: Explique a diferença entre chaves primarias e estrangeiras no sql
RESPOSTA:
	No SQL, a principal diferença entre chaves primárias e estrangeiras reside na sua função dentro do banco de dados: a **chave primária** serve para identificar registros de forma única dentro de sua própria tabela, enquanto a **chave estrangeira** estabelece uma ligação (relacionamento) entre tabelas distintas.

Abaixo, detalho as características e funções de cada uma:

### Chave Primária (Primary Key - PK)
*   **Função:** É o identificador exclusivo de cada registro em uma tabela.
*   **Unicidade:** Não podem existir duas linhas com o mesmo valor na chave primária.
*   **Valores Nulos:** Por padrão, os campos que compõem uma chave primária não podem conter valores nulos (`NOT NULL`), pois isso impediria a identificação do registro.
*   **Composição:** Pode ser formada por apenas um campo ou por um conjunto de campos (chamada de chave composta).
*   **Exemplo:** Em uma tabela de Alunos, o campo `id_aluno` identifica cada estudante de forma única.

### Chave Estrangeira (Foreign Key - FK)
*   **Função:** É um atributo que aponta para a chave primária de outra tabela, permitindo o relacionamento entre os dados.
*   **Integridade Referencial:** Garante que o valor inserido na tabela "filha" obrigatoriamente exista na tabela "pai". Por exemplo, não é possível cadastrar um funcionário em um departamento que não esteja previamente cadastrado na tabela de departamentos.
*   **Relacionamento:** Representa o "lado muitos" em relacionamentos de 1 para muitos (1:N). Por exemplo, um curso pode ter várias vendas relacionadas a ele através da chave estrangeira `id_curso` na tabela de Vendas.
*   **Valores Nulos:** Diferente da PK, uma chave estrangeira pode aceitar valores nulos, caso o relacionamento não seja obrigatório (ex: um funcionário que ainda não foi alocado em nenhum banco). </p>
### Resumo das Diferenças

| Característica | Chave Primária (PK) | Chave Estrangeira (FK) |
| :--- | :--- | :--- |
| **Propósito** | Identificar uma linha de forma única. | Relacionar tabelas entre si. |
| **Unicidade** | O valor deve ser único na tabela. | Os valores podem se repetir (ex: vários funcionários no mesmo depto). |
| **Nulos** | Não permite valores nulos. | Pode permitir nulos, se o projeto permitir. |
| **Localização** | Existe na própria tabela onde define os dados. | Existe em uma tabela referenciando outra. |

### Implementação em SQL
Para definir essas chaves durante a criação de uma tabela, utilizam-se as cláusulas `PRIMARY KEY` e `FOREIGN KEY` associadas a `REFERENCES`:

```sql
CREATE TABLE cursos (
    id_curso integer PRIMARY KEY, -- Define a Chave Primária
    nome_curso varchar(200) NOT NULL,
    id_professor integer,
    FOREIGN KEY (id_professor) REFERENCES professores (id_professor) -- Define a Chave Estrangeira
);
```
No exemplo acima, `id_curso` garante que cada curso seja único, enquanto `id_professor` garante que o curso esteja vinculado a um professor válido que já existe na tabela de professores.
</div>

<div>
<p> 5 PROMPT: Mostre exemplos dos principais comandos DML em sql:
RESPOSTA:
	A **Linguagem de Manipulação de Dados (DML)** é o conjunto de comandos SQL utilizados para acessar, recuperar, inserir, remover e modificar informações em um banco de dados. Os quatro comandos fundamentais da série DML são **SELECT**, **INSERT**, **UPDATE** e **DELETE**.

Abaixo estão os detalhes e exemplos de cada um, conforme as fontes:

### 1. SELECT (Consulta)
É o comando principal da DML, utilizado para **recuperar informações** armazenadas. Ele permite listar campos específicos, filtrar registros com condições e ordenar os resultados.

*   **Selecionar colunas específicas:**
    `SELECT Ra, Nome FROM aluno WHERE serie = 3`
*   **Selecionar todas as colunas de uma tabela:**
    `SELECT * FROM funcionarios`
*   **Filtrar com múltiplas condições (Operadores lógicos):**
    `SELECT * FROM funcionarios WHERE cod_depto = 4 AND dt_admissao = '1985/02/11'`
*   **Ordenar resultados:**
    `SELECT serie, nome FROM aluno ORDER BY serie DESC, nome ASC`
*   **Eliminar resultados duplicados:**
    `SELECT DISTINCT salario FROM funcionarios`

### 2. INSERT (Inserção)
Este comando é utilizado para **carregar novos dados** em uma tabela que foi criada previamente.

*   **Inserção simples (seguindo a ordem das colunas):**
    `INSERT INTO aluno VALUES (123251, 'José da Silva', 3, 'B', 'Rua Direita, 45')`
*   **Inserção especificando as colunas (útil quando não se lembra a ordem exata):**
    `INSERT INTO aluno(nome, ra, serie, endereco, turma) VALUES ('José da Silva', 123251, 3, 'Rua Direita, 45', 'B')`

### 3. UPDATE (Alteração)
O comando **UPDATE** serve para **modificar o valor de um campo** em um registro já existente ou em um grupo de registros que atendam a uma condição.

*   **Alterar um registro específico:**
    `UPDATE aluno SET serie = 4 WHERE ra = 123251`
*   **Alterar múltiplos registros simultaneamente:**
    `UPDATE aluno SET serie = 4 WHERE serie = 3 AND turma = 'B'`

### 4. DELETE (Remoção)
Utilizado para **excluir registros** de uma tabela. É fundamental utilizar a cláusula `WHERE` para evitar a exclusão acidental de todos os dados.

*   **Remover registros específicos:**
    `DELETE FROM aluno WHERE serie = 3 AND turma = 'A'`
*   **Remover todos os registros de uma tabela:**
    `DELETE FROM alunos`

### Resumo das Funções DML

| Comando | Função Principal |
| :--- | :--- |
| **SELECT** | Recuperação/Consulta de informações. |
| **INSERT** | Inserção de novas informações. |
| **UPDATE** | Modificação de informações existentes. |
| **DELETE** | Remoção de informações. | </p>
</div>

<div>
<p> 6 PROMPT: A partir desses exemplos mostre agora como consultar registros em várias tabelas utilizando joins
RESPOSTA:
	Para consultar registros em várias tabelas simultaneamente, a SQL utiliza o conceito de **relacionamento** ou **Junções (Joins)**. No modelo relacional, os dados não estão isolados; as tabelas se conectam através de chaves primárias e estrangeiras.

Abaixo, detalho as principais formas de realizar essas consultas conforme os materiais:

### 1. Junção Implícita (via cláusula WHERE)
Esta é a forma básica de relacionar tabelas. Você lista as tabelas desejadas na cláusula `FROM` e estabelece a condição de ligação na cláusula `WHERE`. Sem essa condição, o banco de dados realiza um **Produto Cartesiano**, combinando cada linha de uma tabela com todas as linhas da outra, o que geralmente gera resultados incorretos.

*   **Exemplo:** Consultar o nome do funcionário e o nome do seu departamento:
    `SELECT funcionarios.nome, deptos.nome FROM funcionarios, deptos WHERE funcionarios.cod_depto = deptos.cod_depto`

### 2. Uso de Variáveis de Tupla (Aliases/Apelidos)
Quando tabelas diferentes possuem colunas com o mesmo nome (como "nome" na tabela de funcionários e "nome" na de departamentos), é obrigatório identificar a qual tabela você se refere usando a notação `tabela.coluna`. Para simplificar, você pode criar **apelidos** na cláusula `FROM`.

*   **Exemplo:**
    `SELECT F.nome, D.nome FROM funcionarios F, deptos D WHERE F.cod_depto = D.cod_depto`

### 3. KEY JOIN
Alguns sistemas permitem o uso da cláusula `KEY JOIN`, que efetua o relacionamento **automaticamente** baseando-se nas chaves primárias e estrangeiras definidas no modelo físico, simplificando a escrita da consulta.

*   **Exemplo:**
    `SELECT funcionarios.nome, deptos.nome FROM funcionarios KEY JOIN deptos`
    *Nota: Esta cláusula exige que o relacionamento seja direto e que não existam valores nulos na chave de ligação.*

### 4. Outer Joins (Junções Externas)
As junções comuns (vistas acima) desprezam registros que não possuem um correspondente na outra tabela. Se você quiser listar **todos** os registros de uma tabela, mesmo aqueles que não têm vínculo (como um funcionário que ainda não possui conta em banco), deve usar o **Outer Join**.

*   **LEFT OUTER JOIN (`*=`):** Traz todas as linhas da tabela à **esquerda**, mesmo sem correspondência na direita.
    `SELECT funcionarios.nome, bancos.nome FROM funcionarios LEFT OUTER JOIN bancos`
    *(Ou em algumas sintaxes: `WHERE funcionarios.cod_banco *= bancos.cod_banco`)*

*   **RIGHT OUTER JOIN (`=*`):** Traz todas as linhas da tabela à **direita**.
    `SELECT funcionarios.nome, bancos.nome FROM funcionarios RIGHT OUTER JOIN bancos`

### Resumo das Junções

| Tipo de Join | Função |
| :--- | :--- |
| **Simple Join (WHERE)** | Retorna apenas registros que possuem correspondência em ambas as tabelas. |
| **KEY JOIN** | Realiza a junção automática baseada nas chaves do banco. |
| **LEFT OUTER JOIN** | Garante que todos os dados da primeira tabela sejam exibidos. |
| **RIGHT OUTER JOIN** | Garante que todos os dados da segunda tabela sejam exibidos. |

Você também pode utilizar **Sub-consultas** (SELECTs aninhados) para recuperar informações de outras tabelas, o que às vezes pode ser mais rápido em termos de execução. </p>
</div>

<div>
<p> 7 PROMPT: Como funcionam as sub-consultas em relação aos Joins?
RESPOSTA:
	As sub-consultas e os *joins* são ferramentas utilizadas para recuperar informações de múltiplas tabelas, mas operam de maneiras distintas. Enquanto os **joins** conectam tabelas diretamente na cláusula `FROM` para formar um conjunto de resultados combinados, as **sub-consultas** são comandos `SELECT` aninhados dentro de outro `SELECT` que devolvem resultados intermediários.

Abaixo estão os detalhes de funcionamento e as principais diferenças entre eles:

### Funcionamento das Sub-consultas
Uma sub-consulta é executada para **cada linha** retornada pela consulta principal. Ela pode ser posicionada em diferentes partes do comando SQL:
*   **Antes da cláusula FROM:** Utilizada para criar colunas temporárias que buscam dados em outras tabelas. Por exemplo, para mostrar o nome de um funcionário e buscar sua agência bancária em outra tabela sem listá-la no `FROM` principal.
*   **Na cláusula WHERE:** Utilizada para filtrar a consulta principal com base em uma lista de valores ou em uma condição lógica.

### Relação e Comparação com os Joins
*   **Substituição:** Em muitos casos, é possível obter o mesmo resultado usando sub-consultas ou *joins*. Por exemplo, você pode usar um `WHERE` com `IN (sub-consulta)` para filtrar registros que existam em outra tabela, o que equivale a um *join*.
*   **Performance:** Os materiais indicam que, em diversas situações, é **vantajoso utilizar sub-consultas** em vez de relacionar várias tabelas no `SELECT` principal via *join*, pois elas podem ser executadas de forma mais rápida pelo sistema.
*   **Limitação de Linhas:** Diferente de um *join*, que pode multiplicar as linhas de uma tabela (Produto Cartesiano) se não houver um filtro adequado, uma sub-consulta padrão **não pode retornar mais de uma linha** por registro da consulta principal, sob risco de erro na execução.
*   **Lógica de Conjuntos:** As sub-consultas permitem o uso de operadores de comparação de conjuntos como `>some`, `>all`, `exists` e `not exists`, que testam a existência ou a relação de um valor contra um grupo de resultados de forma mais direta do que um *join* tradicional.

### Uso da Condição EXISTS
A condição `EXISTS` é uma forma comum de utilizar sub-consultas como alternativa aos *joins*. Ela retorna um valor lógico (verdadeiro ou falso) se a sub-consulta encontrar pelo menos uma linha correspondente, o que evita o erro de "múltiplas linhas" comum em outras formas de aninhamento. </p>
</div>

<div>
<p> 8 - PROMPT: Quais são as funções de agregação e como usá-las?
RESPOSTA:
	As funções de agregação (ou funções agregadas) são ferramentas da linguagem SQL utilizadas para realizar cálculos em grupos de registros, operando em "agregações" de linhas para retornar um **valor único** como resultado. Elas são essenciais para transformar grandes volumes de dados em informações sumarizadas e úteis para a tomada de decisões.

De acordo com as fontes, as principais funções e suas formas de uso são:

### Principais Funções de Agregação
*   **`avg` (Média):** Calcula a média aritmética dos valores de uma coluna. Exemplo: `SELECT avg(salario) FROM funcionarios`.
*   **`sum` (Soma):** Totaliza os valores de uma coluna numérica. Exemplo: `SELECT sum(salario) FROM funcionarios`.
*   **`count` (Contagem):** Conta o número de registros. Pode ser usada como `count(*)` para contar todas as linhas de uma tabela ou em conjunto com `DISTINCT` para contar valores únicos.
*   **`min` (Mínimo):** Identifica o menor valor em um conjunto de registros.
*   **`max` (Máximo):** Identifica o maior valor em um conjunto de registros.
*   **`list` (Lista):** Retorna uma lista de valores separados por vírgula (função específica de algumas implementações como o ISQL).

### Como usá-las corretamente
Para extrair o potencial máximo dessas funções, elas são frequentemente combinadas com outras cláusulas:

1.  **Cláusula `GROUP BY`:** É utilizada para dividir as linhas de uma tabela em grupos menores baseados em um ou mais atributos. Por exemplo, para ver o total de salários por departamento: `SELECT cod_depto, sum(salario) FROM funcionarios GROUP BY cod_depto`.
2.  **Cláusula `HAVING`:** Serve para aplicar condições de filtro aos **grupos** resultantes do `GROUP BY`, permitindo o uso de funções de agregação na comparação. Exemplo: buscar agências onde a média de saldo é superior a 1.200: `... GROUP BY agencia HAVING avg(saldo) > 1200`.
3.  **Uso de `DISTINCT`:** Pode ser inserido dentro da função para eliminar duplicatas antes do cálculo. Por exemplo, para contar quantos clientes únicos possuem conta em uma agência: `count(distinct nome_cliente)`.
4.  **Tratamento de Nulos (`ISNULL`):** Operações matemáticas com valores nulos resultam em nulo. Para evitar isso em agregações, usa-se a função `ISNULL(campo, 0)` para tratar o valor como zero caso ele não exista.

### Regras e Restrições Importantes
*   **Não composição:** As funções agregadas **não podem ser compostas** diretamente na SQL (ex: não é permitido usar `max(avg(saldo))`).
*   **Ordem de execução:** Em uma consulta complexa, o predicado `WHERE` é aplicado primeiro para filtrar linhas individuais; em seguida, as linhas restantes são agrupadas pelo `GROUP BY` e, por fim, o `HAVING` filtra esses grupos.
*   **Padrão ANSI:** Requer que a função `count` seja utilizada preferencialmente como `count(*)` ou `count(distinct...)`.
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

