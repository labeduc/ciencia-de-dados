# Plano de Aula — Python para Ciência de Dados

**Curso:** Python para Ciência de Dados  
**Carga horária total:** 3h (2 aulas de 1h30min)  
**Modalidade:** Online / Presencial  
**Público-alvo:** Iniciantes em programação com noções básicas de lógica (ex.: Scratch)  
**Pré-requisito:** Noções de lógica de programação — o curso referencia conceitos como variáveis, condições e repetição já vistos em Scratch  
**Ferramenta principal:** Google Colab (acesso via navegador, sem instalação local)  
**Modelo de aprendizagem:** Sala de aula invertida — o aluno estuda os notebooks antes da aula; o tempo presencial é dedicado à prática, dúvidas e consolidação.

> A cobertura integral combina estudo prévio e prática presencial. Os materiais de IA são complementares e assíncronos; portanto, não acrescentam tempo à carga horária de 3h.

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
| 1 | `Python_AULA01` | O que é Python; comentários; variáveis e atribuição múltipla; palavras reservadas; strings; `print()`, `input()`; indentação; `dir()` e `__doc__` |
| 2 | `Python_AULA02` | Tipos básicos; conversão; operadores matemáticos, relacionais e booleanos; tabelas-verdade; precedência |
| 3 | `Python_AULA03` | `if/elif/else`; `while`; `break` e `continue` |

### Objetivo Geral

Consolidar, por meio de prática guiada e exercícios, os fundamentos do Python: entrada e saída de dados, manipulação de tipos, expressões e controle de fluxo.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Escrever e executar um programa Python no Google Colab
- Declarar variáveis, ler dados com `input()` e exibir resultados com `print()`
- Reconhecer nomes válidos, palavras reservadas e formas de consultar atributos e documentação de objetos
- Identificar e converter tipos de dados (`int`, `float`, `str`, `bool`)
- Construir expressões com operadores matemáticos, relacionais e booleanos
- Escrever desvios condicionais com `if`, `elif` e `else`
- Criar laços de repetição com `while`, usando `break` e `continue`

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (AULA01–03) |
| Prática guiada — Fundamentos | Variáveis, strings, `print()`, `input()`, conversão de tipo, indentação; consulta breve com `dir()` e `__doc__` |
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
| 0:05 – 0:20 | 15 min | **Prática guiada (`AULA01`):** criar notebook no Colab; variáveis e strings; `print()` e `input()`; conversão com `int()`; indentação; demonstração breve de `dir()` e `__doc__` |
| 0:20 – 0:30 | 10 min | **Prática autônoma (`AULA01`):** programa que lê nome e idade e calcula o ano de nascimento; exercício de correção de indentação |
| 0:30 – 0:50 | 20 min | **Prática guiada (`AULA02`):** tipos com `type()` e conversões; operadores matemáticos, relacionais e booleanos; precedência com parênteses; implementação da fórmula de Bhaskara |
| 0:50 – 1:05 | 15 min | **Prática guiada (`AULA03`):** `if/elif/else` (ordenação de números, faixa de voto, classificação de nota); `while` com contador; `break` e `continue`; Conjectura de Collatz |
| 1:05 – 1:25 | 20 min | **Prática autônoma (`AULA03`):** salto dos múltiplos de 7 de 0 a 100; Bhaskara completo com leitura de dados; desafio opcional: variação da Conjectura de Collatz |
| 1:25 – 1:30 | 5 min | Correção comentada e perguntas; prévia do conteúdo da Aula 2 |

### Avaliação

O aluno conclui a aula com um notebook funcional contendo: um programa de entrada e saída de dados, ao menos uma expressão com múltiplos operadores e um programa com `if/elif/else` e `while` funcionando corretamente.

---

## Aula 2 — Estruturas de Dados, Funções e Bibliotecas

**Duração:** 1h30min  
**Notebooks de referência:** `Python_AULA04`, `Python_AULA05`, `Python_AULA06`

### Preparação (antes da aula)

O aluno deve estudar os seguintes notebooks **antes** desta sessão:

| # | Notebook | Conteúdo |
|---|---|---|
| 4 | `Python_AULA04` | Listas, tuplas, conjuntos, dicionários e laço `for` |
| 5 | `Python_AULA05` | Funções com `def`, parâmetros, retorno, escopo e `lambda` |
| 6 | `Python_AULA06` | Bibliotecas e módulos; PyPI; instalação de pacotes; formas de importação |

### Objetivo Geral

Consolidar, por meio de prática guiada e uma atividade final integradora, o uso das principais estruturas de dados do Python, a criação de funções reutilizáveis e o uso inicial de bibliotecas, sem ampliar a carga horária do curso.

### Objetivos Específicos

Ao final desta aula, o aluno será capaz de:

- Criar e manipular listas com `append()`, `remove()`, `pop()` e fatiamento
- Modelar dados tabulares como lista de listas e acessar elementos por `[linha][coluna]`
- Distinguir e aplicar listas, tuplas, conjuntos e dicionários conforme o problema
- Iterar sobre coleções com o laço `for`
- Criar funções com `def`, definir parâmetros e usar `return`
- Escrever funções anônimas com `lambda` e aplicá-las com `map()`
- Localizar pacotes e consultar sua documentação no PyPI
- Importar módulos e objetos usando `import`, `as` e `from ... import`

### Conteúdo

| Bloco | Tópicos |
|---|---|
| Revisão express | Abertura de dúvidas sobre o conteúdo pré-aula (AULA04–06) |
| Prática guiada — Listas | Criação, indexação, fatiamento, operações e lista de listas |
| Prática guiada — Outros tipos | Tuplas (imutabilidade), conjuntos (sem duplicatas), dicionários (chave-valor) |
| Prática guiada — `for` | Iteração sobre listas e dicionários |
| Prática autônoma — Estruturas | Mini-tradutor com dicionário; cálculo de médias com lista de listas |
| Prática guiada — Funções | `def`, parâmetros, `return`, escopo e integração de funções |
| Prática guiada — Lambda | Reescrita com `lambda`; `map()`, `list()`, `range()` |
| Prática guiada — Bibliotecas | PyPI; instalação de pacotes; `import`, `as` e `from ... import`; exemplos com `math` e `tinydb` |
| Atividade final integradora | Programa curto que combina estruturas de dados, funções e ao menos uma importação |

### Metodologia

- Abertura com roda de dúvidas sobre os notebooks pré-aula (máx. 5 min)
- Prática guiada: instrutor e aluno executam os trechos juntos, comparando comportamentos entre os tipos de coleção
- Prática autônoma com exercícios de complexidade crescente
- Atividade final curta e focada: aluno adapta uma solução já iniciada, combinando os conceitos da aula
- A inclusão da AULA06 ocorre por redistribuição dos blocos práticos, mantendo a sessão em 1h30min

### Recursos

- Google Colab (sem instalação)
- Notebooks: `Python_AULA04`, `Python_AULA05`, `Python_AULA06`
- Funções built-in utilizadas: `list()`, `set()`, `dict()`, `len()`, `range()`, `map()`
- Bibliotecas e serviços: `math`, `tinydb` e PyPI

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: dúvidas sobre o conteúdo pré-aula (AULA04–06) |
| 0:05 – 0:17 | 12 min | **Prática guiada (`AULA04` — Listas):** criação, indexação, `append()`, `remove()`, `pop()`, fatiamento e lista de listas |
| 0:17 – 0:27 | 10 min | **Prática guiada (`AULA04` — Outros tipos):** imutabilidade de tuplas; remoção de duplicatas com conjuntos; dicionários chave-valor; laço `for` |
| 0:27 – 0:40 | 13 min | **Prática autônoma (`AULA04`):** completar um exercício de listas e construir uma versão reduzida do mini-tradutor com dicionário |
| 0:40 – 0:55 | 15 min | **Prática guiada (`AULA05` — Funções):** `def`, parâmetros, retorno e integração de `header()`, `captura_numeros()` e `maior(a, b)` |
| 0:55 – 1:03 | 8 min | **Prática guiada (`AULA05` — Lambda):** reescrita de `maior(a,b)` como `lambda` e uso de `map()` para transformar uma lista |
| 1:03 – 1:15 | 12 min | **Prática guiada (`AULA06` — Bibliotecas):** localizar e consultar um pacote no PyPI; reconhecer pacote ausente; comparar `import math`, `import math as ...` e `from math import ...`; demonstração breve de instalação e importação do `tinydb` |
| 1:15 – 1:25 | 10 min | **Atividade final:** adaptar uma função para receber uma lista e retornar resultados calculados com ao menos um recurso importado de `math`; extensão opcional fora da aula: mini-agenda com `tinydb` |
| 1:25 – 1:30 | 5 min | Apresentação de dois ou três trabalhos; encerramento do curso e próximos passos |

### Avaliação

O aluno entrega um notebook com:
- Ao menos um exemplo funcional de cada tipo de coleção (lista, tupla, conjunto ou dicionário)
- Ao menos uma função com parâmetros e retorno
- Ao menos uma importação funcional usando uma das sintaxes estudadas
- A atividade final integradora concluída

---

## Visão Geral do Curso

| Aula | Tema | Duração | Preparação (notebooks) | Prática em sala |
|---|---|---|---|---|
| 1 | Fundamentos, Tipos e Controle de Fluxo | 1h30min | AULA01, AULA02, AULA03 | Exercícios de expressões, `if/elif/else` e `while` |
| 2 | Estruturas de Dados, Funções e Bibliotecas | 1h30min | AULA04, AULA05, AULA06 | Estruturas, funções, importações e atividade final |
| **Total** | | **3h** | **6 notebooks** | **Exercícios progressivos + 1 atividade integradora** |

---

## Matriz de Cobertura dos Arquivos

| Arquivo | Conteúdo coberto | Forma de cobertura |
|---|---|---|
| `Python_AULA01.ipynb` | Ambiente e execução; comentários; variáveis; palavras reservadas; atribuição múltipla; tipos; strings; `print()`; `input()`; indentação; `dir()`; `__doc__`; exercícios iniciais | Estudo prévio + Aula 1, 25 min de prática |
| `Python_AULA02.ipynb` | Tipos e conversões; `bool("0")` e `bool(0)`; operadores matemáticos, relacionais e booleanos; tabelas-verdade; precedência; Bhaskara | Estudo prévio + Aula 1, 20 min de prática |
| `Python_AULA03.ipynb` | `if/elif/else`; `while`; contador; `break`; `continue`; exercícios de decisão e repetição | Estudo prévio + Aula 1, 35 min de prática |
| `Python_AULA04.ipynb` | Listas, operações e fatiamento; listas de listas; tuplas; conjuntos; dicionários; `for`; iteração de coleções | Estudo prévio + Aula 2, 35 min de prática |
| `Python_AULA05.ipynb` | Funções sem e com parâmetros; retorno; integração de funções; funções como objetos; `lambda`; `map()` | Estudo prévio + Aula 2, 23 min de prática |
| `Python_AULA06.ipynb` | Bibliotecas e módulos; PyPI; instalação; erros de pacote ausente; `import`; `as`; `from ... import`; `math`; `tinydb` | Estudo prévio + Aula 2, 12 min de prática + aplicação na atividade final |
| `ai_primeiro_contato.qmd` | Conceito de assistente de IA, conversa e apoio ao aprendizado de programação | Complementar assíncrono à AULA01; sem acréscimo de carga horária |
| `ai_revisao.qmd` | Revisão dos conceitos de Python com apoio de IA | Complementar assíncrono à AULA05; sem acréscimo de carga horária |
