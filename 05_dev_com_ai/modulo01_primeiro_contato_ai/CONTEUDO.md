# Primeiro Contato com AI — Conteúdo Assíncrono

## Sobre o Conteúdo

Conteúdo assíncrono complementar ao Módulo 1 (Lógica de Programação com Python). O aluno aprende o que é um AI Assistant, como interagir com ele de forma produtiva e como usá-lo para acelerar o aprendizado de programação — sempre a partir dos conceitos de Python já estudados nos notebooks da pasta `01_python`.

**Formato:** Leitura em Markdown (`.md`)
**Carga horária estimada:** até 2h (leitura + exercícios)
**Pré-requisito:** Ter estudado os notebooks `Python_AULA01` a `Python_AULA03` (variáveis, tipos, operadores, `if/elif/else` e `while`)
**Instrutor responsável:** Luis

---

## Parte 1 — O que é um AI Assistant e como conversar com ele

Objetivo: entender o que é um assistente de inteligência artificial, como ele funciona em alto nível e como formular pedidos claros para obter respostas úteis.

---

### 1.1 O que é um AI Assistant?

Um AI Assistant (assistente de inteligência artificial) é um programa que recebe texto como entrada e gera texto como resposta. Exemplos populares incluem ChatGPT, Copilot e Gemini.

**Características principais:**

- **Conversa em linguagem natural:** você escreve como se estivesse conversando com outra pessoa
- **Contexto da conversa:** o assistente lembra do que foi dito anteriormente na mesma conversa
- **Não é um buscador:** ele gera respostas com base em padrões aprendidos durante o treinamento, não pesquisa na internet em tempo real (a menos que tenha essa funcionalidade habilitada)
- **Pode errar:** a resposta nem sempre está correta — você deve sempre validar o resultado

### 1.2 O que um AI Assistant pode fazer por quem está aprendendo a programar?

- Explicar um trecho de código linha por linha
- Mostrar exemplos de uso de um comando ou função
- Ajudar a encontrar erros em um programa
- Sugerir formas diferentes de resolver o mesmo problema
- Traduzir conceitos técnicos para uma linguagem mais simples

### 1.3 O que um AI Assistant **não** faz bem

- Garantir que o código está 100% correto — sempre teste o resultado
- Substituir o entendimento do aluno — copiar sem entender não gera aprendizado
- Resolver problemas ambíguos sem contexto suficiente

### 1.4 Como conversar com um AI Assistant

**Boas práticas:**

- **Seja específico:** em vez de "me ajuda com Python", diga "explique o que o operador `%` faz em Python e dê um exemplo com números pares"
- **Dê contexto:** informe o que você já sabe, o que já tentou e qual resultado esperava
- **Peça passo a passo:** se a resposta for complexa, peça "explique linha por linha" ou "explique como se eu fosse iniciante"
- **Itere:** se a resposta não ficou clara, peça para reformular ou simplificar

**Exemplo de conversa ruim:**

> "Faz um programa de Bhaskara"

**Exemplo de conversa boa:**

> "Estou aprendendo Python e já sei usar `if/elif/else`, `input()` e `math.sqrt()`. Preciso de um programa que leia os coeficientes a, b e c de uma equação de 2º grau e calcule as raízes usando a fórmula de Bhaskara. Se o delta for negativo, deve exibir uma mensagem dizendo que não há raízes reais. Pode me mostrar o código e explicar cada parte?"

---

## Parte 2 — Exercícios: Resolver manualmente e depois pedir à AI que explique

Objetivo: praticar a resolução de problemas simples de Python e, em seguida, usar o AI Assistant para entender cada linha do código produzido.

**Instruções gerais:**

1. Resolva o exercício sozinho primeiro, usando o que aprendeu nos notebooks `Python_AULA01`, `Python_AULA02` e `Python_AULA03` (pasta `01_python`)
2. Depois de ter sua solução funcionando, cole o código no AI Assistant e peça: **"Explique este código linha por linha"**
3. Compare a explicação da AI com o que você entendeu — anote as diferenças

---

### Exercício 1 — Verificador de número par ou ímpar

**Enunciado:** Escreva um programa que leia um número inteiro com `input()` e imprima se ele é **par** ou **ímpar**.

**Conceitos envolvidos:** `input()`, `int()`, operador `%` (resto da divisão), `if/else`, `print()` — ver `Python_AULA01` e `Python_AULA03`.

**Depois de resolver:** Cole seu código no AI Assistant e peça:
> "Explique este código Python linha por linha. Eu sou iniciante e estou aprendendo sobre `if/else` e o operador `%`."

---

### Exercício 2 — Soma de números até o usuário digitar 0

**Enunciado:** Escreva um programa que leia números inteiros repetidamente com `input()` e vá acumulando a soma. Quando o usuário digitar `0`, o programa deve parar e exibir a soma total.

**Conceitos envolvidos:** `while`, `break`, variável acumuladora, `int()`, `input()`, `print()` — ver `Python_AULA03`.

**Depois de resolver:** Cole seu código no AI Assistant e peça:
> "Explique este código Python linha por linha. Quero entender como o `while` e o `break` funcionam juntos."

---

### Exercício 3 — Classificação de temperatura

**Enunciado:** Escreva um programa que leia uma temperatura em graus Celsius com `input()` e classifique:
- Abaixo de 0: **"Congelante"**
- De 0 a 15: **"Frio"**
- De 16 a 30: **"Agradável"**
- Acima de 30: **"Quente"**

**Conceitos envolvidos:** `input()`, `float()` ou `int()`, `if/elif/else`, operadores relacionais — ver `Python_AULA02` e `Python_AULA03`.

**Depois de resolver:** Cole seu código no AI Assistant e peça:
> "Explique este código Python linha por linha. Também me diga se existe uma forma melhor de escrever essas condições."

---

## Parte 3 — Mini-leitura: Como escrever bons requisitos para a AI

Objetivo: aprender a formular pedidos claros e completos para que o AI Assistant gere respostas mais úteis e precisas.

---

### 3.1 Por que os requisitos importam?

Assim como um programa precisa de uma entrada clara para produzir a saída correta, o AI Assistant precisa de um **pedido bem formulado** para gerar uma resposta útil. Quanto mais vago o pedido, mais genérica (e potencialmente inútil) será a resposta.

### 3.2 Template simples para escrever requisitos

Use este modelo sempre que for pedir algo ao AI Assistant:

```
1. CONTEXTO
   Descreva o que você está fazendo e o que já sabe.
   Exemplo: "Estou aprendendo Python e já sei usar variáveis, if/else e while."

2. OBJETIVO
   Diga exatamente o que você quer que a AI faça.
   Exemplo: "Quero um programa que leia notas de alunos e calcule a média."

3. DETALHES E RESTRIÇÕES
   Informe regras, limites ou preferências.
   Exemplo: "Use apenas input(), print() e while. Não use funções ou listas."

4. FORMATO DA RESPOSTA
   Diga como quer receber a resposta.
   Exemplo: "Mostre o código completo e explique cada linha."
```

### 3.3 Exemplos práticos

**Pedido ruim:**
> "Faz um programa de notas"

**Pedido bom (usando o template):**
> **Contexto:** Estou no curso de Python para Ciência de Dados e já estudei variáveis, tipos, operadores e `while` (notebooks `Python_AULA01` a `Python_AULA03`).
>
> **Objetivo:** Quero um programa que leia as notas de 5 alunos e diga qual é a maior nota e a menor nota.
>
> **Detalhes:** Use `input()` para ler as notas, `while` para repetir a leitura 5 vezes e variáveis para guardar a maior e a menor nota. Não use listas nem funções.
>
> **Formato:** Mostre o código completo e depois explique cada bloco.

### 3.4 Dicas finais

- **Comece simples:** não tente pedir tudo de uma vez. Peça o básico, teste, e depois peça melhorias
- **Revise sempre:** leia a resposta da AI com atenção, teste o código e questione o que não entendeu
- **Use a AI como tutora, não como atalho:** o objetivo é aprender, não entregar algo pronto sem entender
- **Itere:** se a resposta não ficou boa, reformule o pedido usando o template acima

---

## Resumo Geral

| # | Parte | Conteúdo |
|---|---|---|
| 1 | Texto | O que é um AI Assistant e como conversar com ele |
| 2 | Exercícios | 3 problemas de Python para resolver manualmente e pedir explicação à AI |
| 3 | Mini-leitura | Como escrever bons requisitos para a AI (template simples) |

---

## Referências

| Recurso | Localização |
|---|---|
| Notebooks de Python (Aulas 01–05) | `01_python/` |
| Conteúdo do módulo de Python | `01_python/CONTEUDO.md` |
| Plano de aula do módulo de Python | `01_python/PLANO_DE_AULA.md` |
