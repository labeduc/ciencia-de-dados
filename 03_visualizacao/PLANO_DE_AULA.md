# Plano de Aula — Visualização de Dados com Python

**Curso:** Visualização de Dados com Python  
**Carga horária total:** 3h (2 aulas de 1h30min)  
**Modalidade:** Online / Presencial  
**Público-alvo:** Iniciantes em Python e Ciência de Dados  
**Pré-requisito:** Nenhum — o curso parte do zero  
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)  
**Dataset principal:** `pokemons.csv` — 1.032 linhas × 44 colunas  
**Modelo de aprendizagem:** Sala de aula invertida — o conteúdo teórico é consumido pelo aluno no site antes da aula; o tempo presencial é dedicado a prática, dúvidas e consolidação.

---

> **Importante para os alunos:** Cada aula pressupõe que você já acessou o website do curso e consumiu as aulas indicadas na seção **Preparação** antes de comparecer à sessão presencial. Chegar sem ter feito essa preparação compromete seu aproveitamento, pois o tempo em sala será dedicado à prática, não à exposição teórica.

---

## Aula 1 — Fundamentos, Manipulação de Dados e Primeiros Gráficos

**Duração:** 1h30min  
**Notebooks de referência:** `aula-01`, `aula-02`, `aula-03`, `aula-04`, `aula-05`, `aula-06`, `aula-07`, `pratica-aula-05`, `pratica-aula-06`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir as seguintes aulas **antes** desta sessão:

| # | Aula no site | Conteúdo |
|---|---|---|
| 1 | Aula 01 | O que é Ciência de Dados e Visualização |
| 2 | Aula 02 | Tipos de gráficos e quando usar cada um |
| 3 | Aula 03 | Google Colab: células, execução, atalhos |
| 4 | Aula 04 | Formatos de dados: tabular, Wide e Long; `melt()` |
| 5 | Aula 05 | Pandas: carregamento, inspeção e agregação de dados |
| 6 | Aula 06 | Gráficos de barras com Seaborn |
| 7 | Aula 07 | Gráficos de linha e área |

### Objetivo Geral

Consolidar, por meio de prática guiada, os conceitos de organização e manipulação de dados com Pandas e dar os primeiros passos na criação de gráficos estáticos com Seaborn e Matplotlib.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar e executar um notebook no Google Colab com carregamento de dados reais
- Transformar dados de formato Wide para Long com `melt()`
- Inspecionar um DataFrame com `head()`, `tail()`, `describe()`, `info()` e `shape`
- Filtrar linhas por condições booleanas e agrupar dados com `groupby()`
- Criar gráficos de barras simples, agrupadas e empilhadas com Seaborn
- Criar gráficos de linha com múltiplas séries e gráficos de área com Matplotlib

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (aulas 01–07) |
| Prática guiada — Pandas | Upload de arquivo, carregamento, inspeção, filtro e agregação |
| Prática autônoma — Pandas | Exercícios progressivos com o dataset de Pokémons |
| Prática guiada — Barras | `countplot()`, `barplot()`, barras agrupadas com `hue` e empilhadas |
| Prática guiada — Linhas e Áreas | `lineplot()` com múltiplas séries, `stackplot()` |
| Prática autônoma — Visualização | Exercícios selecionados de `pratica-aula-06` |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo consumido no site (máx. 5 min)
- Prática guiada: instrutor e aluno executam os notebooks juntos
- Prática autônoma com exercícios; instrutor circula para apoio

### Recursos

- Google Colab (sem instalação)
- Notebooks: `aula-04`, `aula-05`, `aula-06`, `aula-07`, `pratica-aula-05`, `pratica-aula-06`
- Dataset: `pokemons.csv`
- Bibliotecas: `pandas`, `seaborn`, `matplotlib` (pré-instaladas no Colab)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula (aulas 01–07) |
| 0:05 – 0:15 | 10 min | **Prática guiada (`aula-04`):** criar notebook no Colab, fazer upload de arquivo, carregar dados com Pandas, transformar Wide → Long com `melt()` |
| 0:15 – 0:35 | 20 min | **Prática guiada (`aula-05`):** inspeção com `head()`, `describe()`, `info()`, `shape`; filtro por condições booleanas; `groupby()` com métricas de resumo |
| 0:35 – 0:50 | 15 min | **Prática autônoma (`pratica-aula-05`):** exercícios 1 a 3 |
| 0:50 – 1:00 | 10 min | **Prática guiada (`aula-06`):** `countplot()`, `barplot()`, barras agrupadas com `hue` e empilhadas com `melt()` |
| 1:00 – 1:10 | 10 min | **Prática guiada (`aula-07`):** `lineplot()` com múltiplas séries, `stackplot()` |
| 1:10 – 1:25 | 15 min | **Prática autônoma (`pratica-aula-06`):** exercícios selecionados |
| 1:25 – 1:30 | 5 min | Correção comentada e perguntas |

### Avaliação

O aluno conclui a aula com um notebook funcional que carrega, manipula e visualiza o dataset de Pokémons, produzindo ao menos um gráfico de barras e um de linha com customização básica.

---

## Aula 2 — Visualizações Estáticas, Avançadas e Interativas

**Duração:** 1h30min  
**Notebooks de referência:** `aula-08` a `aula-16`, `pratica-aula-08`, `pratica-aula-09-14`

### Preparação (antes da aula)

O aluno deve acessar o website do curso e consumir as seguintes aulas **antes** desta sessão:

| # | Aula no site | Conteúdo |
|---|---|---|
| 8 | Aula 08 | Gráfico de dispersão e Quadrantes |
| 9 | Aula 09 | Gráfico de pizza e polimento visual |
| 10 | Aula 10 | Boas práticas de design (`rcParams`, DPI, `spines`) |
| 11 | Aula 11 | Mapas de rede com NetworkX |
| 12 | Aula 12 | Diagrama de Sankey com Plotly |
| 13 | Aula 13 | Nuvem de palavras (WordCloud) |
| 14 | Aula 14 | Bancos de dados com DuckDB e JupySQL |
| 15 | Aula 15 | Gráficos interativos com Plotly Express |
| 16 | Aula 16 | Objeto Figure: controle total do layout |

### Objetivo Geral

Consolidar, por meio de prática guiada e atividade final, a criação de gráficos estáticos avançados, visualizações especializadas e gráficos interativos com Plotly.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar gráficos de dispersão, quadrantes e pizza com polimento visual profissional
- Produzir ao menos um gráfico avançado (rede, Sankey ou wordcloud)
- Criar gráficos interativos com Plotly Express e configurar o objeto `Figure`
- Construir um visual completo e pronto para apresentação com tooltip personalizado

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (aulas 08–16) |
| Prática estática | Exercícios selecionados de `pratica-aula-08` (dispersão, quadrantes, pizza, polimento) |
| Prática avançada | Ao menos 2 exercícios de `pratica-aula-09-14` (rede, Sankey, wordcloud ou DuckDB) |
| Atividade final | Gráfico Plotly completo construído do zero pelo aluno |

### Metodologia

- Abertura com roda de dúvidas sobre o conteúdo pré-aula (máx. 5 min)
- Prática guiada rápida nos tipos de gráfico mais complexos
- Prática autônoma com exercícios; aluno escolhe ao menos dois gráficos avançados
- Atividade final: live coding do instrutor + construção autônoma pelo aluno

### Recursos

- Notebooks: `aula-08` a `aula-16`, `pratica-aula-08`, `pratica-aula-09-14`
- Dataset: `pokemons.csv`
- Bibliotecas: `seaborn`, `matplotlib`, `networkx`, `plotly`, `wordcloud`, `duckdb`, `jupysql`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula (aulas 08–16) |
| 0:05 – 0:25 | 20 min | **Prática guiada (`pratica-aula-08`):** dispersão, Gráfico de Quadrantes, pizza e polimento visual (`rcParams`, DPI, `spines`) |
| 0:25 – 0:50 | 25 min | **Prática autônoma (`pratica-aula-09-14`):** aluno escolhe e resolve ao menos 2 dos 8 exercícios (rede, Sankey, wordcloud ou DuckDB) |
| 0:50 – 1:05 | 15 min | **Live coding do instrutor:** construção camada a camada de um gráfico Plotly completo (título, legenda, eixos, background, tooltip) |
| 1:05 – 1:25 | 20 min | **Atividade final:** aluno escolhe um tipo de gráfico e constrói um visual Plotly completo com o dataset de Pokémons |
| 1:25 – 1:30 | 5 min | Apresentação de dois ou três trabalhos; encerramento do curso e próximos passos |

### Avaliação

O aluno entrega um notebook com:
- Ao menos dois gráficos estáticos com customização visual
- Ao menos um gráfico avançado (rede, Sankey, wordcloud ou consulta DuckDB)
- Um gráfico Plotly completo: tipo definido, título, legenda posicionada, eixos ajustados e tooltip personalizado

---

## Visão Geral do Curso

| Aula | Módulo | Duração | Preparação (site) | Prática em sala |
|---|---|---|---|---|
| 1 | Fundamentos, Pandas e Primeiros Gráficos | 1h30min | Aulas 01 a 07 | `aula-04`, `pratica-aula-05`, `pratica-aula-06` |
| 2 | Visualizações Avançadas e Interativas | 1h30min | Aulas 08 a 16 | `pratica-aula-08`, `pratica-aula-09-14`, atividade final |
| **Total** | | **3h** | **16 aulas no site** | **4 práticas + 1 atividade final** |
