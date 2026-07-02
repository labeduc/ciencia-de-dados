# Revisão com AI — Conteúdo Assíncrono

## Sobre o Conteúdo

Conteúdo assíncrono complementar ao Módulo 2 (Continuação de Python). O aluno aprende a usar o AI Assistant como ferramenta de depuração, geração e revisão de código — desenvolvendo senso crítico para avaliar as respostas da AI e questionar suas escolhas. Todos os exercícios utilizam conceitos de Python já estudados nos notebooks da pasta `01_python`.

**Formato:** Leitura em Markdown (`.md`)
**Carga horária estimada:** até 2h (leitura + exercícios)
**Pré-requisito:** Ter estudado os notebooks `Python_AULA01` a `Python_AULA05` e o conteúdo do Módulo 1 de AI (`05_dev_com_ai/modulo01_primeiro_contato_ai/`)
**Instrutor responsável:** Luis

---

## Parte 1 — Prática AI: Encontrar bugs com ajuda da AI

Objetivo: desenvolver a habilidade de usar o AI Assistant para depurar código, e ao mesmo tempo avaliar criticamente se a AI identificou os problemas corretamente.

---

### Instruções gerais

1. Leia cada programa com atenção e tente **identificar os bugs sozinho** antes de usar a AI
2. Anote os bugs que você encontrou
3. Cole o código no AI Assistant e peça: **"Este código tem bugs. Encontre todos e explique cada um."**
4. Compare os bugs que a AI apontou com os que você encontrou
5. Avalie: a AI acertou? Deixou escapar algum? Apontou algo que não era bug?

---

### Programa 1 — Calculadora de média (3 bugs)

O programa abaixo deveria ler 3 notas, calcular a média e dizer se o aluno foi aprovado (média >= 7) ou reprovado.

**Conceitos envolvidos:** `input()`, `int()`, `float()`, operadores matemáticos, `if/else`, `print()` — ver `Python_AULA01`, `Python_AULA02`, `Python_AULA03`.

```python
nota1 = input("Digite a nota 1: ")
nota2 = input("Digite a nota 2: ")
nota3 = input("Digite a nota 3: ")

media = nota1 + nota2 + nota3 / 3

if media > 7:
    print("Aprovado com média" + media)
else:
    print("Reprovado")
```

**Bugs presentes:**
1. As notas não são convertidas para número (`float()` ou `int()`) — a soma concatena strings em vez de somar valores
2. Falta de parênteses na fórmula da média — a divisão por 3 se aplica apenas a `nota3` devido à precedência de operadores (deveria ser `(nota1 + nota2 + nota3) / 3`)
3. A condição de aprovação usa `>` em vez de `>=` — aluno com média exatamente 7 seria reprovado

> **Dica:** Há ainda um erro de execução na linha do `print("Aprovado com média" + media)` — não é possível concatenar `str` com `float` sem conversão. Verifique se a AI identifica este ponto também.

**Depois de avaliar, peça à AI:**
> "Corrija todos os bugs e mostre o código funcionando. Explique cada correção."

---

### Programa 2 — Contador regressivo (3 bugs)

O programa abaixo deveria fazer uma contagem regressiva de 10 até 1 e depois imprimir "Lançamento!".

**Conceitos envolvidos:** `while`, operadores relacionais, `print()`, variável contadora — ver `Python_AULA03`.

```python
contador = 10

while contador >= 0:
    print(contador)
    contador = contador + 1

print("Lançamento!")
```

**Bugs presentes:**
1. O incremento deveria ser decremento — `contador + 1` deveria ser `contador - 1`
2. A condição `>= 0` faz o programa imprimir `0`, mas a contagem deveria ir até 1 (deveria ser `>= 1` ou `> 0`)
3. Consequência do bug 1: o programa entra em loop infinito porque o contador nunca diminui

**Depois de avaliar, peça à AI:**
> "Corrija todos os bugs e mostre o código funcionando. Explique cada correção."

---

### Programa 3 — Tradutor de frutas com dicionário (3 bugs)

O programa abaixo deveria permitir que o usuário digite o nome de uma fruta em português e receba a tradução para inglês. O programa deve continuar pedindo frutas até o usuário digitar "sair".

**Conceitos envolvidos:** `dict`, `while True`, `break`, `input()`, `if/elif/else`, operador `in` — ver `Python_AULA03`, `Python_AULA04`.

```python
frutas = {"maça": "apple", "banana": "banana", "uva": "grape", "laranja": "orange"}

while True:
    fruta = input("Digite o nome da fruta (ou 'sair' para encerrar): ")

    if fruta == "Sair":
        break

    if fruta in frutas:
        print("A tradução de " + fruta + " é: " + frutas[fruta])
    else
        print("Fruta não encontrada no dicionário.")
```

**Bugs presentes:**
1. A chave `"maça"` está com grafia errada — deveria ser `"maçã"` (com til e cedilha), ou o enunciado deveria alertar sobre acentuação
2. A comparação `fruta == "Sair"` é sensível a maiúsculas/minúsculas — o usuário provavelmente digitará `"sair"` (minúsculo), então a comparação deveria ser `fruta == "sair"`
3. Falta `:` no `else` — deveria ser `else:` (erro de sintaxe)

**Depois de avaliar, peça à AI:**
> "Corrija todos os bugs e mostre o código funcionando. Explique cada correção."

---

## Parte 2 — Desafio AI: Gerar código, revisar e questionar

Objetivo: praticar a geração de código com AI usando um requisito detalhado, revisar o resultado e questionar as escolhas feitas pela AI.

---

### Instruções

1. Copie o requisito abaixo e envie ao AI Assistant
2. Leia o código gerado com atenção — **não execute imediatamente**
3. Tente entender cada linha antes de rodar
4. Execute o código e teste com diferentes entradas
5. Use as perguntas de questionamento (Parte 3) para aprofundar o entendimento

### Requisito para enviar à AI

> **Contexto:** Estou aprendendo Python e já sei usar variáveis, tipos, `if/elif/else`, `while`, listas, dicionários e funções com `def` (notebooks `Python_AULA01` a `Python_AULA05` do curso de Python para Ciência de Dados).
>
> **Objetivo:** Quero um programa que funcione como um mini-quiz de conhecimentos gerais. O programa deve:
> - Ter pelo menos 5 perguntas armazenadas em uma estrutura de dados
> - Cada pergunta deve ter 3 alternativas (a, b, c) e uma resposta correta
> - Apresentar as perguntas uma a uma e ler a resposta do usuário
> - Contar os acertos e, ao final, exibir a pontuação e uma mensagem de desempenho
>
> **Detalhes e Restrições:**
> - Use apenas o que eu já sei: variáveis, listas, dicionários, `for` ou `while`, `if/elif/else` e funções com `def`
> - Não use bibliotecas externas
> - Organize o código com pelo menos duas funções
>
> **Formato:** Mostre o código completo e funcional. Não explique ainda — vou revisar primeiro e depois fazer perguntas.

### Após receber o código, faça a revisão

Antes de perguntar qualquer coisa, responda para si mesmo:

- [ ] Consigo entender o que cada função faz?
- [ ] Entendo como os dados das perguntas estão armazenados (lista, dicionário, lista de dicionários)?
- [ ] O programa funciona quando testo com respostas corretas e incorretas?
- [ ] Há alguma parte do código que eu não usaria ou faria diferente?

### Depois da revisão, questione a AI

Use as perguntas da Parte 3 (abaixo) para questionar as escolhas feitas pela AI. Exemplos:

> "Por que você escolheu usar uma lista de dicionários em vez de só um dicionário?"
>
> "O que acontece se o usuário digitar uma letra maiúscula como resposta?"
>
> "Existe outra forma de organizar essas perguntas que seria mais simples?"

---

## Parte 3 — Leitura: Como questionar a AI sobre o código dela

Objetivo: aprender a fazer perguntas que aprofundam o entendimento do código gerado pela AI, em vez de aceitar tudo sem crítica.

---

### 3.1 Por que questionar?

Aceitar o código da AI sem questionar é como copiar a prova de um colega — você entrega, mas não aprende. Questionar faz você:

- Entender **por que** a AI fez cada escolha
- Descobrir alternativas que podem ser mais simples ou mais adequadas ao seu nível
- Identificar se a AI cometeu erros ou fez suposições que não combinam com o seu contexto

### 3.2 Guia de perguntas prontas

Use estas perguntas sempre que receber código da AI. Não precisa usar todas — escolha as que fazem sentido para o caso.

**Sobre a estrutura do código:**

- "Por que você organizou o código dessa forma?"
- "Qual é a vantagem de usar uma função aqui em vez de escrever tudo no corpo do programa?"
- "Teria como simplificar esse trecho sem perder funcionalidade?"

**Sobre escolhas de dados:**

- "Por que você usou um dicionário aqui e não uma lista?"
- "O que aconteceria se eu usasse uma tupla em vez de uma lista neste caso?"
- "Existe outra estrutura de dados que resolveria o mesmo problema?"

**Sobre lógica e fluxo:**

- "O que acontece se o usuário digitar algo inesperado (ex.: uma letra em vez de um número)?"
- "Esse `while` pode entrar em loop infinito? Em que situação?"
- "Por que a condição do `if` está escrita assim e não de outra forma?"

**Sobre alternativas:**

- "Você poderia reescrever esse trecho usando apenas o que eu já sei (`while`, `if`, listas)?"
- "Qual seria a versão mais simples possível desse programa?"
- "Se eu quisesse adicionar mais perguntas, o que precisaria mudar no código?"

**Sobre erros e limitações:**

- "Esse código tem algum bug que você não mencionou?"
- "O que acontece se a lista estiver vazia?"
- "Esse código funcionaria com entradas em maiúsculas e minúsculas?"

### 3.3 Exemplo de conversa de questionamento

**Você:** "Por que você usou `for pergunta in perguntas` em vez de `while`?"

**AI:** "O `for` é mais indicado quando sabemos quantos itens vamos iterar. Como a lista de perguntas tem tamanho fixo, o `for` percorre cada item automaticamente sem precisar de um contador manual."

**Você:** "E se eu quisesse que o quiz parasse quando o usuário errasse 3 vezes?"

**AI:** "Nesse caso, o `while` seria mais adequado, porque a condição de parada depende de algo que acontece durante a execução, não apenas do tamanho da lista."

### 3.4 Dicas finais

- **Não aceite a primeira versão:** peça melhorias, simplificações ou alternativas
- **Teste antes de confiar:** sempre execute o código e experimente entradas diferentes
- **Compare com o que você sabe:** se a AI usou algo que você ainda não aprendeu, peça para reescrever usando apenas o que você conhece (conceitos da pasta `01_python`)
- **Anote o que aprendeu:** registre as respostas mais úteis para consultar depois

---

## Resumo Geral

| # | Parte | Conteúdo | Duração estimada |
|---|---|---|---|
| 1 | Prática AI | 3 programas com bugs para depurar com ajuda da AI | 40 min |
| 2 | Desafio AI | Gerar código com requisito detalhado, revisar e questionar | 50 min |
| 3 | Leitura | Como questionar a AI sobre o código dela (guia com perguntas prontas) | 30 min |

---

## Referências

| Recurso | Localização |
|---|---|
| Notebooks de Python (Aulas 01–05) | `01_python/` |
| Conteúdo do módulo de Python | `01_python/CONTEUDO.md` |
| Plano de aula do módulo de Python | `01_python/PLANO_DE_AULA.md` |
| Módulo 1 — Primeiro Contato com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
