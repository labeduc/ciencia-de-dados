# Repositório de Conteúdo — WVCode Blog

## O que é este repositório

Este repositório contém as aulas do módulo de Visualização de Dados da trilha de Ciência de Dados do LabEduc. O foco principal é **Ciência de Dados e Visualização de Dados com Python**, voltado para iniciantes e profissionais que desejam aprofundar seus conhecimentos em análise de dados programática.

Cada pasta representa uma aula publicada. O conteúdo está no formato **Jupyter Notebook (`.ipynb`)**, compatível com Google Colab, Jupyter e VS Code.

O conjunto de dados usado na maior parte dos exemplos é o dataset de **Pokémons** (`pokemons.csv`), com 1032 entradas e 44 colunas.

---

## Séries de Conteúdo

O repositório está organizado em quatro séries principais mais posts avulsos:

| Série | Pasta | Descrição |
|---|---|---|
| **Visualização de Dados com Python** | `visualizacao/` | Curso completo do zero: teoria, ferramentas, bibliotecas e boas práticas |
| **Testes em Dados** | `testes/` | Validação e qualidade de dados com Pandas |
| **Posts Avulsos** | `extras/` | Integrações com IA generativa, Power BI e outras ferramentas |

---

## Índice Ordenado

### Série: Visualização de Dados com Python

Curso estruturado para quem está começando em Python e Ciência de Dados. Ensina desde a teoria de visualização até a criação de gráficos profissionais e interativos.

#### Aulas

| Pasta | Título | Tópicos Principais |
|---|---|---|
| `visualizacao/aula-01/` | **Aula 01 — Teoria de Visualização de Dados** | Ciclo de vida de dados, tipos de gráficos, ferramentas |
| `visualizacao/aula-02/` | **Aula 02 — Google Colab** | Células de código e texto, carregamento de dados, Google Drive |
| `visualizacao/aula-03/` | **Aula 03 — Formatos de Dados** | Formato largo vs. longo, DataFrames, Series |
| `visualizacao/aula-04/` | **Aula 04 — Prática: Aulas 2 e 3** | Upload de arquivos, transformação largo→longo, bibliotecas externas |
| `visualizacao/aula-05/` | **Aula 05 — Pandas** | `read_csv`, `head`, `tail`, `sample`, `describe`, `info`, filtragem, `groupby` |
| `visualizacao/aula-06/` | **Aula 06 — Seaborn: Gráficos de Barras** | `countplot`, `barplot`, `melt`, barras agrupadas e empilhadas |
| `visualizacao/aula-07/` | **Aula 07 — Seaborn: Linhas e Áreas** | `lineplot`, múltiplas séries, `stackplot` via MatplotLib |
| `visualizacao/aula-08/` | **Aula 08 — Dispersão e Quadrantes** | `scatterplot`, outliers, `apply`, legenda externa, Quadrante Mágico |
| `visualizacao/aula-09/` | **Aula 09 — Gráfico de Pizza** | Quando usar pizza, boas práticas, `plt.pie` |
| `visualizacao/aula-10/` | **Aula 10 — Melhorando seus Visuais** | `rcParams`, DPI, spines, paleta de cores, valores nas barras |
| `visualizacao/aula-11/` | **Aula 11 — Mapas de Rede** | NetworkX, nodos, vértices com peso |
| `visualizacao/aula-12/` | **Aula 12 — Sankey Charts** | Diagrama de Sankey com Plotly, relação entre categorias |
| `visualizacao/aula-13/` | **Aula 13 — Wordclouds** | Biblioteca wordcloud, frequência de termos, máscara de imagem |
| `visualizacao/aula-14/` | **Aula 14 — Pandas e Bancos de Dados** | DuckDB, JupySQL, SQL e Python em notebooks |
| `visualizacao/aula-15/` | **Aula 15 — Gráficos Interativos** | Plotly Express: barras, linhas, dispersão e pizza interativos |
| `visualizacao/aula-16/` | **Aula 16 — Visualizações Efetivas** | Plotly Figure, título, legenda, eixos, labels, tooltips |

#### Práticas

| Pasta | Título | Aula de Referência |
|---|---|---|
| `visualizacao/pratica-aula-05/` | **Prática 05 — Pandas** | Aula 05 |
| `visualizacao/pratica-aula-06/` | **Prática 06 — Iniciando com Seaborn** | Aula 06 |
| `visualizacao/pratica-aula-08/` | **Prática 08 — Dispersão e Quadrantes** | Aula 08 |
| `visualizacao/pratica-aula-09-14/` | **Prática 09 a 14 — Consolidação** | Aulas 09 a 14 |

---

### Série: Testes em Dados

Validação e garantia de qualidade de conjuntos de dados.

| Pasta | Título | Tópicos Principais |
|---|---|---|
| `testes/testes-001/` | **Teste em Dados — Básico** | Validações com Pandas, `assert`, Sweetviz, D-Tale |

---

### Posts Avulsos

Posts independentes sobre integrações e ferramentas especiais.

| Pasta | Título | Tópicos Principais |
|---|---|---|
| `extras/pandasai/` | **Pandas AI — Converse com seu DataFrame** | Interface conversacional com GPT/OpenAI sobre DataFrames |
| `extras/powerbiclient/` | **Power BI no Jupyter!** | Biblioteca `powerbiclient`, embeddings de relatórios |
| `extras/classif-texto/` | **Classificação de Texto com a API da OpenAI** | NLP sem dados de treino, scraping, categorização com GPT |

---

## Tecnologias e Bibliotecas Abordadas

| Categoria | Tecnologias |
|---|---|
| **Linguagem** | Python 3.12 |
| **Ambiente** | Google Colab, Jupyter Notebook, VS Code |
| **Manipulação de Dados** | Pandas, NumPy, csv (stdlib) |
| **Visualização Estática** | Seaborn, MatplotLib |
| **Visualização Interativa** | Plotly Express, Plotly Graph Objects |
| **Grafos e Redes** | NetworkX |
| **Nuvem de Palavras** | WordCloud, PIL |
| **Bancos de Dados** | DuckDB, JupySQL, SQLAlchemy |
| **Transformação de Dados** | dbt-core (PostgreSQL) |
| **EDA / Qualidade** | Sweetviz, D-Tale, jupyter-summarytools |
| **Inteligência Artificial** | OpenAI API (GPT), PandasAI |
| **Power BI** | powerbiclient |
| **Scraping** | BeautifulSoup4, requests-html |

---

## Dataset Principal

**`pokemons.csv`** — Presente em: `visualizacao/aula-04/` a `aula-16/` e todos os notebooks de prática.

- 1032 linhas × 44 colunas
- Colunas principais: `Number`, `Name`, `Type 1`, `Type 2`, `HP`, `Att`, `Def`, `Spa`, `Spd`, `Spe`, `BST`, `Generation`, `Legendary`, resistências contra cada tipo, `Height`, `Weight`, `BMI`

---

## Estatísticas do Repositório

| Item | Quantidade |
|---|---|
| Total de notebooks (`.ipynb`) | 24 |
| Notebooks de aula | 20 |
| Notebooks de prática | 4 |
| Arquivos Quarto (`.qmd`) | 1 |
| Séries de conteúdo | 3 |
| Dependências Python (`requirements.txt`) | 20 pacotes |
