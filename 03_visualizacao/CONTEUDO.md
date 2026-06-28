# Visualização de Dados com Python

## Sobre o Curso

Curso completo de Visualização de Dados com Python voltado para iniciantes e profissionais que desejam aprofundar conhecimentos em análise de dados programática. O conteúdo parte da teoria de visualização e evolui até a criação de gráficos profissionais e interativos.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Jupyter e VS Code.  
**Dataset principal:** `pokemons.csv` — 1.032 linhas × 44 colunas (usado da Aula 05 em diante).  
**Total de aulas:** 16 aulas teóricas + 4 práticas

---

## Módulo 1 — Fundamentos

Objetivo: construir a base conceitual e operacional necessária para começar a trabalhar com dados em Python.

---

### Aula 01 — Teoria de Visualização de Dados

**Pasta:** `aula-01/`

Introdução à Ciência de Dados e ao papel da Visualização dentro do fluxo de trabalho analítico.

**Tópicos:**
- O que é Ciência de Dados e por que ela importa
- O fluxo de trabalho do Cientista de Dados
- O que é Visualização de Dados
- Tipos de visualização (comparação, distribuição, composição, relação)
- Tipos de visualização × objetivo de comunicação
- Ferramentas disponíveis para criar visualizações
- Por que usar Python para visualização

---

### Aula 02 — Google Colab

**Pasta:** `aula-02/`

Apresentação da plataforma que será utilizada ao longo de todo o curso.

**Tópicos:**
- O que é o Google Colab e suas vantagens
- Como acessar e criar um notebook
- Células de texto (Markdown) e células de código
- Execução de células e atalhos de teclado
- Exemplo prático de uso básico do notebook
- Dicas de produtividade

---

### Aula 03 — Formatos de Dados

**Pasta:** `aula-03/`

Compreensão dos formatos em que os dados chegam e como representá-los em Python.

**Tópicos:**
- Fontes de dados e seus formatos
- Formato tabular como base do processamento de dados
- Formato Largo (Wide) vs. Formato Longo (Long)
- Representação em Python: listas e dicionários
- Diferença entre Wide e Long na prática
- Introdução a DataFrames e Series

---

### Aula 04 — Prática: Aulas 2 e 3

**Pasta:** `aula-04/`

Aula prática que consolida os conceitos de Colab e formatos de dados.

**Exercícios:**
- Criar e salvar um notebook no Google Colab e no Google Drive
- Fazer upload de arquivo de dados via sistema local do notebook
- Montar o Google Drive no notebook e carregar dados a partir dele
- Escrever script para carregar e inspecionar dados
- Transformar dados do formato Largo para o Longo com `melt()`
- Usar bibliotecas externas para simplificar o trabalho

---

## Módulo 2 — Manipulação de Dados com Pandas

Objetivo: dominar a biblioteca Pandas para carregar, inspecionar, filtrar e agregar dados antes de visualizá-los.

---

### Aula 05 — Pandas

**Pasta:** `aula-05/`

Introdução completa à principal biblioteca de manipulação de dados em Python.

**Tópicos:**
- Instalação e importação do Pandas
- Carregamento de dados com `read_csv()`
- Inspeção do DataFrame: `head()`, `tail()`, `sample()`, `describe()`, `info()`, `shape`
- Acesso a colunas e linhas do DataFrame
- Iteração sobre linhas com `iterrows()`
- Filtragem de dados com condições booleanas
- Agregação com `groupby()` e funções de resumo

**Biblioteca:** `pandas`

---

### Prática 05 — Pandas

**Pasta:** `pratica-aula-05/`

**Exercícios:**
1. Carregar o dataset e conhecer sua estrutura (shape, colunas, tipos)
2. Explorar estatísticas descritivas do dataset
3. Acessar colunas específicas e linhas por posição/condição
4. Filtrar Pokémons por critérios (tipo, geração, lendário)
5. Agregar e resumir dados por categoria com `groupby()`

---

## Módulo 3 — Visualizações Estáticas com Seaborn e Matplotlib

Objetivo: criar os principais tipos de gráficos estáticos com Seaborn e Matplotlib, evoluindo de gráficos simples até visuais com aparência profissional.

---

### Aula 06 — Iniciando com Seaborn: Gráficos de Barras

**Pasta:** `aula-06/`

Primeira aula dedicada à criação de gráficos com Seaborn.

**Tópicos:**
- Vantagens do Seaborn: interface de alto nível e configuração simplificada
- Instalação e configuração do tema global
- `countplot()`: contagem de ocorrências por categoria
- `barplot()`: média (ou outra métrica) por categoria
- `melt()` para transformar dados em formato longo para gráficos agrupados
- Barras agrupadas com `hue`
- Gráfico de barras empilhadas

**Bibliotecas:** `seaborn`, `pandas`, `matplotlib`

---

### Prática 06 — Iniciando com Seaborn

**Pasta:** `pratica-aula-06/`

**Exercícios:**
1. Gráfico de colunas verticais com `countplot()` por tipo de Pokémon
2. Gráfico de barras horizontal com `countplot()`
3. Média de atributo por categoria com `barplot()`
4. Comparação de métricas com `hue` e `melt()`
5. Gráfico de colunas empilhadas

---

### Aula 07 — Linhas e Áreas

**Pasta:** `aula-07/`

Gráficos para representar a variação de uma métrica ao longo de um eixo contínuo.

**Tópicos:**
- Quando usar gráficos de linha e de área
- `lineplot()` do Seaborn: série única e múltiplas séries
- Parâmetros de estilo: marcadores, traços, largura de linha
- Gráfico de área empilhado com `stackplot()` do Matplotlib
- Combinação de Seaborn com Matplotlib para personalização

**Bibliotecas:** `seaborn`, `matplotlib`

---

### Aula 08 — Dispersão e Quadrantes

**Pasta:** `aula-08/`

Gráficos para análise de distribuição e correlação entre variáveis contínuas.

**Tópicos:**
- Quando usar gráficos de dispersão
- `scatterplot()`: distribuição de pontos por duas variáveis
- Colorindo pontos com `hue` para adicionar uma terceira dimensão
- Identificação de outliers
- Criação de coluna derivada com `apply()`
- Posicionamento de legenda externa ao gráfico
- Construção de Gráfico de Quadrantes (Quadrante Mágico)
- Anotações com linhas de referência (`axvline`, `axhline`)

**Bibliotecas:** `seaborn`, `matplotlib`

---

### Prática 08 — Dispersão e Quadrantes

**Pasta:** `pratica-aula-08/`

**Exercícios:**
1. Gráfico de dispersão básico com dois atributos do Pokémon
2. Colorir pontos por tipo com `hue`
3. Ajustar posicionamento e formatação da legenda
4. Construir gráfico de quadrantes com linhas de referência
5. Filtrar o dataset e aplicar o gráfico de quadrantes no subconjunto

---

### Aula 09 — Gráfico de Pizza

**Pasta:** `aula-09/`

Introdução ao Matplotlib e discussão sobre o uso adequado do gráfico de pizza.

**Tópicos:**
- A polêmica em torno do gráfico de pizza e quando (não) usá-lo
- Definição e características do gráfico de pizza/torta
- `plt.pie()`: sintaxe básica e parâmetros principais
- Boas práticas: número de fatias, rótulos, destaque de fatias (`explode`)
- Formatação de percentuais e legendas

**Biblioteca:** `matplotlib`

---

### Aula 10 — Melhorando seus Visuais

**Pasta:** `aula-10/`

Transformação de um gráfico funcional em um visual de apresentação profissional, seguindo boas práticas de design.

**Cenário:** evolução da população dos países do BRICS ao longo dos anos.

**Tópicos:**
- Configuração global com `rcParams`
- Ajuste de tamanho de figura e DPI
- Remoção de ruído visual: `spines`, grids desnecessários
- Adição de títulos e subtítulos com fontes ajustadas
- Remoção do eixo Y e adição de valores diretamente nas barras
- Paleta de cores personalizada para destaque de dados
- Alinhamento de texto e hierarquia visual

**Bibliotecas:** `seaborn`, `matplotlib`, `pandas`

---

### Prática 09 a 14 — Consolidação

**Pasta:** `pratica-aula-09-14/`

Prática abrangente que cobre as aulas 09 a 14 em sequência, usando o dataset de Pokémons em todos os exercícios.

**Exercícios:**
1. Gráfico de pizza com distribuição de Pokémons por tipo (Aula 09)
2. Limpeza visual: remover elementos desnecessários de um gráfico (Aula 10)
3. Adicionar valores diretamente nas barras de um gráfico (Aula 10)
4. Aplicar paleta de cores personalizada (Aula 10)
5. Construir mapa de rede de relações entre tipos (Aula 11)
6. Diagrama de Sankey entre gerações e tipos (Aula 12)
7. Nuvem de palavras com nomes de Pokémons (Aula 13)
8. Consultar o dataset com SQL usando DuckDB em notebook (Aula 14)

---

## Módulo 4 — Visualizações Avançadas e Bancos de Dados

Objetivo: ampliar o repertório com tipos de gráficos especializados e integrar Python com bancos de dados SQL.

---

### Aula 11 — Mapas de Rede

**Pasta:** `aula-11/`

Visualização de relações e conexões entre entidades usando grafos.

**Tópicos:**
- O que é um mapa de rede (network map) e quando usá-lo
- Conceitos: nodos (vértices) e arestas (edges)
- Criação de grafo com `NetworkX`
- Adição de nodos e arestas com pesos
- Plotagem do grafo com `nx.draw()`
- Personalização: tamanho de nodo por grau, cor por grupo, largura de aresta por peso

**Biblioteca:** `networkx`, `matplotlib`

---

### Aula 12 — Sankey Charts

**Pasta:** `aula-12/`

Visualização de fluxo e transferência entre categorias com o Diagrama de Sankey.

**Tópicos:**
- O que é o Diagrama de Sankey e sua origem histórica
- Quando usar: relação entre duas variáveis com fluxo entre categorias
- Preparação dos dados: source, target e value
- Construção do diagrama com `plotly.graph_objects`
- Personalização de cores e rótulos dos nodos

**Biblioteca:** `plotly`

---

### Aula 13 — Wordclouds

**Pasta:** `aula-13/`

Técnica visual para analisar variáveis qualitativas por frequência de termos.

**Tópicos:**
- O que é uma nuvem de palavras e quando utilizá-la
- Preparação do texto: frequência de termos
- Criação com a biblioteca `wordcloud`
- Customização: tamanho, cores e fontes
- Uso de máscara de imagem para formatar o contorno da nuvem

**Bibliotecas:** `wordcloud`, `PIL`, `matplotlib`

---

### Aula 14 — Pandas e Bancos de Dados

**Pasta:** `aula-14/`

Integração entre Python e bancos de dados relacionais para consulta de grandes volumes de dados.

**Tópicos:**
- Por que usar bancos de dados em vez de arquivos
- Introdução ao SQL no contexto de Ciência de Dados
- Criação de banco de dados em memória com `DuckDB`
- Carregamento de um DataFrame Pandas como tabela SQL
- Consultas SQL diretamente no notebook com `JupySQL` (`%sql`, `%%sql`)
- Fluxo completo: carregar → consultar → visualizar
- Boas práticas: fechar a conexão após uso

**Bibliotecas:** `duckdb`, `jupysql`

---

## Módulo 5 — Gráficos Interativos com Plotly

Objetivo: recriar os principais tipos de gráfico em Plotly e aprender a configurar visualizações prontas para apresentação.

---

### Aula 15 — Gráficos Interativos

**Pasta:** `aula-15/`

Introdução ao Plotly Express para criação de gráficos interativos com sintaxe simples.

**Tópicos:**
- Vantagens dos gráficos interativos (hover, zoom, filtro por legenda)
- Configuração do ambiente Plotly no Colab
- `px.bar()`: gráfico de barras/colunas interativo
- `px.line()`: gráfico de linhas/área interativo
- `px.scatter()`: gráfico de dispersão interativo
- `px.pie()`: gráfico de pizza interativo
- Parâmetros comuns: `color`, `title`, `labels`, `hover_data`

**Biblioteca:** `plotly.express`

---

### Aula 16 — Criando Visualizações Efetivas

**Pasta:** `aula-16/`

Aula final do curso: construção de gráficos prontos para uso em apresentações e relatórios usando o objeto `Figure` do Plotly.

**Tópicos:**
- O objeto `Figure` do Plotly e sua estrutura (data + layout)
- Escolha do tipo de gráfico adequado ao dado
- Adição e formatação de título
- Configuração de legenda: posição, tamanho, visibilidade
- Ajuste de eixos: títulos, escala, grid e limites
- Remoção de background para visual mais limpo
- Adição de labels nos dados (`text`, `textposition`)
- Configuração de tooltips personalizados (`hovertemplate`)

**Biblioteca:** `plotly.graph_objects`

---

## Resumo Geral

| # | Tipo | Pasta | Título | Módulo |
|---|---|---|---|---|
| 01 | Aula | `aula-01/` | Teoria de Visualização de Dados | Fundamentos |
| 02 | Aula | `aula-02/` | Google Colab | Fundamentos |
| 03 | Aula | `aula-03/` | Formatos de Dados | Fundamentos |
| 04 | Prática | `aula-04/` | Prática: Aulas 2 e 3 | Fundamentos |
| 05 | Aula | `aula-05/` | Pandas | Pandas |
| P5 | Prática | `pratica-aula-05/` | Prática: Pandas | Pandas |
| 06 | Aula | `aula-06/` | Iniciando com Seaborn — Gráficos de Barras | Seaborn/Matplotlib |
| P6 | Prática | `pratica-aula-06/` | Prática: Iniciando com Seaborn | Seaborn/Matplotlib |
| 07 | Aula | `aula-07/` | Linhas e Áreas | Seaborn/Matplotlib |
| 08 | Aula | `aula-08/` | Dispersão e Quadrantes | Seaborn/Matplotlib |
| P8 | Prática | `pratica-aula-08/` | Prática: Dispersão e Quadrantes | Seaborn/Matplotlib |
| 09 | Aula | `aula-09/` | Gráfico de Pizza | Seaborn/Matplotlib |
| 10 | Aula | `aula-10/` | Melhorando seus Visuais | Seaborn/Matplotlib |
| 11 | Aula | `aula-11/` | Mapas de Rede | Visualizações Avançadas |
| 12 | Aula | `aula-12/` | Sankey Charts | Visualizações Avançadas |
| 13 | Aula | `aula-13/` | Wordclouds | Visualizações Avançadas |
| 14 | Aula | `aula-14/` | Pandas e Bancos de Dados | Visualizações Avançadas |
| P9-14 | Prática | `pratica-aula-09-14/` | Prática: Consolidação (Aulas 9 a 14) | Visualizações Avançadas |
| 15 | Aula | `aula-15/` | Gráficos Interativos | Plotly |
| 16 | Aula | `aula-16/` | Criando Visualizações Efetivas | Plotly |

---

## Tecnologias e Bibliotecas

| Categoria | Tecnologias |
|---|---|
| **Linguagem** | Python 3.12 |
| **Ambiente** | Google Colab, Jupyter Notebook, VS Code |
| **Manipulação de Dados** | Pandas, NumPy |
| **Visualização Estática** | Seaborn, Matplotlib |
| **Visualização Interativa** | Plotly Express, Plotly Graph Objects |
| **Grafos e Redes** | NetworkX |
| **Nuvem de Palavras** | WordCloud, PIL |
| **Bancos de Dados** | DuckDB, JupySQL |
