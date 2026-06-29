# Python para Ciência de Dados

## Sobre o Curso

Curso introdutório de Python voltado para iniciantes que desejam ingressar em programação e ciência de dados. O conteúdo parte dos conceitos mais básicos da linguagem e evolui progressivamente até a criação de funções reutilizáveis e manipulação de estruturas de dados complexas.

**Formato:** Jupyter Notebook (`.ipynb`), compatível com Google Colab, Thonny, REPL e VS Code.  
**Pré-requisito:** Noções de lógica de programação (conceitos como variáveis, condições e repetição são referenciados em comparação com Scratch).  
**Total de aulas:** 5 aulas teórico-práticas

---

## Módulo 1 — Fundamentos da Linguagem

Objetivo: apresentar a linguagem Python, seus conceitos essenciais e as primeiras ferramentas de entrada e saída de dados.

---

### Aula 01 — Introdução ao Python

**Arquivo:** `Python_AULA01.ipynb`

Apresentação da linguagem Python e dos elementos básicos para escrever os primeiros programas.

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
- Correção de programa com indentação errada (impressão de tabela de quadrados e cubos)

---

### Aula 02 — Tipos Básicos, Operações e Expressões

**Arquivo:** `Python_AULA02.ipynb`

Apresentação dos tipos de dados nativos do Python e das operações disponíveis para construir expressões.

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
- Implementação da fórmula de Bhaskara (equação de 2º grau) com `if/elif/else` e `math.sqrt()`

---

## Módulo 2 — Controle de Fluxo

Objetivo: dominar os comandos que controlam o caminho de execução de um programa — decisões e repetições.

---

### Aula 03 — Controle de Fluxo e Repetição

**Arquivo:** `Python_AULA03.ipynb`

Apresentação dos comandos de desvio condicional e de laço de repetição do Python.

**Tópicos:**
- Desvio condicional `if`: sintaxe, condição booleana e bloco indentado
- `if / else`: decisão binária
- `if / elif / else`: múltiplas condições encadeadas (alternativa a switch/case)
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

## Módulo 3 — Estruturas de Dados

Objetivo: apresentar as principais estruturas de dados do Python para armazenar e manipular coleções de valores.

---

### Aula 04 — Listas, Tuplas, Conjuntos e Dicionários

**Arquivo:** `Python_AULA04.ipynb`

Exploração das quatro estruturas de dados nativas do Python para organizar coleções de informações.

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

## Módulo 4 — Funções e Programação Modular

Objetivo: aprender a criar funções para reutilizar código, isolar problemas e escrever programas mais organizados.

---

### Aula 05 — Funções

**Arquivo:** `Python_AULA05.ipynb`

Introdução ao conceito de funções no Python: definição, parâmetros, retorno e funções anônimas.

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

## Resumo Geral

| # | Arquivo | Título | Módulo |
|---|---|---|---|
| 01 | `Python_AULA01.ipynb` | Introdução ao Python | Fundamentos da Linguagem |
| 02 | `Python_AULA02.ipynb` | Tipos Básicos, Operações e Expressões | Fundamentos da Linguagem |
| 03 | `Python_AULA03.ipynb` | Controle de Fluxo e Repetição | Controle de Fluxo |
| 04 | `Python_AULA04.ipynb` | Listas, Tuplas, Conjuntos e Dicionários | Estruturas de Dados |
| 05 | `Python_AULA05.ipynb` | Funções | Funções e Programação Modular |

---

## Tecnologias e Conceitos

| Categoria | Detalhes |
|---|---|
| **Linguagem** | Python 3.x |
| **Ambiente** | Google Colab, Thonny, REPL, VS Code |
| **Tipos de dados** | `str`, `int`, `float`, `complex`, `bool` |
| **Estruturas de dados** | `list`, `tuple`, `set`, `dict` |
| **Biblioteca padrão** | `math` (`sqrt`) |
| **Funções built-in** | `print()`, `input()`, `int()`, `float()`, `bool()`, `str()`, `type()`, `len()`, `list()`, `set()`, `dict()`, `range()`, `map()` |
