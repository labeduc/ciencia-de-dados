# Plano de Aula — Banco de Dados com SQL

**Curso:** Banco de Dados com SQL e NoSQL
**Carga horária total:** 6h (4 aulas de 1h30min)
**Modalidade:** Online / Presencial
**Público-alvo:** Iniciantes em Banco de Dados e Ciência de Dados
**Pré-requisito:** Nenhum — o curso parte do zero
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)
**SGBD utilizado:** SQLite (via `sqlite3` e extensão `%sql` / `%%sql`) e MongoDB (via `mongita`)
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
| 1:25 – 1:30 | 5 min | Apresentação de soluções; encerramento |

### Avaliação

O aluno entrega um notebook com:
- O banco de dados BDEmpregados criado a partir do zero, com tipos de dados e restrições apropriadas
- Todos os registros do modelo inseridos corretamente
- As 10 consultas do exercício final resolvidas, incluindo ao menos um `JOIN` e agregações com `GROUP BY`

---

## Aula 3 — Modelagem de Dados

**Duração:** 1h30min
**Notebook de referência:** `Aula03_Banco_Dados.ipynb`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir os seguintes conteúdos **antes** desta sessão:

| # | Conteúdo no site | Assunto |
|---|---|---|
| 11 | O que é modelagem de dados | Conceito, importância e relação com IA |
| 12 | Entidades, atributos e relacionamentos | Os 3 conceitos fundamentais da modelagem |
| 13 | Tipos de relacionamento | 1:1, 1:N e N:N — tabela intermediária |
| 14 | Níveis de modelagem | Conceitual, Lógico e Físico |
| 15 | Diagrama Entidade-Relacionamento (ER) | Elementos do diagrama e leitura |
| 16 | Normalização | Redundância, anomalias e formas normais (visão geral) |

### Objetivo Geral

Consolidar, por meio de prática guiada e exercícios, os conceitos de modelagem de dados relacional — das entidades e relacionamentos ao `CREATE TABLE` — conectando a importância de dados bem estruturados para IA.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Identificar entidades, atributos e relacionamentos a partir de um cenário do mundo real
- Diferenciar os tipos de relacionamento: 1:1, 1:N e N:N
- Reconhecer a necessidade de tabela intermediária em relacionamentos N:N
- Distinguir os 3 níveis de modelagem (Conceitual, Lógico e Físico)
- Ler e interpretar um Diagrama Entidade-Relacionamento (ER)
- Criar tabelas com chaves primárias, estrangeiras e constraints a partir de um modelo lógico
- Compreender normalização e os problemas de redundância
- Relacionar modelagem de dados com qualidade de dados para IA

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula |
| Contextualização | Por que modelagem importa na era da IA — dados organizados como base para recomendações e RAG |
| Conceitos fundamentais | Entidade, Atributo e Relacionamento (com exemplos: Spotify, Steam, Instagram) |
| Tipos de relacionamento | 1:1, 1:N, N:N — tabela intermediária |
| Níveis de modelagem | Conceitual → Lógico → Físico |
| Diagrama ER | Elementos do diagrama, exemplo Spotify simplificado |
| Prática guiada — Rede Social de Games | Modelagem completa: conceitual → lógico → `CREATE TABLE` (Jogador, Jogo, Conquista, Partida) |
| Prática guiada — Inserção e consultas | Populando o banco e executando JOINs |
| Normalização | Comparação: tabela única vs. normalizada |
| Boas práticas | 8 regras de ouro de modelagem |
| Exercícios | 5 consultas + 1 desafio (criar tabela N:N Conquista_Jogador) |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam o notebook juntos, construindo o banco do zero
- Exercícios autônomos: aluno resolve consultas e desafio de modelagem, com apoio do instrutor

### Recursos

- Notebook: `Aula03_Banco_Dados.ipynb`
- Banco de dados: `game_social.db` (criado durante a aula)
- Bibliotecas: `sqlite3`, `ipython-sql`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula |
| 0:05 – 0:15 | 10 min | **Contextualização:** por que modelagem importa — conexão com IA, exemplos do dia a dia |
| 0:15 – 0:30 | 15 min | **Conceitos:** entidade, atributo, relacionamento; tipos de relacionamento (1:1, 1:N, N:N) |
| 0:30 – 0:40 | 10 min | **Níveis de modelagem e Diagrama ER:** conceitual → lógico → físico; leitura de diagrama |
| 0:40 – 1:00 | 20 min | **Prática guiada:** modelagem da Rede Social de Games — do conceitual ao `CREATE TABLE`, inserção de dados e consultas com JOIN |
| 1:00 – 1:10 | 10 min | **Normalização e boas práticas:** comparação tabela única vs. normalizada, 8 regras de ouro |
| 1:10 – 1:25 | 15 min | **Exercícios:** consultas 1–5 + desafio (criar tabela Conquista_Jogador) |
| 1:25 – 1:30 | 5 min | Revisão de soluções; encerramento |

### Avaliação

O aluno conclui a aula com um notebook funcional contendo:
- Um banco de dados (`game_social.db`) modelado e criado do zero com entidades, relacionamentos e constraints
- Consultas com JOIN sobre o banco modelado
- Exercícios resolvidos, incluindo o desafio de criar uma nova tabela N:N

---

## Aula 4 — NoSQL e MongoDB

**Duração:** 1h30min
**Notebook de referência:** `Aula04_Banco_Dados.ipynb`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir os seguintes conteúdos **antes** desta sessão:

| # | Conteúdo no site | Assunto |
|---|---|---|
| 17 | SQL vs NoSQL | Diferenças, vantagens e quando usar cada um |
| 18 | Tipos de banco NoSQL | Documentos, Chave-Valor, Colunar e Grafos |
| 19 | MongoDB — conceitos | Coleções, documentos, campos, JSON/BSON |
| 20 | CRUD no MongoDB | `insert`, `find`, `update`, `delete` e operadores |

### Objetivo Geral

Apresentar bancos de dados NoSQL com foco em MongoDB, usando a biblioteca mongita para prática guiada de CRUD com documentos JSON, comparando com o modelo relacional visto nas aulas anteriores.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Diferenciar bancos SQL e NoSQL e identificar quando usar cada um
- Conhecer os 4 tipos de banco NoSQL (Documentos, Chave-Valor, Colunar, Grafos)
- Criar bancos e coleções no MongoDB usando mongita
- Inserir documentos com `insert_one()` e `insert_many()`
- Consultar documentos com `find()`, `find_one()` e operadores de filtro (`$gt`, `$lt`, `$in`, etc.)
- Buscar dentro de listas e subdocumentos (dot notation)
- Atualizar documentos com `update_one()`, `update_many()` e operadores (`$set`, `$inc`, `$push`, `$pull`)
- Deletar documentos com `delete_one()` e `delete_many()`
- Comparar operações equivalentes em SQL e MongoDB
- Relacionar o uso de NoSQL com aplicações de IA (RAG, cache, busca vetorial)

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula |
| SQL vs NoSQL | Diferenças, vantagens, quem usa o quê (Spotify, Steam, ChatGPT) |
| Tipos de NoSQL | Documentos, Chave-Valor, Colunar, Grafos |
| MongoDB — vocabulário | Coleção, documento, campo; equivalência com SQL |
| Prática guiada — Setup | Instalação do mongita, conexão ao banco em memória |
| Prática guiada — INSERT | `insert_one()` com documento aninhado, `insert_many()` com campos variáveis |
| Prática guiada — FIND | `find()`, `find_one()`, operadores de filtro, busca em listas e subdocumentos |
| Prática guiada — UPDATE | `$set`, `$inc`, `$push`, `$pull`, `update_one()`, `update_many()` |
| Prática guiada — DELETE | `delete_one()`, `delete_many()` |
| Coleção de jogos | Inserção e consultas avançadas (busca em listas, dot notation, contagem) |
| Comparação SQL vs MongoDB | Tabela lado a lado de operações equivalentes |
| Quando usar SQL vs NoSQL | Critérios de decisão + uso na IA moderna |
| Exercícios | 6 exercícios + 1 desafio (criar coleção de partidas) |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam o notebook juntos, explorando CRUD no MongoDB
- Exercícios autônomos: aluno resolve consultas e desafio de criação de coleção, com apoio do instrutor

### Recursos

- Notebook: `Aula04_Banco_Dados.ipynb`
- Banco de dados: `game_social_nosql` (em memória, via mongita)
- Bibliotecas: `mongita`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula |
| 0:05 – 0:15 | 10 min | **Contextualização:** SQL vs NoSQL, tipos de NoSQL, quem usa o quê |
| 0:15 – 0:25 | 10 min | **MongoDB conceitos:** coleção, documento, campo; vocabulário SQL → MongoDB |
| 0:25 – 0:35 | 10 min | **Prática guiada:** setup com mongita, `insert_one()` com documento aninhado |
| 0:35 – 0:45 | 10 min | **Prática guiada:** `insert_many()` com campos variáveis entre documentos |
| 0:45 – 1:00 | 15 min | **Prática guiada:** `find()`, `find_one()`, operadores, busca em listas e subdocumentos |
| 1:00 – 1:10 | 10 min | **Prática guiada:** `update_one()`, `update_many()`, `delete_one()`; comparação SQL vs MongoDB |
| 1:10 – 1:25 | 15 min | **Exercícios:** 6 consultas + desafio (criar coleção de partidas) |
| 1:25 – 1:30 | 5 min | Revisão de soluções; encerramento do curso |

### Avaliação

O aluno conclui a aula com um notebook funcional contendo:
- Um banco NoSQL (`game_social_nosql`) com coleções de jogadores e jogos
- Operações de CRUD executadas com mongita
- Exercícios resolvidos, incluindo o desafio de criar uma nova coleção de partidas

---

## Visão Geral do Curso

| Aula | Módulo | Duração | Preparação (site) | Prática em sala |
|---|---|---|---|---|
| 1 | Fundamentos e Consultas SQL | 1h30min | O que é BD, tipos de BD, SQL, SELECT, WHERE, ORDER BY, GROUP BY, HAVING | `Aula01_Banco_Dados`, `Aula01_SQL_Island` |
| 2 | Manipulação de Dados, DDL e Relacionamentos | 1h30min | INSERT, DDL, restrições, DELETE, UPDATE, integridade referencial, JOIN | `Aula02_Banco_Dados`, `Aula02_Exercicio2` |
| 3 | Modelagem de Dados | 1h30min | Modelagem, entidades, relacionamentos, diagrama ER, normalização | `Aula03_Banco_Dados` |
| 4 | NoSQL e MongoDB | 1h30min | SQL vs NoSQL, tipos de NoSQL, MongoDB, CRUD | `Aula04_Banco_Dados` |
| **Total** | | **6h** | **20 conteúdos no site** | **4 práticas + 1 atividade final + 2 desafios** |
