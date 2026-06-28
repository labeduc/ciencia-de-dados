# Plano de Aula — Visualização de Dados com Python

**Curso:** Visualização de Dados com Python  
**Carga horária total:** 7h30min (5 aulas de 1h30min)  
**Modalidade:** Online / Presencial  
**Público-alvo:** Iniciantes em Python e Ciência de Dados  
**Pré-requisito:** Nenhum — o curso parte do zero  
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)  
**Dataset principal:** `pokemons.csv` — 1.032 linhas × 44 colunas

---

## Aula 1 — Fundamentos

**Duração:** 1h30min  
**Notebooks de referência:** `aula-01`, `aula-02`, `aula-03`, `aula-04`

### Objetivo Geral

Apresentar o universo da Ciência de Dados e da Visualização, familiarizar o aluno com o Google Colab e ensinar como os dados são representados e organizados antes de serem visualizados.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Explicar o que é Ciência de Dados e o papel da Visualização no fluxo analítico
- Identificar o tipo de gráfico adequado para cada objetivo de comunicação
- Criar e executar um notebook no Google Colab
- Carregar um arquivo de dados local ou do Google Drive em um notebook
- Distinguir o formato Largo (Wide) do formato Longo (Long) e converter um no outro

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Teoria | Ciência de Dados, fluxo de trabalho, tipos de visualização × objetivo |
| Plataforma | Google Colab: células, execução, atalhos, Google Drive |
| Dados | Formatos tabular, Wide e Long; listas, dicionários, DataFrames e Series |
| Prática | Upload de dados, carregamento com script, transformação Wide → Long com `melt()` |

### Metodologia

- Exposição dialogada com slides (blocos de teoria)
- Demonstração ao vivo no Colab acompanhada pelo aluno
- Prática guiada: aluno executa as células junto com o instrutor
- Encerramento com recapitulação oral e espaço para dúvidas

### Recursos

- Google Colab (sem instalação)
- Notebook: `aula-01`, `aula-02`, `aula-03`, `aula-04`
- Arquivo de dados para upload (fornecido pelo instrutor)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Apresentação do curso, objetivos gerais e dinâmica das aulas |
| 0:05 – 0:20 | 15 min | **Teoria:** O que é Ciência de Dados; fluxo de trabalho; tipos de visualização e quando usar cada um |
| 0:20 – 0:35 | 15 min | **Google Colab:** criar notebook, células de texto e código, execução, atalhos, salvar no Drive |
| 0:35 – 0:50 | 15 min | **Formatos de dados:** tabular, Wide vs Long; listas e dicionários em Python; DataFrames e Series |
| 0:50 – 1:20 | 30 min | **Prática guiada (`aula-04`):** criar notebook no Colab, fazer upload de arquivo, carregar dados com script, transformar Wide → Long com `melt()` |
| 1:20 – 1:30 | 10 min | Recapitulação dos conceitos-chave e espaço para perguntas |

### Avaliação

Observação da participação durante a prática guiada. O aluno conclui a aula com um notebook funcional que carrega e transforma um conjunto de dados.

---

## Aula 2 — Manipulação de Dados com Pandas

**Duração:** 1h30min  
**Notebooks de referência:** `aula-05`, `pratica-aula-05`

### Objetivo Geral

Capacitar o aluno a usar a biblioteca Pandas para carregar, inspecionar, filtrar e agregar dados — habilidades fundamentais para qualquer análise antes da visualização.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Importar e usar a biblioteca Pandas em um notebook
- Carregar um arquivo CSV com `read_csv()` e entender a estrutura retornada
- Inspecionar um DataFrame com `head()`, `tail()`, `sample()`, `describe()`, `info()` e `shape`
- Acessar colunas e filtrar linhas por condições booleanas
- Agrupar dados com `groupby()` e calcular métricas de resumo

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Introdução | O que é Pandas e por que usá-lo; importação |
| Carregamento | `read_csv()`: parâmetros principais |
| Inspeção | `head()`, `tail()`, `sample()`, `describe()`, `info()`, `shape` |
| Acesso e filtro | Acesso a colunas, filtragem com condições booleanas, `iterrows()` |
| Agregação | `groupby()` com `mean()`, `count()`, `sum()` |
| Prática | 5 exercícios progressivos com o dataset de Pokémons |

### Metodologia

- Demonstração ao vivo de cada função, seguida de execução pelo aluno
- Progressão gradual: cada conceito usa o resultado do anterior
- Prática autônoma com exercícios numerados; instrutor circula para apoio

### Recursos

- Notebook: `aula-05`, `pratica-aula-05`
- Dataset: `pokemons.csv`
- Biblioteca: `pandas` (pré-instalada no Colab)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Recapitulação da Aula 1; o que é o Pandas e por que precisamos dele |
| 0:05 – 0:20 | 15 min | **Carregamento e estrutura:** `read_csv()`, o que é um DataFrame, colunas e tipos |
| 0:20 – 0:40 | 20 min | **Inspeção:** `head()`, `tail()`, `sample()`, `describe()`, `info()`, `shape` — demonstração e execução conjunta |
| 0:40 – 0:55 | 15 min | **Acesso e filtragem:** acesso a colunas, condições booleanas, `loc` e `iterrows()` |
| 0:55 – 1:10 | 15 min | **Agregação:** `groupby()` com exemplos práticos no dataset de Pokémons |
| 1:10 – 1:25 | 15 min | **Prática autônoma (`pratica-aula-05`):** exercícios 1 a 5 |
| 1:25 – 1:30 | 5 min | Correção comentada dos exercícios e perguntas |

### Avaliação

Resolução dos 5 exercícios da prática. O aluno demonstra autonomia ao carregar, filtrar e agregar o dataset sem assistência direta.

---

## Aula 3 — Visualizações Estáticas com Seaborn e Matplotlib

**Duração:** 1h30min  
**Notebooks de referência:** `aula-06`, `aula-07`, `aula-08`, `aula-09`, `aula-10`, `pratica-aula-06`, `pratica-aula-08`

### Objetivo Geral

Ensinar a criar os principais tipos de gráficos estáticos com Seaborn e Matplotlib, culminando na produção de visuais com aparência profissional aplicando boas práticas de design.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar gráficos de barras, linhas, áreas e pizza com Seaborn e Matplotlib
- Usar `hue` e `melt()` para representar múltiplas dimensões em um mesmo gráfico
- Construir um gráfico de dispersão e identificar outliers
- Montar um Gráfico de Quadrantes com linhas de referência
- Aplicar ajustes visuais profissionais: remoção de ruído, paleta de cores, valores nas barras, DPI e tamanho de figura

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Barras | `countplot()`, `barplot()`, barras agrupadas com `hue`, empilhadas |
| Linhas e Áreas | `lineplot()`, múltiplas séries, `stackplot()` |
| Dispersão | `scatterplot()`, `hue`, outliers, `apply()`, legenda externa |
| Quadrantes | Gráfico de Quadrantes, `axvline()`, `axhline()` |
| Pizza | `plt.pie()`, boas práticas, `explode`, percentuais |
| Polimento visual | `rcParams`, DPI, `spines`, valores nas barras, paleta de cores |

### Metodologia

- Demonstração comparativa: "gráfico básico → gráfico melhorado" para evidenciar o impacto do polimento visual
- Prática guiada nos blocos de barras e dispersão (os de maior impacto prático)
- Prática autônoma com exercícios selecionados das práticas 06 e 08

### Recursos

- Notebooks: `aula-06` a `aula-10`, `pratica-aula-06`, `pratica-aula-08`
- Dataset: `pokemons.csv`
- Bibliotecas: `seaborn`, `matplotlib`, `pandas`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Recapitulação da Aula 2; visão geral do módulo |
| 0:05 – 0:20 | 15 min | **Barras:** `countplot()`, `barplot()`, barras agrupadas com `hue` e empilhadas (`melt()`) |
| 0:20 – 0:30 | 10 min | **Linhas e Áreas:** `lineplot()` com múltiplas séries, `stackplot()` |
| 0:30 – 0:45 | 15 min | **Dispersão e Quadrantes:** `scatterplot()`, outliers, `axvline()`/`axhline()`, legenda externa |
| 0:45 – 0:55 | 10 min | **Pizza:** `plt.pie()`, quando usar, `explode`, percentuais e boas práticas |
| 0:55 – 1:10 | 15 min | **Polimento visual:** `rcParams`, DPI, remoção de `spines`, valores nas barras, paleta personalizada |
| 1:10 – 1:25 | 15 min | **Prática autônoma:** exercícios selecionados de `pratica-aula-06` (ex. 1-3) e `pratica-aula-08` (ex. 1-2) |
| 1:25 – 1:30 | 5 min | Correção comentada e perguntas |

### Avaliação

O aluno produz ao menos dois gráficos distintos com dataset de Pokémons, aplicando customização visual (título, cores, sem ruído visual).

---

## Aula 4 — Visualizações Avançadas e Bancos de Dados

**Duração:** 1h30min  
**Notebooks de referência:** `aula-11`, `aula-12`, `aula-13`, `aula-14`, `pratica-aula-09-14`

### Objetivo Geral

Ampliar o repertório de visualizações com gráficos especializados (redes, Sankey, wordcloud) e integrar Python com bancos de dados SQL usando DuckDB diretamente no notebook.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar e personalizar um mapa de rede com NetworkX
- Construir um Diagrama de Sankey para representar fluxo entre categorias
- Gerar uma nuvem de palavras com frequência de termos e máscara de imagem
- Criar um banco de dados em memória com DuckDB e consultá-lo com SQL no notebook
- Resolver exercícios de consolidação que combinam todos esses tipos de gráfico

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Rede | NetworkX: nodos, arestas, pesos, `nx.draw()`, personalização |
| Sankey | Plotly Graph Objects: source/target/value, cores e rótulos |
| Wordcloud | `WordCloud`, frequência de termos, máscara com PIL |
| Banco de Dados | DuckDB, `JupySQL`, `%sql` / `%%sql`, fluxo carregar → consultar → visualizar |
| Prática | 8 exercícios de consolidação (Aulas 09 a 14) |

### Metodologia

- Apresentação de cada gráfico com contexto de uso real ("quando você usaria isso?")
- Demonstração ao vivo com execução conjunta pelo aluno
- Prática autônoma nos exercícios de consolidação; aluno escolhe ao menos 3 para resolver

### Recursos

- Notebooks: `aula-11`, `aula-12`, `aula-13`, `aula-14`, `pratica-aula-09-14`
- Dataset: `pokemons.csv`
- Bibliotecas: `networkx`, `plotly`, `wordcloud`, `PIL`, `duckdb`, `jupysql`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Recapitulação da Aula 3; visão geral do módulo |
| 0:05 – 0:20 | 15 min | **Mapas de Rede:** NetworkX, nodos e arestas, pesos, personalização visual |
| 0:20 – 0:35 | 15 min | **Sankey:** conceito, preparação dos dados (source/target/value), plotagem com Plotly |
| 0:35 – 0:50 | 15 min | **Wordcloud:** frequência de termos, geração básica, máscara de imagem personalizada |
| 0:50 – 1:05 | 15 min | **Bancos de Dados:** DuckDB + JupySQL, criação de tabela a partir de DataFrame, consultas SQL no notebook |
| 1:05 – 1:25 | 20 min | **Prática autônoma (`pratica-aula-09-14`):** aluno escolhe e resolve ao menos 3 dos 8 exercícios |
| 1:25 – 1:30 | 5 min | Correção dos exercícios selecionados e perguntas |

### Avaliação

O aluno demonstra uso de ao menos três tipos de gráfico avançado e realiza uma consulta SQL funcional sobre o dataset via DuckDB.

---

## Aula 5 — Gráficos Interativos com Plotly

**Duração:** 1h30min  
**Notebooks de referência:** `aula-15`, `aula-16`

### Objetivo Geral

Ensinar a criar gráficos interativos com Plotly Express e a configurar visualizações completas e prontas para apresentação usando o objeto `Figure` do Plotly Graph Objects.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar os principais tipos de gráfico com Plotly Express (`bar`, `line`, `scatter`, `pie`)
- Configurar parâmetros de interatividade: hover, zoom e filtro por legenda
- Usar o objeto `Figure` para controlar título, legenda, eixos, labels e tooltips
- Produzir um gráfico completo, sem background e com tooltip personalizado, pronto para uso em apresentação

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Plotly Express | `px.bar()`, `px.line()`, `px.scatter()`, `px.pie()`, parâmetros `color`, `title`, `labels`, `hover_data` |
| Objeto Figure | Estrutura data + layout; título, legenda, eixos, remoção de background |
| Labels e Tooltips | `text`, `textposition`, `hovertemplate` personalizado |
| Atividade final | Gráfico completo do zero com o dataset de Pokémons |

### Metodologia

- Demonstração comparativa entre Seaborn (estático) e Plotly (interativo) para evidenciar a diferença
- Live coding: instrutor constrói o gráfico final ao vivo camada por camada enquanto explica cada decisão
- Atividade final autônoma: o aluno escolhe um tipo de gráfico e o constrói do zero aplicando todas as configurações aprendidas

### Recursos

- Notebooks: `aula-15`, `aula-16`
- Dataset: `pokemons.csv`
- Bibliotecas: `plotly.express`, `plotly.graph_objects`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Recapitulação da Aula 4; apresentação do módulo final |
| 0:05 – 0:10 | 5 min | Comparação entre gráficos estáticos e interativos: quando usar cada abordagem |
| 0:10 – 0:30 | 20 min | **Plotly Express:** `px.bar()`, `px.line()`, `px.scatter()`, `px.pie()` — demonstração e execução conjunta |
| 0:30 – 1:00 | 30 min | **Objeto Figure camada por camada:** título → legenda → eixos → remoção de background → labels → tooltip personalizado |
| 1:00 – 1:25 | 25 min | **Atividade final:** aluno escolhe um tipo de gráfico e constrói um visual completo com o dataset de Pokémons, aplicando todas as configurações |
| 1:25 – 1:30 | 5 min | Apresentação de dois ou três trabalhos finais; encerramento do curso e indicação de próximos passos |

### Avaliação

O aluno entrega um notebook com um gráfico Plotly completo: tipo de gráfico definido, título, legenda posicionada, eixos ajustados e tooltip personalizado. O gráfico deve ser legível e comunicar claramente a informação escolhida.

---

## Visão Geral do Curso

| Aula | Módulo | Duração | Notebooks | Prática |
|---|---|---|---|---|
| 1 | Fundamentos | 1h30min | aula-01 a aula-04 | Sim (`aula-04`) |
| 2 | Pandas | 1h30min | aula-05 | Sim (`pratica-aula-05`) |
| 3 | Seaborn e Matplotlib | 1h30min | aula-06 a aula-10 | Sim (`pratica-aula-06`, `pratica-aula-08`) |
| 4 | Visualizações Avançadas | 1h30min | aula-11 a aula-14 | Sim (`pratica-aula-09-14`) |
| 5 | Plotly Interativo | 1h30min | aula-15 e aula-16 | Sim (atividade final) |
| **Total** | | **7h30min** | **20 notebooks** | **4 práticas + 1 atividade final** |
