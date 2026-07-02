# Plano de Aula — Revisão com AI (Conteúdo Assíncrono)

**Módulo:** 2 — Continuação de Python e Revisão com AI
**Tipo:** Conteúdo assíncrono (complementar à aula ativa de Python)
**Carga horária estimada:** até 2h
**Modalidade:** Assíncrona (estudo individual)
**Público-alvo:** Alunos do LabEduc que já estudaram os notebooks `Python_AULA01` a `Python_AULA05` e o conteúdo assíncrono do Módulo 1 de AI
**Pré-requisito:** Ter estudado variáveis, tipos, operadores, `if/elif/else`, `while`, listas, dicionários e funções (pasta `01_python`) e o Módulo 1 de AI (`05_dev_com_ai/modulo01_primeiro_contato_ai/`)
**Instrutor responsável:** Luis
**Modelo de aprendizagem:** Sala de aula invertida — este conteúdo assíncrono é consumido pelo aluno por conta própria, antes ou depois da aula ativa de Python (pasta `01_python`).

---

> **Importante para os alunos:** Este material é de estudo individual. Nos exercícios de depuração, tente encontrar os bugs sozinho **antes** de pedir ajuda à AI. No desafio de geração, revise o código **antes** de perguntar qualquer coisa. O objetivo é desenvolver senso crítico, não apenas obter respostas.

---

## Estrutura do Conteúdo Assíncrono

**Arquivo de referência:** `CONTEUDO.md` (nesta mesma pasta)

### Preparação

O aluno deve ter concluído o estudo dos seguintes materiais **antes** de iniciar este conteúdo:

| # | Material | Conteúdo |
|---|---|---|
| 1 | `Python_AULA01` | O que é Python; variáveis; strings; `print()`, `input()`; indentação |
| 2 | `Python_AULA02` | Tipos básicos; conversão; operadores matemáticos, relacionais e booleanos |
| 3 | `Python_AULA03` | `if/elif/else`; `while`; `break` e `continue` |
| 4 | `Python_AULA04` | Listas, tuplas, conjuntos, dicionários e laço `for` |
| 5 | `Python_AULA05` | Funções com `def`, parâmetros, retorno, escopo e `lambda` |
| 6 | Módulo 1 — AI | O que é um AI Assistant; como conversar; template de requisitos |

### Objetivo Geral

Desenvolver a habilidade de usar o AI Assistant para depurar, gerar e revisar código Python, formando um senso crítico sobre as respostas da AI.

### Objetivos Específicos

Ao final deste conteúdo, o aluno será capaz de:

- Identificar bugs em programas Python e usar a AI para validar suas hipóteses
- Avaliar criticamente se a AI acertou, errou ou deixou escapar problemas no código
- Gerar código com a AI a partir de um requisito detalhado e revisar o resultado antes de aceitar
- Questionar as escolhas da AI usando perguntas estruturadas sobre estrutura, dados e lógica

### Conteúdo

| Parte | Título | Tipo | Duração estimada |
|---|---|---|---|
| 1 | Prática AI: encontrar bugs com ajuda da AI | Exercício de depuração | 40 min |
| 2 | Desafio AI: gerar, revisar e questionar código | Desafio prático | 50 min |
| 3 | Como questionar a AI sobre o código dela | Leitura + guia de perguntas | 30 min |

---

## Detalhamento das Partes

### Parte 1 — Prática AI: Encontrar bugs com ajuda da AI (40 min)

**Objetivo:** Usar a AI como ferramenta de depuração e desenvolver a capacidade de avaliar se a análise da AI está correta.

**Dinâmica:**
1. O aluno tenta identificar os bugs sozinho
2. Cola o código no AI Assistant e pede para encontrar todos os bugs
3. Compara os resultados: a AI acertou? Deixou escapar? Apontou falsos positivos?

**Exercícios:**

| # | Programa | Bugs | Conceitos de `01_python` envolvidos |
|---|---|---|---|
| 1 | Calculadora de média | 3 bugs: falta de conversão de tipo, precedência de operadores, condição `>` vs `>=` | `input()`, `float()`, operadores, `if/else` — AULA01, AULA02, AULA03 |
| 2 | Contador regressivo | 3 bugs: incremento em vez de decremento, condição do `while`, loop infinito | `while`, operadores, variável contadora — AULA03 |
| 3 | Tradutor de frutas com dicionário | 3 bugs: grafia de chave, case sensitivity, falta de `:` no `else` | `dict`, `while True`, `break`, `if/else`, `in` — AULA03, AULA04 |

**Resultado esperado:** O aluno identifica bugs por conta própria, usa a AI para validar e sabe avaliar se a análise da AI está correta.

---

### Parte 2 — Desafio AI: Gerar código, revisar e questionar (50 min)

**Objetivo:** Praticar o ciclo completo: formular requisito → gerar código com AI → revisar → questionar escolhas.

**Dinâmica:**
1. O aluno envia um requisito detalhado para a AI (mini-quiz de conhecimentos gerais)
2. Recebe o código e **não executa imediatamente** — lê e tenta entender cada parte
3. Executa e testa com diferentes entradas
4. Questiona as escolhas da AI usando o guia de perguntas da Parte 3

**Requisito utilizado:** Programa de mini-quiz com 5 perguntas, 3 alternativas cada, contagem de acertos e mensagem de desempenho — usando apenas conceitos dos notebooks `Python_AULA01` a `Python_AULA05`.

**Resultado esperado:** O aluno sabe gerar código com AI usando requisitos estruturados (template do Módulo 1), revisar o resultado criticamente e formular perguntas de aprofundamento.

---

### Parte 3 — Leitura: Como questionar a AI sobre o código dela (30 min)

**Objetivo:** Fornecer um repertório de perguntas prontas para que o aluno questione decisões da AI em vez de aceitar tudo sem crítica.

**Tópicos:**
- Por que questionar a AI é essencial para o aprendizado
- Perguntas sobre estrutura do código
- Perguntas sobre escolhas de estruturas de dados
- Perguntas sobre lógica e fluxo de execução
- Perguntas sobre alternativas e simplificações
- Perguntas sobre erros e limitações
- Exemplo de conversa de questionamento (`for` vs. `while`)
- Dicas finais: não aceitar a primeira versão, testar antes de confiar, comparar com o que já sabe

**Resultado esperado:** O aluno tem um guia de referência para questionar qualquer código gerado pela AI e sabe quando pedir alternativas mais simples.

---

## Metodologia

- Estudo individual assíncrono com exercícios práticos
- Depuração manual seguida de validação com AI (Parte 1)
- Geração de código com requisito estruturado, revisão e questionamento (Parte 2)
- Leitura com guia de perguntas prontas reutilizável (Parte 3)
- Todos os exercícios se baseiam em conceitos já estudados na pasta `01_python` (AULA01 a AULA05)

## Recursos

- Arquivo `CONTEUDO.md` (nesta mesma pasta)
- Notebooks de referência: `Python_AULA01` a `Python_AULA05` (pasta `01_python`)
- Conteúdo do Módulo 1 de AI: `05_dev_com_ai/modulo01_primeiro_contato_ai/`
- AI Assistant à escolha do aluno (ChatGPT, Copilot, Gemini ou similar)
- Google Colab ou ambiente Python para testar os exercícios

## Cronograma Sugerido

| Bloco | Duração | Atividade |
|---|---|---|
| 0:00 – 0:15 | 15 min | **Prática AI (Programa 1):** Calculadora de média — encontrar bugs sozinho, pedir análise à AI, comparar resultados |
| 0:15 – 0:25 | 10 min | **Prática AI (Programa 2):** Contador regressivo — encontrar bugs sozinho, pedir análise à AI, comparar resultados |
| 0:25 – 0:40 | 15 min | **Prática AI (Programa 3):** Tradutor de frutas — encontrar bugs sozinho, pedir análise à AI, comparar resultados |
| 0:40 – 0:55 | 15 min | **Desafio AI (etapa 1):** Enviar requisito do mini-quiz à AI e receber o código |
| 0:55 – 1:15 | 20 min | **Desafio AI (etapa 2):** Revisar o código gerado, executar, testar com diferentes entradas |
| 1:15 – 1:30 | 15 min | **Desafio AI (etapa 3):** Questionar as escolhas da AI usando o guia de perguntas |
| 1:30 – 2:00 | 30 min | **Leitura (Parte 3):** Como questionar a AI sobre o código dela — leitura do guia e prática com as perguntas prontas |

## Avaliação

O aluno conclui este conteúdo assíncrono com:

- Análise dos 3 programas com bugs: para cada um, lista dos bugs encontrados sozinho vs. bugs apontados pela AI, com avaliação de acerto
- Código do mini-quiz gerado pela AI, revisado e testado pelo aluno
- Pelo menos 3 perguntas de questionamento feitas à AI sobre o código do mini-quiz, com as respostas obtidas

---

## Relação com Outros Módulos

| Componente | Descrição | Localização |
|---|---|---|
| Aula ativa (1h) | Continuação de Python — prática guiada com instrutor | `01_python/` |
| Conteúdo assíncrono (até 2h) | Revisão com AI — estudo individual | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Pré-requisito — Módulo 1 AI | Primeiro Contato com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
