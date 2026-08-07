# Conteúdo Programático Completo - Curso de Ciência de Dados

Este documento consolida o conteúdo programático de todos os módulos do curso.

---

## Módulo 1 - Python para Ciência de Dados

### Sobre o Curso
Curso introdutório de Python voltado para iniciantes que desejam ingressar em programação e ciência de dados. O conteúdo parte dos conceitos mais básicos da linguagem e evolui progressivamente até a criação de funções reutilizáveis e manipulação de estruturas de dados complexas.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Thonny, REPL e VS Code.  
**Pré-requisito:** Noções de lógica de programação.  
**Total de aulas:** 5 aulas teórico-práticas

---

### Aula 01 — Introdução ao Python
**Tópicos:**
- O que é Python: linguagem interpretada, multiplataforma e open source
- Plataformas de desenvolvimento: Thonny, Programiz, REPL, VSCode, PyCharm
- Como executar um programa Python (extensão `.py` e interpretador do Colab)
- Comentários com `#`
- Variáveis: declaração e uso
- Strings: aspas simples, duplas e multilinha (`'''`)
- Saída de dados com `print()`
- Entrada de dados com `input()`
- Conversão de tipo com `int()`
- Indentação e blocos de código

**Exercícios:**
- Programa que lê nome e idade e calcula o ano de nascimento
- Correção de programa com indentação errada

---

### Aula 02 — Tipos Básicos, Operações e Expressões
**Tópicos:**
- Tipos básicos: `str`, `int`, `float`, `complex`, `bool`
- Identificação de tipo com `type()`
- Conversão entre tipos: `int()`, `float()`, `bool()`, `str()`
- Comportamento de `bool("0")` vs. `bool(0)`
- Operadores matemáticos: `+`, `-`, `*`, `/`, `**`, `//`, `%`, negação unária
- Operadores relacionais: `==`, `!=`, `>`, `>=`, `<`, `<=`, intervalo `a < x < b`
- Operadores booleanos: `&`, `|`, `^`, `not`
- Parênteses e precedência de operadores

**Exercício:**
- Implementação da fórmula de Bhaskara com `if/elif/else` e `math.sqrt()`

---

### Aula 03 — Controle de Fluxo e Repetição
**Tópicos:**
- Desvio condicional `if`: sintaxe, condição booleana e bloco indentado
- `if / else`: decisão binária
- `if / elif / else`: múltiplas condições encadeadas
- Laço de repetição `while`: sintaxe e uso de contador
- Laço infinito com `while True`
- Comandos `break` e `continue`
- Operador `%` (resto da divisão) para testar paridade e divisibilidade

**Exercícios:**
- Ordenação de dois números lidos pelo usuário com `if`
- Verificação de obrigatoriedade de voto por faixa etária
- Classificação de nota escolar com `if/elif/else`
- Conjectura de Collatz (laço com `break` e `continue`)
- Salto dos múltiplos de 7 de 0 a 100

---

### Aula 04 — Listas, Tuplas, Conjuntos e Dicionários
**Tópicos:**
- **Listas (`list`):** declaração com `[]` e com `list()`, indexação a partir do zero, índices negativos
- Operações com listas: `append()`, `remove()`, `del`, `pop()`
- Fatiamento de listas: `lista[inicio:fim]`, `lista[:fim]`, `lista[inicio:]`
- Lista de listas (matriz bidimensional): modelagem de tabelas, acesso por `[linha][coluna]`
- **Tuplas:** declaração com `()`, imutabilidade e limitações
- **Conjuntos (`set`):** sem ordem, sem índice e sem duplicatas
- Conversão de lista em conjunto com `set()` para remover duplicatas
- Operações com conjuntos: `add()`, operador `in`
- **Dicionários (`dict`):** estrutura chave-valor, declaração com `{}` e com `dict()`
- Operações com dicionários: acesso por chave, `del`, `keys()`, operador `in`
- Laço de repetição `for` para iterar listas e dicionários
- Método `format()` para interpolação de strings

**Exercícios:**
- Manipulação de lista de frutas com `append`, `remove` e `pop`
- Cálculo de total e média de notas usando lista de listas com `while`
- Mini-sistema de tradutor de animais com dicionário e `while True`

---

### Aula 05 — Funções
**Tópicos:**
- Motivação para funções: reuso, isolamento e abstração
- Sintaxe de declaração com `def`
- Funções sem parâmetro e sem retorno (procedimentos)
- Funções sem parâmetro com retorno
- Funções com parâmetros e retorno
- Comando `return` e retorno de múltiplos valores com tupla
- Escopo de variáveis: variáveis locais vs. variáveis globais
- Funções como objetos (passagem de função como argumento)
- Funções anônimas com `lambda`: sintaxe `lambda argumentos: expressão`
- Expressão condicional em linha (`a if condição else b`)
- Funções de ordem superior: `map()`, `list()`, `range()`

**Exercícios:**
- Implementação de `header()`, `captura_numeros()` e `maior()` integrados em um programa completo
- Reescrita de `maior()` como função lambda
- Duplicação de lista com `for` vs. `map()` + `lambda`
- Função `maior3(a, b, c)` que calcula o maior entre três números reutilizando `maior(a, b)`

---

## Módulo 2 - Estatística e Análise de Dados

### Sobre o Curso
Curso de Estatística Básica e Análise de Dados, focado na recolha, organização, cálculo descritivo e interpretação analítica de grandes volumes de informação utilizando folhas de cálculo.

**Formato:** Leitura em Markdown (`.md`) + práticas com planilhas  
**Software:** Google Planilhas ou Microsoft Excel

---

### Aula 1: Introdução, Recolha e Organização de Dados
**Objetivos:** Compreender os conceitos fundamentais de estatística; aprender a recolher e estruturar massas de dados; identificar variáveis de referência.

**Conteúdos Programáticos:**
- Definição de Estatística, População e Amostra
- A importância do tamanho da amostra para representar fielmente uma população
- Organização de dados em tabelas: estruturação em linhas (elementos) e colunas (categorias/variáveis)
- Técnicas de ordenamento e agrupamento por variáveis para a criação de subconjuntos analíticos

**Metodologia / Atividades Práticas:**
- Análise de Cenário: Reflexão sobre a organização financeira pessoal ao longo de um ano
- Exercício de Construção: Criação de uma tabela de dados com categorias predefinidas e subsequente ordenação/agrupamento

---

### Aula 2: Medidas de Tendência Central e Frequências
**Objetivos:** Calcular e identificar informações essenciais em conjuntos de dados; preencher dados em falta; aplicar fórmulas de estatística descritiva em planilhas.

**Conteúdos Programáticos:**
- Conceito de Mínimo (`MÍN`) e Máximo (`MÁX`) num conjunto de dados (amplitude primária)
- Média aritmética (`MÉDIA`): cálculo da posição central
- Frequência Absoluta (número de ocorrências) e Frequência Relativa (percentagem do total)
- Moda (`MODO`): identificação do valor com maior recorrência
- Frequência Acumulada: soma consecutiva das frequências para análise de impacto progressivo

**Metodologia / Atividades Práticas:**
- Atividade Prática 1 (Equipa de Voleibol): Utilização de funções estatísticas para extrair extremos e médias
- Atividade Prática 2 (Consumo de Combustível): Importação de CSV para calcular médias de despesas mensais
- Atividade Prática 3 (Análise Amostral): Avaliação da variação da frequência relativa à medida que a amostra cresce

---

### Aula 3: Ordenação de Dados e a Mediana
**Objetivos:** Compreender o impacto do ordenamento na análise de dados; calcular e interpretar a mediana como medida robusta de tendência central.

**Conteúdos Programáticos:**
- O conceito de Mediana (`MED`) como o valor que divide o conjunto de dados exatamente ao meio
- A importância do ordenamento prévio (rol de dados) para o cálculo da mediana
- Regras de cálculo para conjuntos de dados com número ímpar e par de elementos
- Comparação analítica: Quando utilizar a Média versus quando utilizar a Mediana (sensibilidade a outliers)

**Metodologia / Atividades Práticas:**
- Estudo de Caso: Análise do impacto de valores extremos (*outliers*) em um conjunto de salários
- Laboratório de Dados: Resolução prática de exercícios de cálculo de mediana

---

### Aula 4: Análise Avançada, Correlação e Projeções
**Objetivos:** Analisar criticamente distribuições de dados; identificar relações matemáticas entre variáveis; projetar valores futuros ou intermediários com segurança.

**Conteúdos Programáticos:**
- **Desvio Padrão e Variância:** Introdução ao conceito de dispersão de dados em torno da média
- **Correlação:** Relação matemática entre duas variáveis (Covariância)
  - Coeficiente próximo de `1`: linearidade direta
  - Coeficiente próximo de `-1`: linearidade inversa
  - **Correlação Espúria:** Situações onde há forte relação matemática, mas nenhuma ligação lógica/causal
- **Interpolação vs. Extrapolação:**
  - *Interpolação:* Estimar valores intermédios dentro de um grupo limitado de dados conhecidos
  - *Extrapolação:* Assumir que a tendência matemática se manterá para além dos limites conhecidos

**Metodologia / Atividades Práticas:**
- Estudo de Caso Financeiro e Consumo: Análise de matrizes de dados para verificar correlação entre preços de combustíveis
- Exercício de Projeção: Aplicação de conceitos de interpolação e extrapolação baseados em séries temporais

---

## Módulo 3 - Visualização de Dados com Python

### Sobre o Curso
Curso completo de Visualização de Dados com Python voltado para iniciantes e profissionais. O conteúdo parte da teoria de visualização e evolui até a criação de gráficos profissionais e interativos.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Jupyter e VS Code.  
**Total de aulas:** 16 aulas teóricas + 4 práticas

---

### Aula 01 — Teoria de Visualização de Dados
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
**Tópicos:**
- O que é o Google Colab e suas vantagens
- Como acessar e criar um notebook
- Células de texto (Markdown) e células de código
- Execução de células e atalhos de teclado
- Exemplo prático de uso básico do notebook
- Dicas de produtividade

---

### Aula 03 — Formatos de Dados
**Tópicos:**
- Fontes de dados e seus formatos
- Formato tabular como base do processamento de dados
- Formato Largo (Wide) vs. Formato Longo (Long)
- Representação em Python: listas e dicionários
- Diferença entre Wide e Long na prática
- Introdução a DataFrames e Series

---

### Aula 04 — Prática: Aulas 2 e 3
**Exercícios:**
- Criar e salvar um notebook no Google Colab e no Google Drive
- Fazer upload de arquivo de dados via sistema local do notebook
- Montar o Google Drive no notebook e carregar dados a partir dele
- Escrever script para carregar e inspecionar dados
- Transformar dados do formato Largo para o Longo com `melt()`
- Usar bibliotecas externas para simplificar o trabalho

---

### Aula 05 — Pandas
**Tópicos:**
- Instalação e importação do Pandas
- Carregamento de dados com `read_csv()`
- Inspeção do DataFrame: `head()`, `tail()`, `sample()`, `describe()`, `info()`, `shape`
- Acesso a colunas e linhas do DataFrame
- Iteração sobre linhas com `iterrows()`
- Filtragem de dados com condições booleanas
- Agregação com `groupby()` e funções de resumo

---

### Prática 05 — Pandas
**Exercícios:**
1. Carregar o dataset e conhecer sua estrutura
2. Explorar estatísticas descritivas do dataset
3. Acessar colunas específicas e linhas por posição/condição
4. Filtrar Pokémons por critérios (tipo, geração, lendário)
5. Agregar e resumir dados por categoria com `groupby()`

---

### Aula 06 — Iniciando com Seaborn: Gráficos de Barras
**Tópicos:**
- Vantagens do Seaborn: interface de alto nível e configuração simplificada
- Instalação e configuração do tema global
- `countplot()`: contagem de ocorrências por categoria
- `barplot()`: média (ou outra métrica) por categoria
- `melt()` para transformar dados em formato longo para gráficos agrupados
- Barras agrupadas com `hue`
- Gráfico de barras empilhadas

---

### Prática 06 — Iniciando com Seaborn
**Exercícios:**
1. Gráfico de colunas verticais com `countplot()` por tipo de Pokémon
2. Gráfico de barras horizontal com `countplot()`
3. Média de atributo por categoria com `barplot()`
4. Comparação de métricas com `hue` e `melt()`
5. Gráfico de colunas empilhadas

---

### Aula 07 — Linhas e Áreas
**Tópicos:**
- Quando usar gráficos de linha e de área
- `lineplot()` do Seaborn: série única e múltiplas séries
- Parâmetros de estilo: marcadores, traços, largura de linha
- Gráfico de área empilhado com `stackplot()` do Matplotlib
- Combinação de Seaborn com Matplotlib para personalização

---

### Aula 08 — Dispersão e Quadrantes
**Tópicos:**
- Quando usar gráficos de dispersão
- `scatterplot()`: distribuição de pontos por duas variáveis
- Colorindo pontos com `hue` para adicionar uma terceira dimensão
- Identificação de outliers
- Criação de coluna derivada com `apply()`
- Posicionamento de legenda externa ao gráfico
- Construção de Gráfico de Quadrantes (Quadrante Mágico)
- Anotações com linhas de referência (`axvline`, `axhline`)

---

### Prática 08 — Dispersão e Quadrantes
**Exercícios:**
1. Gráfico de dispersão básico com dois atributos do Pokémon
2. Colorir pontos por tipo com `hue`
3. Ajustar posicionamento e formatação da legenda
4. Construir gráfico de quadrantes com linhas de referência
5. Filtrar o dataset e aplicar o gráfico de quadrantes no subconjunto

---

### Aula 09 — Gráfico de Pizza
**Tópicos:**
- A polêmica em torno do gráfico de pizza e quando (não) usá-lo
- Definição e características do gráfico de pizza/torta
- `plt.pie()`: sintaxe básica e parâmetros principais
- Boas práticas: número de fatias, rótulos, destaque de fatias (`explode`)
- Formatação de percentuais e legendas

---

### Aula 10 — Melhorando seus Visuais
**Cenário:** evolução da população dos países do BRICS ao longo dos anos.

**Tópicos:**
- Configuração global com `rcParams`
- Ajuste de tamanho de figura e DPI
- Remoção de ruído visual: `spines`, grids desnecessários
- Adição de títulos e subtítulos com fontes ajustadas
- Remoção do eixo Y e adição de valores diretamente nas barras
- Paleta de cores personalizada para destaque de dados
- Alinhamento de texto e hierarquia visual

---

### Prática 09 a 14 — Consolidação
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

### Aula 11 — Mapas de Rede
**Tópicos:**
- O que é um mapa de rede (network map) e quando usá-lo
- Conceitos: nodos (vértices) e arestas (edges)
- Criação de grafo com `NetworkX`
- Adição de nodos e arestas com pesos
- Plotagem do grafo com `nx.draw()`
- Personalização: tamanho de nodo por grau, cor por grupo, largura de aresta por peso

---

### Aula 12 — Sankey Charts
**Tópicos:**
- O que é o Diagrama de Sankey e sua origem histórica
- Quando usar: relação entre duas variáveis com fluxo entre categorias
- Preparação dos dados: source, target e value
- Construção do diagrama com `plotly.graph_objects`
- Personalização de cores e rótulos dos nodos

---

### Aula 13 — Wordclouds
**Tópicos:**
- O que é uma nuvem de palavras e quando utilizá-la
- Preparação do texto: frequência de termos
- Criação com a biblioteca `wordcloud`
- Customização: tamanho, cores e fontes
- Uso de máscara de imagem para formatar o contorno da nuvem

---

### Aula 14 — Pandas e Bancos de Dados
**Tópicos:**
- Por que usar bancos de dados em vez de arquivos
- Introdução ao SQL no contexto de Ciência de Dados
- Criação de banco de dados em memória com `DuckDB`
- Carregamento de um DataFrame Pandas como tabela SQL
- Consultas SQL diretamente no notebook com `JupySQL` (`%sql`, `%%sql`)
- Fluxo completo: carregar → consultar → visualizar
- Boas práticas: fechar a conexão após uso

---

### Aula 15 — Gráficos Interativos
**Tópicos:**
- Vantagens dos gráficos interativos (hover, zoom, filtro por legenda)
- Configuração do ambiente Plotly no Colab
- `px.bar()`: gráfico de barras/colunas interativo
- `px.line()`: gráfico de linhas/área interativo
- `px.scatter()`: gráfico de dispersão interativo
- `px.pie()`: gráfico de pizza interativo
- Parâmetros comuns: `color`, `title`, `labels`, `hover_data`

---

### Aula 16 — Criando Visualizações Efetivas
**Tópicos:**
- O objeto `Figure` do Plotly e sua estrutura (data + layout)
- Escolha do tipo de gráfico adequado ao dado
- Adição e formatação de título
- Configuração de legenda: posição, tamanho, visibilidade
- Ajuste de eixos: títulos, escala, grid e limites
- Remoção de background para visual mais limpo
- Adição de labels nos dados (`text`, `textposition`)
- Configuração de tooltips personalizados (`hovertemplate`)

---

## Módulo 4 - Banco de Dados com SQL e NoSQL

### Sobre o Curso
Curso introdutório de Banco de Dados voltado para iniciantes em Ciência de Dados. O conteúdo parte da teoria de bancos de dados relacionais, evolui pela linguagem SQL e modelagem de dados, e culmina com uma introdução a bancos NoSQL com MongoDB.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Jupyter e VS Code.  
**SGBD utilizado:** SQLite (via biblioteca `sqlite3` e extensão `ipython-sql`) e MongoDB (via biblioteca `mongita`).  
**Total de aulas:** 4 aulas teórico-práticas + 2 notebooks de exercícios.

---

### Aula 01 — Introdução a Banco de Dados e Consultas SQL
**Tópicos:**
- O que é um banco de dados (quiz de abertura)
- Apresentação da disciplina: presença dos bancos de dados no dia a dia
- Crescimento do volume de dados no mundo (Data Never Sleeps, unidades de medida)
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

---

### Prática 01 — SQL Island
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

---

### Prática 02 — Modelagem do Banco BDEmpregados
**Exercícios:**
1. Criar todas as tabelas do modelo BDEmpregado, escolhendo o melhor tipo de dado e a melhor nomenclatura
2. Inserir todos os registros do modelo em suas respectivas tabelas
3. Selecionar todos os campos da tabela de empregados
4. Selecionar todos os campos da tabela de empregados ordenados por RG (decrescente)
5. Selecionar todos os campos da tabela de empregados ordenados por nome (decrescente)
6. Relacionar empregados e dependentes: nome do empregado, nome, data de nascimento e relação de cada dependente
7. Contar quantos empregados existem por departamento
8. Contar quantos empregados existem por projeto
9. Contar quantos projetos existem por departamento
10. Contar quantos dependentes existem no total

---

### Aula 03 — Modelagem de Dados
**Tópicos:**
- O que é modelagem de dados e por que ela importa na era da IA
- Os 3 conceitos fundamentais: Entidade, Atributo e Relacionamento
- Tipos de relacionamento: 1:1, 1:N e N:N (tabela intermediária)
- Os 3 níveis de modelagem: Conceitual, Lógico e Físico
- Diagrama Entidade-Relacionamento (ER): elementos e leitura
- Prática guiada: modelagem completa de uma Rede Social de Games (Jogador, Jogo, Conquista, Partida)
- Do modelo conceitual ao `CREATE TABLE` com constraints
- Inserção de dados temáticos (nicknames, jogos reais) e consultas com `JOIN`
- Normalização: comparação tabela única vs. normalizada
- Boas práticas de modelagem (8 regras de ouro)
- Exercícios: 5 consultas + 1 desafio (criar tabela N:N `Conquista_Jogador`)

---

### Aula 04 — NoSQL e MongoDB
**Tópicos:**
- SQL vs NoSQL: diferenças, vantagens e quando usar cada um
- Tipos de banco NoSQL: Documentos, Chave-Valor, Colunar e Grafos
- MongoDB: coleções, documentos, campos — vocabulário SQL → MongoDB
- O poder dos documentos: dados aninhados (listas e objetos dentro de documentos)
- Setup com `mongita` (versão leve do MongoDB para aprendizado)
- `insert_one()` e `insert_many()` — inserção de documentos com campos variáveis
- `find()` e `find_one()` — consultas com operadores (`$gt`, `$lt`, `$gte`, `$lte`, `$ne`, `$in`, `$or`)
- Busca dentro de listas e subdocumentos (dot notation)
- `sort()` e `limit()` — ordenação e limitação de resultados
- `update_one()` e `update_many()` — operadores `$set`, `$inc`, `$push`, `$pull`, `$unset`
- `delete_one()` e `delete_many()` — remoção de documentos
- `count_documents()` — contagem com filtros
- Comparação lado a lado: SQL vs MongoDB
- Quando usar SQL vs NoSQL — critérios de decisão
- NoSQL e IA: RAG, cache, busca vetorial
- Exercícios: 6 consultas + 1 desafio (criar coleção de partidas)

---

---

## Módulo 5 - Desenvolvimento com AI

### Sobre o Conteúdo
Trilha de desenvolvimento que ensina a usar AI Assistants como ferramentas de aprendizado e criação de software, aplicando conceitos de UX, HTML, CSS, JavaScript e integração de dados em um projeto de dashboard funcional.

---

### Aula 1 — Primeiro Contato com AI (Assíncrono)
**Carga horária:** até 2h (leitura + exercícios)

**Conteúdo:**
- O que é um AI Assistant e como conversar com ele
- O que um AI Assistant pode fazer por quem está aprendendo a programar
- O que um AI Assistant **não** faz bem
- Como conversar com um AI Assistant (boas práticas)
- 3 exercícios de Python para resolver manualmente e pedir explicação à AI
- Mini-leitura: Como escrever bons requisitos para a AI (template simples)

---

### Aula 2 — Revisão com AI (Assíncrono)
**Carga horária:** até 2h (leitura + exercícios)

**Conteúdo:**
- Prática AI: 3 programas com bugs para depurar com ajuda da AI
- Desafio AI: Gerar código com requisito detalhado, revisar e questionar
- Leitura: Como questionar a AI sobre o código dela (guia com perguntas prontas)

---

### Módulo 6 — UX e Design de Interfaces + AI para Prototipação
**Carga horária:** 3h (1h aula ativa + até 2h assíncrono)

**Aula Ativa (1h):**
- O que é UX: pensar no usuário antes de codar
- Princípios básicos de UX para dashboards
- Wireframe rápido: papel, Paint ou aplicação simplificada
- Atividade em aula: wireframe da dashboard
- Prática AI: descrever a interface e receber sugestões

**Conteúdo Assíncrono:**
- Leitura: UX para iniciantes (30 min)
- Tarefa: criar wireframe do projeto de integração (40 min)
- Desafio AI: descrever o wireframe e pedir críticas de usabilidade (30 min)
- Checklist: revisão do protótipo antes de começar a codar (20 min)

---

### Módulo 7 — HTML e CSS com AI Assistants
**Carga horária:** 3h (1h aula ativa + até 2h assíncrono)

**Aula Ativa (1h):**
- HTML semântico: estrutura da página
- CSS essencial: box model, flexbox, responsividade
- Prática AI intensiva: o ciclo Requisito → Gerar → Aprender → Revisar
- Prática em aula: Card de KPI

**Conteúdo Assíncrono:**
- Leitura: Guia visual HTML + CSS (30 min)
- Tarefa: construir a estrutura HTML/CSS da dashboard (60 min)
- Prática AI obrigatória: o ciclo para cada seção (incluso nos 60 min)
- Leitura complementar: semântica e acessibilidade (30 min)

---

### Módulo 8 — JavaScript + Interatividade + Dados na Tela
**Carga horária:** 3h (1h aula ativa + até 2h assíncrono)

**Aula Ativa (1h):**
- JS essencial: variáveis, funções, eventos (comparação Python → JavaScript)
- DOM: selecionar e modificar elementos
- Prática AI intensiva: carregar dados e renderizar tabela

**Conteúdo Assíncrono:**
- Leitura: JavaScript essencial para quem já viu Python (20 min)
- Leitura: DOM para iniciantes com diagrama visual (20 min)
- Tarefa: adicionar interatividade à dashboard (40 min)
- Prática AI: gerar validação de formulário, pedir testes, verificar (20 min)

---

### Módulo 9 — Exibir e Organizar Dados no Frontend + Integração Completa com AI
**Carga horária:** 3h (1h aula ativa + até 2h assíncrono)

**Aula Ativa (1h):**
- Criar gráficos a partir de dados com Chart.js
- Idealizar a integração completa do projeto
- Ciclo AI completo e autônomo (aluno decide o que construir)

**Conteúdo Assíncrono:**
- Leitura: Chart.js essencial com 3 tipos de gráfico (30 min)
- Tarefa: implementar gráficos pertinentes à análise de dados (40 min)
- Refinamentos com AI: filtros, loading e tratamento de erros (30 min)
- Autoavaliação: "O que consegui fazer sozinho vs. o que a AI fez por mim?" (20 min)

---

### Módulo 10 — Projeto Integrador — Visualização de Dados
**Carga horária:** 3h (1h aula ativa + até 2h assíncrono)

**Aula Ativa (1h):**
- Revisão e correções finais com mentoria
- Documentar o uso de AI no projeto (Diário de Campo)
- Apresentação para a turma (3–5 minutos)

**Conteúdo Assíncrono:**
- Finalizar a página: ajustes visuais, responsividade, testes (50 min)
- Escrever o Diário de Campo (40 min)
- Preparar apresentação (30 min)

**Entrega Final:**
1. Dashboard funcional (index.html, style.css, script.js)
2. Diário de Campo (3 melhores prompts, 1 erro da AI, 1 aprendizado)
3. Apresentação (demo ao vivo ou slides)

---

## Tecnologias e Bibliotecas

| Categoria | Tecnologias |
|---|---|
| **Linguagem** | Python 3.12, JavaScript, SQL |
| **Ambiente** | Google Colab, Jupyter Notebook, VS Code |
| **Python** | Pandas, NumPy, math |
| **Visualização Estática** | Seaborn, Matplotlib |
| **Visualização Interativa** | Plotly Express, Plotly Graph Objects |
| **Grafos e Redes** | NetworkX |
| **Nuvem de Palavras** | WordCloud, PIL |
| **Bancos de Dados** | SQLite, DuckDB, JupySQL |
| **Frontend** | HTML5, CSS3, Chart.js |
| **AI Assistants** | ChatGPT, Copilot, Gemini (uso pedagógico) |
