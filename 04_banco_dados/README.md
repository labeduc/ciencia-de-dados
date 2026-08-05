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
| 01 | `Aula01_Banco_Dados.ipynb` | Dados e IA, Banco de Dados, `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY`, `HAVING` |
| P1 | `Aula01_SQL_Island.ipynb` | Prática gamificada — consultas SQL em banco temático de aldeias e habitantes |
| 02 | `Aula02_Banco_Dados.ipynb` | `INSERT`, `CREATE TABLE`, `DELETE`, `UPDATE`, Constraints, `JOIN` |
| P2 | `Aula02_Exercicio2.ipynb` | Atividade final — modelagem e criação do banco BDEmpregados |
| 03 | `Aula03_Banco_Dados.ipynb` | Modelagem de Dados — entidades, atributos, relacionamentos, diagrama ER, normalização |
| 04 | `Aula04_Banco_Dados.ipynb` | NoSQL e MongoDB — documentos JSON, CRUD com mongita, dados aninhados |

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
