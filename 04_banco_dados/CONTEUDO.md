# Banco de Dados com SQL

## Sobre o Curso

Curso introdutório de Banco de Dados Relacionais e SQL voltado para iniciantes em Ciência de Dados. O conteúdo parte da teoria de bancos de dados e evolui até a modelagem, criação e consulta de tabelas relacionais com SQL.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Jupyter e VS Code.
**SGBD utilizado:** SQLite, acessado via biblioteca `sqlite3` e extensão `ipython-sql` (`%sql` / `%%sql`).
**Bancos de dados de exemplo:** `clientes.db`, `videogame_sales.db`, `sql_island.db`, banco modelado a partir de `BDEmpregados.pdf`.
**Total de aulas:** 2 aulas teórico-práticas + 2 notebooks de exercícios.

---

## Módulo Único — Fundamentos de Banco de Dados e SQL

Objetivo: compreender o papel dos bancos de dados relacionais, dominar a linguagem SQL para consulta e manipulação de dados, e aprender a modelar e criar um banco de dados relacional do zero.

---

### Aula 01 — Introdução a Banco de Dados e Consultas SQL

**Pasta:** `aulas/Aula01_Banco_Dados.ipynb`

Primeira aula do curso: contextualização sobre bancos de dados e introdução ao comando SELECT e suas cláusulas.

**Tópicos:**
- O que é um banco de dados (quiz de abertura)
- Apresentação da disciplina: presença dos bancos de dados no dia a dia
- Crescimento do volume de dados no mundo (Data Never Sleeps, unidades de medida — de Kilobyte a Zettabyte)
- Tipos de banco de dados: SQL (Relacional) vs. NoSQL (Chave-Valor, Grafo, Documentos, Colunar)
- Principais SGBDs relacionais: Oracle, SQL Server, IBM DB2, PostgreSQL, SQLite, MySQL
- Introdução à linguagem SQL e sua organização: DQL, DML, DDL, DCL, DTL
- Comando `SELECT`: sintaxe e exemplos
- Conectando a um banco SQLite com a biblioteca `sqlite3` e com a extensão `%sql` / `%%sql`
- Inspeção da estrutura de uma tabela com `PRAGMA table_info`
- Cláusula `WHERE` e operadores: `=`, `<>`, `OR`, `AND`, `()`, `LIKE`, `NOT LIKE`, `IN`, `NOT IN`, `BETWEEN`, `NOT BETWEEN`
- Cláusula `ORDER BY`
- Cláusula `GROUP BY` e funções de agregação: `COUNT`, `MAX`, `MIN`
- Cláusula `HAVING`
- Exercícios práticos com o dataset `VideoGame_Sales`

**Bibliotecas:** `sqlite3`, `ipython-sql`
**Banco de dados:** `clientes.db`, `videogame_sales.db`

---

### Prática 01 — SQL Island

**Pasta:** `aulas/Aula01_SQL_Island.ipynb`

Notebook de exercícios gamificado com um banco de dados temático (aldeias, habitantes e itens), consolidando `SELECT`, `WHERE`, `ORDER BY` e agregações.

**Exercícios:**
1. `SELECT` com `WHERE` — habitantes de uma cidade e filtro por sobrenome
2. `SELECT` com `WHERE` — identificar o chefe de cada aldeia
3. `SELECT` com `WHERE` composto e `ORDER BY` — filtro por sexo, cidade e quantidade de ouro
4. Agregação com `SUM` — cidade mais rica
5. `ORDER BY` — cidadão mais rico
6. Relacionamento entre tabelas — item e respectivo proprietário
7. Desafio: converter o resultado de um cursor SQL para um `DataFrame` do pandas

---

### Aula 02 — Manipulação de Dados, DDL e Relacionamentos

**Pasta:** `aulas/Aula02_Banco_Dados.ipynb`

Segunda aula do curso: evolução do SELECT para os comandos de manipulação e definição de dados, com foco em relacionamentos entre tabelas.

**Tópicos:**
- Revisão do conteúdo da aula anterior
- Comando `INSERT`: sintaxe e exemplos, com e sem lista explícita de colunas
- DDL — Data Definition Language: criação (`CREATE TABLE`) e remoção (`DROP TABLE`) de tabelas
- Escolha de tipos de dados e nomenclatura de colunas
- Restrições (constraints): `NULL` / `NOT NULL`, `CHECK`, `UNIQUE`, `DEFAULT`, `PRIMARY KEY`, `FOREIGN KEY`
- Comando `DELETE`: sintaxe e exemplos
- Comando `UPDATE`: sintaxe e exemplos
- Integridade referencial: chave primária, chave estrangeira e relacionamento entre tabelas
- `SELECT` com `JOIN` entre tabelas relacionadas

**Bibliotecas:** `sqlite3`, `ipython-sql`
**Banco de dados:** `clientes.db`

---

### Prática 02 — Modelagem do Banco BDEmpregados

**Pasta:** `aulas/Aula02_Exercicio2.ipynb`
**Material de apoio:** `aulas/BDEmpregados.pdf` — esquema de exemplo com as tabelas `Empregado`, `Departamento`, `Projeto`, `Dependentes`, `Departamento_Projeto` e `Empregado_Projeto`.

Exercício de consolidação: modelagem, criação e consulta de um banco de dados relacional completo a partir de um conjunto de tabelas de exemplo (RH).

**Exercícios:**
1. Criar todas as tabelas do modelo BDEmpregado, escolhendo o melhor tipo de dado e a melhor nomenclatura para cada atributo
2. Inserir todos os registros do modelo em suas respectivas tabelas
3. Selecionar todos os campos da tabela de empregados
4. Selecionar todos os campos da tabela de empregados ordenados por RG (decrescente)
5. Selecionar todos os campos da tabela de empregados ordenados por nome (decrescente)
6. Relacionar empregados e dependentes: nome do empregado, nome, data de nascimento e relação de cada dependente, ordenados por nome do dependente
7. Contar quantos empregados existem por departamento
8. Contar quantos empregados existem por projeto
9. Contar quantos projetos existem por departamento
10. Contar quantos dependentes existem no total

---

## Resumo Geral

| # | Tipo | Pasta | Título |
|---|---|---|---|
| 01 | Aula | `aulas/Aula01_Banco_Dados.ipynb` | Introdução a Banco de Dados e Consultas SQL |
| P1 | Prática | `aulas/Aula01_SQL_Island.ipynb` | SQL Island |
| 02 | Aula | `aulas/Aula02_Banco_Dados.ipynb` | Manipulação de Dados, DDL e Relacionamentos |
| P2 | Prática | `aulas/Aula02_Exercicio2.ipynb` | Modelagem do Banco BDEmpregados |

---

## Tecnologias e Bibliotecas

| Categoria | Tecnologias |
|---|---|
| **Linguagem** | Python 3.12, SQL |
| **Ambiente** | Google Colab, Jupyter Notebook, VS Code |
| **SGBD** | SQLite |
| **Acesso ao Banco** | `sqlite3`, `ipython-sql` (`%sql` / `%%sql`) |
| **Manipulação de Dados** | pandas (conversão de cursor para DataFrame) |
