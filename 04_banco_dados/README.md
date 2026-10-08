# Banco de Dados com SQL

Curso introdutório de Banco de Dados voltado para jovens adolescentes do ensino médio. O conteúdo parte da contextualização de dados e IA no dia a dia, evolui pela linguagem SQL, modelagem de dados relacional e introdução a NoSQL com MongoDB.

**Carga horária:** 6h (4 aulas de 1h30min)
**Público-alvo:** Iniciantes — segundo grau
**Modelo:** Sala de aula invertida (teoria no site, prática em aula)
**Ferramenta:** Google Colab (sem instalação)
**SGBD:** SQLite e MongoDB (via mongita)

## Estrutura do Projeto

| Arquivo | Descrição |
|---|---|
| `PLANO_DE_AULA.md` | Plano de aula completo — objetivos, cronograma, metodologia e avaliação |
| `CONTEUDO.md` | Índice detalhado de todos os tópicos do curso |
| `aulas/` | Notebooks Jupyter com as aulas e exercícios práticos |

## Aulas

| # | Notebook | Tema |
|---|---|---|
| 01 | `Aula01_Banco_Dados.ipynb` | Dados e IA no dia a dia, como o ChatGPT usa banco de dados (RAG), crescimento dos dados (Data Never Sleeps), tipos de BD, introdução a SQL, `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY`, `HAVING`, exercícios com gabarito (`videogame_sales`) |
| P1 | `Aula01_SQL_Island.ipynb` | Prática gamificada — consultas SQL em banco temático de aldeias e habitantes |
| 02 | `Aula02_Banco_Dados.ipynb` | `INSERT`, `CREATE TABLE`, `DELETE`, `UPDATE`, Constraints, `JOIN` |
| P2 | `Aula02_Exercicio2.ipynb` | Atividade final — modelagem e criação do banco BDEmpregados |
| 03 | `Aula03_Banco_Dados.ipynb` | Modelagem de Dados — entidades, atributos, relacionamentos, diagrama ER, normalização (com diagramas visuais) |
| 04 | `Aula04_Banco_Dados.ipynb` | NoSQL e MongoDB — documentos JSON, CRUD com mongita, dados aninhados |

### Detalhamento — Aula 01

| Seção | Conteúdo |
|---|---|
| Dados e IA | Como TikTok, Spotify, Netflix e outras plataformas coletam e usam seus dados; o ciclo dado + algoritmo de recomendação |
| O Dilema das Redes | Clip do documentário *The Social Dilemma* (Netflix) como recurso de contextualização |
| ChatGPT e Banco de Dados | Explicação simplificada de RAG (*Retrieval-Augmented Generation*) — como a IA consulta bancos de dados para gerar respostas |
| Crescimento dos dados | Infográficos *Data Never Sleeps 12.0* (2024) e *AI Edition 2025* (Domo) |
| Tipos de BD | SQL (Relacional) vs. NoSQL (Chave-Valor, Grafo, Documentos, Colunar); principais SGBDs |
| Introdução a SQL | Categorias da linguagem (DQL, DML, DDL, DCL, DTL); conexão com SQLite via `sqlite3` e `%sql`/`%%sql` |
| Consultas SQL | `SELECT`, `WHERE` (operadores `=`, `<>`, `OR`, `AND`, `LIKE`, `IN`, `BETWEEN`), `ORDER BY`, `GROUP BY`, `HAVING` |
| Exercícios | Exercícios práticos com dataset `videogame_sales` — inclui resoluções detalhadas (gabarito) |

## Como Usar

1. Abra os notebooks no [Google Colab](https://colab.research.google.com/) ou no Jupyter Notebook
2. Os datasets são baixados automaticamente via `!wget` a partir do repositório [labeduc/datasets](https://github.com/labeduc/datasets)
3. Siga a ordem: **Aula 01 → Prática 01 → Aula 02 → Prática 02 → Aula 03 → Aula 04**

## Tecnologias

| Categoria | Tecnologias |
|---|---|
| **Linguagem** | Python 3, SQL |
| **Ambiente** | Google Colab, Jupyter Notebook, VS Code |
| **SGBD** | SQLite, MongoDB (mongita) |
| **Bibliotecas** | `sqlite3`, `ipython-sql`, `pandas`, `mongita` |
| **Bancos** | `clientes.db`, `videogame_sales.db`, `sql_island.db`, `game_social.db`, `bdempregados.db` |
