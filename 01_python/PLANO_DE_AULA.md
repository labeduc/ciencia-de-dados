# Plano de Aula — Python para Ciência de Dados

**Curso:** Python para Ciência de Dados  
**Carga horária total:** 3h (2 aulas de 1h30min)  
**Modalidade:** Online / Presencial  
**Público-alvo:** Iniciantes em programação com noções básicas de lógica (ex.: Scratch)  
**Pré-requisito:** Noções de lógica de programação — o curso referencia conceitos como variáveis, condições e repetição já vistos em Scratch  
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)  
**Modelo de aprendizagem:** Sala de aula invertida — o aluno estuda os notebooks antes da aula; o tempo presencial é dedicado à prática, dúvidas e consolidação.

---

> **Importante para os alunos:** Cada aula pressupõe que você já estudou os notebooks indicados na seção **Preparação** antes de comparecer à sessão presencial. Chegar sem ter feito essa preparação compromete seu aproveitamento, pois o tempo em sala será dedicado à prática — não à leitura do conteúdo.

---

## Aula 1 — Fundamentos, Tipos e Controle de Fluxo

**Duração:** 1h30min  
**Notebooks de referência:** `Python_AULA01`, `Python_AULA02`, `Python_AULA03`

### Preparação (antes da aula)

O aluno deve estudar os seguintes notebooks **antes** desta sessão:

| # | Notebook | Conteúdo |
|---|---|---|
| 1 | `Python_AULA01` | O que é Python; variáveis; strings; `print()`, `input()`; indentação |
| 2 | `Python_AULA02` | Tipos básicos; conversão; operadores matemáticos, relacionais e booleanos |
| 3 | `Python_AULA03` | `if/elif/else`; `while`; `break` e `continue` |

### Objetivo Geral

Consolidar, por meio de prática guiada e exercícios, os fundamentos do Python: entrada e saída de dados, manipulação de tipos, expressões e controle de fluxo.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Escrever e executar um programa Python no Google Colab
- Declarar variáveis, ler dados com `input()` e exibir resultados com `print()`
- Identificar e converter tipos de dados (`int`, `float`, `str`, `bool`)
- Construir expressões com operadores matemáticos, relacionais e booleanos
- Escrever desvios condicionais com `if`, `elif` e `else`
- Criar laços de repetição com `while`, usando `break` e `continue`

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (AULA01–03) |
| Prática guiada — Fundamentos | Variáveis, strings, `print()`, `input()`, conversão de tipo, indentação |
| Prática autônoma — Fundamentos | Programa de cálculo do ano de nascimento; correção de indentação |
| Prática guiada — Tipos e Expressões | Operadores e expressões; Bhaskara com `math.sqrt()` e `if/elif/else` |
| Prática guiada — Controle de Fluxo | `while` com contador; `break` e `continue`; Conjectura de Collatz |
| Prática autônoma — Controle de Fluxo | Múltiplos de 7; classificação de nota escolar; problema à escolha do aluno |

### Metodologia

- Abertura com roda de dúvidas sobre os notebooks pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam os trechos juntos, célula a célula
- Prática autônoma com exercícios progressivos; instrutor circula para apoio
- Correção comentada ao final de cada bloco autônomo

### Recursos

- Google Colab (sem instalação)
- Notebooks: `Python_AULA01`, `Python_AULA02`, `Python_AULA03`
- Biblioteca: `math` (já disponível no Python padrão)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula (AULA01–03) |
| 0:05 – 0:20 | 15 min | **Prática guiada (`AULA01`):** criar notebook no Colab; variáveis e strings; `print()` e `input()`; conversão com `int()`; indentação e blocos |
| 0:20 – 0:30 | 10 min | **Prática autônoma (`AULA01`):** programa que lê nome e idade e calcula o ano de nascimento; exercício de correção de indentação |
| 0:30 – 0:50 | 20 min | **Prática guiada (`AULA02`):** tipos com `type()` e conversões; operadores matemáticos, relacionais e booleanos; precedência com parênteses; implementação da fórmula de Bhaskara |
| 0:50 – 1:05 | 15 min | **Prática guiada (`AULA03`):** `if/elif/else` (ordenação de números, faixa de voto, classificação de nota); `while` com contador; `break` e `continue`; Conjectura de Collatz |
| 1:05 – 1:25 | 20 min | **Prática autônoma (`AULA03`):** salto dos múltiplos de 7 de 0 a 100; Bhaskara completo com leitura de dados; desafio opcional: variação da Conjectura de Collatz |
| 1:25 – 1:30 | 5 min | Correção comentada e perguntas; prévia do conteúdo da Aula 2 |

### Avaliação

O aluno conclui a aula com um notebook funcional contendo: um programa de entrada e saída de dados, ao menos uma expressão com múltiplos operadores e um programa com `if/elif/else` e `while` funcionando corretamente.

---

## Aula 2 — Estruturas de Dados e Funções

**Duração:** 1h30min  
**Notebooks de referência:** `Python_AULA04`, `Python_AULA05`

### Preparação (antes da aula)

O aluno deve estudar os seguintes notebooks **antes** desta sessão:

| # | Notebook | Conteúdo |
|---|---|---|
| 4 | `Python_AULA04` | Listas, tuplas, conjuntos, dicionários e laço `for` |
| 5 | `Python_AULA05` | Funções com `def`, parâmetros, retorno, escopo e `lambda` |

### Objetivo Geral

Consolidar, por meio de prática guiada e uma atividade final integradora, o uso das principais estruturas de dados do Python e a criação de funções reutilizáveis.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar e manipular listas com `append()`, `remove()`, `pop()` e fatiamento
- Modelar dados tabulares como lista de listas e acessar elementos por `[linha][coluna]`
- Distinguir e aplicar listas, tuplas, conjuntos e dicionários conforme o problema
- Iterar sobre coleções com o laço `for`
- Criar funções com `def`, definir parâmetros e usar `return`
- Escrever funções anônimas com `lambda` e aplicá-las com `map()`

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (AULA04–05) |
| Prática guiada — Listas | Criação, indexação, fatiamento, operações e lista de listas |
| Prática guiada — Outros tipos | Tuplas (imutabilidade), conjuntos (sem duplicatas), dicionários (chave-valor) |
| Prática guiada — `for` | Iteração sobre listas e dicionários |
| Prática autônoma — Estruturas | Mini-tradutor com dicionário; cálculo de médias com lista de listas |
| Prática guiada — Funções | `def`, parâmetros, `return`, escopo e integração de funções |
| Prática guiada — Lambda | Reescrita com `lambda`; `map()`, `list()`, `range()` |
| Atividade final integradora | Programa completo que combina estruturas de dados e funções |

### Metodologia

- Abertura com roda de dúvidas sobre os notebooks pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam os trechos juntos, comparando comportamentos entre os tipos de coleção
- Prática autônoma com exercícios de complexidade crescente
- Atividade final: aluno constrói um programa integrador escolhido dentre as opções propostas

### Recursos

- Google Colab (sem instalação)
- Notebooks: `Python_AULA04`, `Python_AULA05`
- Funções built-in utilizadas: `list()`, `set()`, `dict()`, `len()`, `range()`, `map()`

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula (AULA04–05) |
| 0:05 – 0:20 | 15 min | **Prática guiada (`AULA04` — Listas):** criação com `[]` e `list()`; indexação positiva e negativa; `append()`, `remove()`, `pop()`; fatiamento; lista de listas com cálculo de médias |
| 0:20 – 0:35 | 15 min | **Prática guiada (`AULA04` — Outros tipos):** tupla com tentativa de modificação (erro proposital); conjunto com remoção de duplicatas via `set()`; dicionário chave-valor com `in`, `keys()` e `del`; laço `for` sobre listas e dicionários |
| 0:35 – 0:55 | 20 min | **Prática autônoma (`AULA04`):** completar o exercício de lista de frutas (`append` e `pop`); construir o mini-tradutor de animais com dicionário e `while True`; desafio opcional: remover duplicatas de uma lista usando `set()` e converter de volta para `list()` |
| 0:55 – 1:10 | 15 min | **Prática guiada (`AULA05` — Funções):** `def` sem parâmetro e sem retorno (`header()`); `def` com retorno de tupla (`captura_numeros()`); `def` com parâmetros e retorno (`maior(a, b)`); integração das três funções em um programa completo |
| 1:10 – 1:20 | 10 min | **Prática guiada (`AULA05` — Lambda):** reescrita de `maior(a,b)` como `lambda`; `list(map(lambda ...))` para dobrar valores de uma lista; comparação com a versão com `for` |
| 1:20 – 1:25 | 5 min | **Atividade final (escolha do aluno):** opção A — função `maior3(a,b,c)` que reutiliza `maior(a,b)`; opção B — função que recebe uma lista e retorna média, mínimo e máximo sem bibliotecas; opção C — mini-agenda com dicionário e funções separadas para cadastrar e consultar |
| 1:25 – 1:30 | 5 min | Apresentação de dois ou três trabalhos; encerramento do curso e próximos passos |

### Avaliação

O aluno entrega um notebook com:
- Ao menos um exemplo funcional de cada tipo de coleção (lista, tupla, conjunto ou dicionário)
- Ao menos uma função com parâmetros e retorno
- A atividade final integradora concluída (qualquer uma das três opções)

---

## Visão Geral do Curso

| Aula | Tema | Duração | Preparação (notebooks) | Prática em sala |
|---|---|---|---|---|
| 1 | Fundamentos, Tipos e Controle de Fluxo | 1h30min | AULA01, AULA02, AULA03 | Exercícios de expressões, `if/elif/else` e `while` |
| 2 | Estruturas de Dados e Funções | 1h30min | AULA04, AULA05 | Mini-tradutor, médias com listas, funções e atividade final |
| **Total** | | **3h** | **5 notebooks** | **Exercícios progressivos + 1 atividade integradora** |
