# Plano de Aula — Banco de Dados com SQL

**Curso:** Banco de Dados com SQL
**Carga horária total:** 3h (2 aulas de 1h30min)
**Modalidade:** Online / Presencial
**Público-alvo:** Iniciantes em Banco de Dados e Ciência de Dados
**Pré-requisito:** Nenhum — o curso parte do zero
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)
**SGBD utilizado:** SQLite, via `sqlite3` e extensão `%sql` / `%%sql`
**Modelo de aprendizagem:** Sala de aula invertida — o conteúdo teórico é consumido pelo aluno no site antes da aula; o tempo presencial é dedicado a prática, dúvidas e consolidação.

---

> **Importante para os alunos:** Cada aula pressupõe que você já acessou o website do curso e consumiu as aulas indicadas na seção **Preparação** antes de comparecer à sessão presencial. Chegar sem ter feito essa preparação compromete seu aproveitamento, pois o tempo em sala será dedicado à prática, não à exposição teórica.

---

## Aula 1 — Fundamentos e Consultas SQL

**Duração:** 1h30min
**Notebooks de referência:** `Aula01_Banco_Dados.ipynb`, `Aula01_SQL_Island.ipynb`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir os seguintes conteúdos **antes** desta sessão:

| # | Conteúdo no site | Assunto |
|---|---|---|
| 1 | O que é um banco de dados | Conceito, crescimento do volume de dados e tipos de banco (SQL x NoSQL) |
| 2 | Introdução a SQL | Organização da linguagem: DQL, DML, DDL, DCL, DTL |
| 3 | Comando SELECT | Sintaxe básica e conexão a um banco SQLite |
| 4 | Cláusula WHERE | Operadores de filtro (`=`, `<>`, `AND`, `OR`, `LIKE`, `IN`, `BETWEEN`, etc.) |
| 5 | Cláusulas ORDER BY, GROUP BY e HAVING | Ordenação, agregação (`COUNT`, `MAX`, `MIN`) e filtro de grupos |

### Objetivo Geral

Consolidar, por meio de prática guiada, os conceitos fundamentais de banco de dados relacional e o uso do comando `SELECT` com suas principais cláusulas.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Conectar-se a um banco de dados SQLite via `sqlite3` e via `%sql` / `%%sql`
- Inspecionar a estrutura de uma tabela com `PRAGMA table_info`
- Escrever consultas `SELECT` com filtros usando `WHERE` e seus operadores
- Ordenar resultados com `ORDER BY`
- Agrupar e agregar dados com `GROUP BY`, `COUNT`, `MAX` e `MIN`
- Filtrar grupos agregados com `HAVING`

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula |
| Prática guiada — Conexão e SELECT | `sqlite3`, `%sql`/`%%sql`, `PRAGMA table_info`, `SELECT` básico com `clientes.db` |
| Prática guiada — WHERE, ORDER BY, GROUP BY, HAVING | Operadores de filtro, ordenação e agregação com `clientes.db` |
| Prática autônoma — VideoGame Sales | Exercícios do notebook `Aula01_Banco_Dados` com `videogame_sales.db` |
| Prática autônoma — SQL Island | Exercícios gamificados do notebook `Aula01_SQL_Island` |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo consumido no site (máx. 5 min)
- Prática guiada: instrutor e aluno executam os notebooks juntos
- Prática autônoma com exercícios; instrutor circula para apoio

### Recursos

- Google Colab (sem instalação)
- Notebooks: `Aula01_Banco_Dados.ipynb`, `Aula01_SQL_Island.ipynb`
- Bancos de dados: `clientes.db`, `videogame_sales.db`, `sql_island.db`
- Bibliotecas: `sqlite3`, `ipython-sql` (pré-instaladas ou instaláveis no Colab)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula |
| 0:05 – 0:15 | 10 min | **Prática guiada:** conectar ao banco `clientes.db` com `sqlite3` e com `%sql`/`%%sql`; inspecionar estrutura com `PRAGMA table_info` |
| 0:15 – 0:30 | 15 min | **Prática guiada:** `SELECT` com `WHERE` — operadores `=`, `<>`, `AND`, `OR`, `()`, `LIKE`, `IN`, `BETWEEN` |
| 0:30 – 0:45 | 15 min | **Prática guiada:** `ORDER BY`, `GROUP BY` com `COUNT`/`MAX`/`MIN` e `HAVING` |
| 0:45 – 1:05 | 20 min | **Prática autônoma (`Aula01_Banco_Dados`):** exercícios com `videogame_sales.db` |
| 1:05 – 1:25 | 20 min | **Prática autônoma (`Aula01_SQL_Island`):** exercícios a–f |
| 1:25 – 1:30 | 5 min | Desafio (SQL Island, item g) e encerramento |

### Avaliação

O aluno conclui a aula com um notebook funcional capaz de conectar a um banco SQLite e responder a perguntas de negócio usando `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY` e `HAVING`.

---

## Aula 2 — Manipulação de Dados, DDL e Modelagem

**Duração:** 1h30min
**Notebooks de referência:** `Aula02_Banco_Dados.ipynb`, `Aula02_Exercicio2.ipynb`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir os seguintes conteúdos **antes** desta sessão:

| # | Conteúdo no site | Assunto |
|---|---|---|
| 6 | Comando INSERT | Inserção de registros, com e sem lista de colunas |
| 7 | DDL — CREATE e DROP TABLE | Criação e remoção de tabelas, tipos de dados |
| 8 | Restrições (constraints) | `NOT NULL`, `CHECK`, `UNIQUE`, `DEFAULT`, `PRIMARY KEY`, `FOREIGN KEY` |
| 9 | Comandos DELETE e UPDATE | Exclusão e atualização de registros |
| 10 | Integridade referencial e JOIN | Relacionamento entre tabelas, chave primária e estrangeira |

### Objetivo Geral

Consolidar, por meio de prática guiada e atividade final, a criação, manipulação e relacionamento de tabelas em um banco de dados relacional.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Inserir, atualizar e excluir registros com `INSERT`, `UPDATE` e `DELETE`
- Criar e remover tabelas com `CREATE TABLE` e `DROP TABLE`, definindo tipos de dados e restrições adequadas
- Aplicar chave primária e chave estrangeira para garantir integridade referencial
- Escrever consultas `SELECT` com `JOIN` entre tabelas relacionadas
- Modelar e construir um banco de dados relacional completo a partir de um conjunto de tabelas de exemplo

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula |
| Prática guiada — INSERT | Inserção de registros em `clientes.db` |
| Prática guiada — DDL e Restrições | `CREATE TABLE`, `DROP TABLE`, tipos de dados, `PRIMARY KEY`, `FOREIGN KEY` e demais constraints |
| Prática guiada — DELETE, UPDATE e JOIN | Atualização, exclusão e consulta com `JOIN` entre tabelas relacionadas |
| Atividade final — BDEmpregados | Modelagem, criação e consulta de um banco de dados completo (`Aula02_Exercicio2`) |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam os notebooks juntos
- Atividade final: aluno modela e constrói o banco de dados de forma autônoma, com apoio do instrutor

### Recursos

- Notebooks: `Aula02_Banco_Dados.ipynb`, `Aula02_Exercicio2.ipynb`
- Material de apoio: `BDEmpregados.pdf`
- Banco de dados: `clientes.db`
- Bibliotecas: `sqlite3`, `ipython-sql`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula |
| 0:05 – 0:15 | 10 min | **Prática guiada:** comando `INSERT`, com e sem lista de colunas |
| 0:15 – 0:30 | 15 min | **Prática guiada:** `CREATE TABLE`, `DROP TABLE`, tipos de dados e restrições (`PRIMARY KEY`, `FOREIGN KEY`, `NOT NULL`, `CHECK`, `UNIQUE`, `DEFAULT`) |
| 0:30 – 0:40 | 10 min | **Prática guiada:** comandos `DELETE` e `UPDATE` |
| 0:40 – 0:55 | 15 min | **Prática guiada:** integridade referencial e `SELECT` com `JOIN` |
| 0:55 – 1:10 | 15 min | **Atividade final (`Aula02_Exercicio2`):** modelar e criar as tabelas do BDEmpregados, inserir os registros (exercícios 1–2) |
| 1:10 – 1:25 | 15 min | **Atividade final (`Aula02_Exercicio2`):** consultas com `ORDER BY`, `JOIN` e `GROUP BY` (exercícios 3–10) |
| 1:25 – 1:30 | 5 min | Apresentação de soluções; encerramento do curso |

### Avaliação

O aluno entrega um notebook com:
- O banco de dados BDEmpregados criado a partir do zero, com tipos de dados e restrições apropriadas
- Todos os registros do modelo inseridos corretamente
- As 10 consultas do exercício final resolvidas, incluindo ao menos um `JOIN` e agregações com `GROUP BY`

---

## Visão Geral do Curso

| Aula | Módulo | Duração | Preparação (site) | Prática em sala |
|---|---|---|---|---|
| 1 | Fundamentos e Consultas SQL | 1h30min | O que é BD, tipos de BD, SQL, SELECT, WHERE, ORDER BY, GROUP BY, HAVING | `Aula01_Banco_Dados`, `Aula01_SQL_Island` |
| 2 | Manipulação de Dados, DDL e Modelagem | 1h30min | INSERT, DDL, restrições, DELETE, UPDATE, integridade referencial, JOIN | `Aula02_Banco_Dados`, `Aula02_Exercicio2` (atividade final) |
| **Total** | | **3h** | **10 conteúdos no site** | **2 práticas + 1 atividade final** |
