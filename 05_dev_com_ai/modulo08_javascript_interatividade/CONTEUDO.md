# JavaScript + Interatividade + Dados na Tela

## Sobre o Conteúdo

Módulo que combina aula ativa (1h) e conteúdo assíncrono (até 2h), cobrindo os fundamentos de JavaScript aplicados à dashboard do projeto de integração. O aluno aprende a manipular o DOM, carregar dados gerados na trilha de ciência de dados e adicionar interatividade (filtros, eventos, validação), sempre seguindo o ciclo de trabalho com AI.

**Formato:** Leitura em Markdown (`.md`) + prática de codificação JavaScript
**Carga horária total:** 3h (1h aula ativa + até 2h assíncrono)
**Pré-requisitos:**
- Python (`01_python/`): variáveis, tipos, controle de fluxo, listas, dicionários, funções — base de lógica transferível para JS
- Visualização (`03_visualizacao/`): dados e gráficos que serão renderizados na dashboard
- Banco de Dados (`04_banco_dados/`): dados estruturados que alimentam a interface
- Módulo 6 — UX (`modulo06_ux_prototipacao_ai/`): wireframe e requisitos da dashboard
- Módulo 7 — HTML/CSS (`modulo07_html_css_com_ai/`): estrutura HTML/CSS já implementada
- Módulos de AI (`modulo01_*`, `modulo02_*`): template de requisitos, questionamento e revisão
**Instrutora responsável:** Larissa

---

## 🎯 Aula Ativa (1h)

### Bloco 1 — JS essencial: variáveis, funções, eventos (15 min)

#### JavaScript para quem já sabe Python

O aluno já conhece lógica de programação em Python (`01_python/`). JavaScript usa os mesmos conceitos com sintaxe diferente.

**Comparação rápida Python → JavaScript:**

| Conceito | Python | JavaScript |
|---|---|---|
| Variável | `nome = "Ana"` | `let nome = "Ana";` |
| Constante | (convenção `MAIÚSCULA`) | `const PI = 3.14;` |
| Função | `def somar(a, b):` | `function somar(a, b) {` |
| Arrow function | `lambda a, b: a + b` | `(a, b) => a + b` |
| Condicional | `if x > 10:` | `if (x > 10) {` |
| Loop for | `for item in lista:` | `for (let item of lista) {` |
| Lista/Array | `frutas = ["maçã", "uva"]` | `let frutas = ["maçã", "uva"];` |
| Dicionário/Objeto | `{"nome": "Ana", "idade": 20}` | `{ nome: "Ana", idade: 20 }` |
| Print/Log | `print("Olá")` | `console.log("Olá");` |
| Comentário | `# comentário` | `// comentário` |

**Diferenças importantes:**

- JavaScript usa `{}` para blocos (Python usa indentação)
- JavaScript usa `;` no final de cada instrução (opcional, mas recomendado)
- `let` para variáveis que mudam, `const` para constantes
- Arrays em JS têm métodos como `forEach()`, `map()`, `filter()` (similares a `for` e `map()` do Python)

#### Tipos de dados em JavaScript

| Tipo | Exemplo | Equivalente Python |
|---|---|---|
| `string` | `"texto"` ou `'texto'` | `str` |
| `number` | `42`, `3.14` | `int`, `float` |
| `boolean` | `true`, `false` | `True`, `False` |
| `array` | `[1, 2, 3]` | `list` |
| `object` | `{ chave: "valor" }` | `dict` |
| `null` | `null` | `None` |
| `undefined` | `undefined` | (sem equivalente direto) |

#### Funções

```javascript
// Função tradicional
function calcularMedia(valores) {
    let soma = 0;
    for (let valor of valores) {
        soma += valor;
    }
    return soma / valores.length;
}

// Arrow function (equivalente a lambda do Python)
const dobrar = (n) => n * 2;

// Usando métodos de array (similar a map() do Python)
const notas = [7, 8.5, 6, 9];
const dobradas = notas.map(n => n * 2);
```

#### Eventos

Eventos são ações do usuário (clique, digitação, seleção) que disparam funções no JavaScript.

```javascript
// Quando o botão for clicado, executa a função
const botao = document.querySelector("#meu-botao");
botao.addEventListener("click", function() {
    console.log("Botão clicado!");
});

// Versão com arrow function
botao.addEventListener("click", () => {
    console.log("Botão clicado!");
});
```

| Evento | Quando dispara | Uso na dashboard |
|---|---|---|
| `click` | Clique do mouse | Botão de filtrar, expandir gráfico |
| `change` | Valor de select/input muda | Dropdown de filtro |
| `input` | Usuário digita algo | Campo de busca |
| `submit` | Formulário enviado | Formulário de filtros |
| `DOMContentLoaded` | Página terminou de carregar | Carregar dados iniciais |

---

### Bloco 2 — DOM: selecionar e modificar elementos (10 min)

#### O que é o DOM?

O DOM (Document Object Model) é a representação da página HTML como uma **árvore de objetos** que o JavaScript pode ler e modificar.

```
document
└── html
    ├── head
    │   └── title
    └── body
        ├── header
        │   └── h1
        ├── main
        │   ├── section.kpis
        │   │   ├── article.kpi-card
        │   │   └── article.kpi-card
        │   └── section.grafico-principal
        └── footer
```

#### Selecionar elementos

| Método | O que seleciona | Exemplo |
|---|---|---|
| `querySelector()` | Primeiro elemento que casa | `document.querySelector(".kpi-card")` |
| `querySelectorAll()` | Todos que casam (NodeList) | `document.querySelectorAll(".kpi-card")` |
| `getElementById()` | Elemento por ID | `document.getElementById("titulo")` |

#### Modificar elementos

```javascript
// Mudar texto
const titulo = document.querySelector("h1");
titulo.textContent = "Dashboard Atualizada";

// Mudar HTML interno
const card = document.querySelector(".kpi-card .kpi-valor");
card.innerHTML = "<strong>2.350</strong>";

// Mudar estilo
card.style.color = "#4CAF50";

// Adicionar/remover classe CSS
card.classList.add("destaque");
card.classList.remove("destaque");

// Criar elemento novo
const novoCard = document.createElement("article");
novoCard.className = "kpi-card";
novoCard.innerHTML = `<h2>Novo KPI</h2><p class="kpi-valor">500</p>`;
document.querySelector(".kpis").appendChild(novoCard);
```

---

### Bloco 3 — Prática AI intensiva: carregar dados e renderizar (30 min)

O aluno carrega dados da trilha de ciência de dados e renderiza na dashboard usando o ciclo AI.

#### Dados da trilha de ciência de dados

No curso, os dados foram trabalhados em Python/Pandas (`03_visualizacao/`) e SQL (`04_banco_dados/`). Para usar no front end, esses dados podem ser representados como **array de objetos JavaScript** (equivalente a uma lista de dicionários do Python).

**Exemplo — dados de vendas (estrutura similar às usadas no curso):**

```javascript
const vendas = [
    { mes: "Jan", valor: 12500, categoria: "Eletrônicos" },
    { mes: "Fev", valor: 15800, categoria: "Eletrônicos" },
    { mes: "Mar", valor: 9200, categoria: "Roupas" },
    { mes: "Abr", valor: 18400, categoria: "Eletrônicos" },
    { mes: "Mai", valor: 11300, categoria: "Roupas" },
    { mes: "Jun", valor: 21000, categoria: "Eletrônicos" }
];
```

#### Prática em aula: renderizar tabela de dados

**Etapa 1 — Requisito:**

> **Contexto:** Estou construindo uma dashboard de dados em HTML, CSS e JavaScript puro. Já tenho a estrutura HTML/CSS do Módulo 7. Conheço Python (`for`, `map()`, listas, dicionários) e estou aprendendo a equivalência em JavaScript.
>
> **Objetivo:** Criar uma função que recebe um array de objetos (dados de vendas) e gera uma tabela HTML dentro de um `<section>` existente.
>
> **Detalhes:** A função deve criar `<table>`, `<thead>`, `<tbody>` e `<tr>/<td>` dinamicamente. Cada coluna é uma chave do objeto (mes, valor, categoria). A tabela deve ter classe CSS para estilização.
>
> **Restrições:** JavaScript puro. Sem bibliotecas, sem frameworks.
>
> **Formato:** Mostre o JavaScript e o HTML necessário. Não explique ainda.

**Etapa 2 — Gerar:**

O aluno recebe o código da AI e **lê antes de executar**.

**Etapa 3 — Aprender:**

> "Qual a diferença entre `forEach` e `map` neste caso?"
>
> "Por que usou `document.createElement` em vez de concatenar strings HTML?"
>
> "Como `Object.keys()` funciona? É parecido com `.keys()` do dicionário Python?"

**Etapa 4 — Revisar:**

> "Inseri um bug de propósito no código: troquei `tbody` por `thead`. A AI encontra?"
>
> "O que acontece se o array de dados estiver vazio?"
>
> "Gere 3 casos de teste para essa função."

#### Encerramento (5 min)

- Compartilhamento de 2–3 tabelas renderizadas
- Orientação para o conteúdo assíncrono: adicionar filtros e validação

---

## 📖 Conteúdo Assíncrono (até 2h)

### Parte 1 — Leitura: JavaScript essencial para quem já viu Python (20 min)

Objetivo: consolidar a equivalência Python → JavaScript como referência de consulta.

---

#### 1.1 Variáveis e constantes

```javascript
// let = variável que pode mudar (como variável Python normal)
let contador = 0;
contador = 1; // OK

// const = constante (como convenção MAIÚSCULA do Python)
const PI = 3.14159;
// PI = 3; // ERRO: não pode reatribuir

// var = evite usar (escopo problemático, legado)
```

**Quando usar cada um:**
- `const` por padrão (a maioria dos valores não precisa mudar)
- `let` quando o valor precisa mudar (contadores, acumuladores)
- `var` nunca (legado, comportamento de escopo confuso)

#### 1.2 Arrays e métodos essenciais

| Método JS | Equivalente Python | O que faz |
|---|---|---|
| `arr.push(item)` | `lista.append(item)` | Adiciona ao final |
| `arr.pop()` | `lista.pop()` | Remove do final |
| `arr.length` | `len(lista)` | Tamanho |
| `arr.includes(x)` | `x in lista` | Verifica se contém |
| `arr.indexOf(x)` | `lista.index(x)` | Posição do item |
| `arr.forEach(fn)` | `for item in lista:` | Percorre cada item |
| `arr.map(fn)` | `list(map(fn, lista))` | Transforma cada item |
| `arr.filter(fn)` | `[x for x in lista if ...]` | Filtra itens |
| `arr.reduce(fn, init)` | `functools.reduce(fn, lista, init)` | Reduz a um valor |
| `arr.find(fn)` | (sem equivalente direto) | Primeiro que satisfaz |
| `arr.sort()` | `lista.sort()` | Ordena (muta o array) |

**Exemplos com dados da dashboard:**

```javascript
const notas = [7, 8.5, 6, 9, 5.5, 10];

// Média (equivalente ao cálculo feito em 02_estatistica/)
const soma = notas.reduce((acc, nota) => acc + nota, 0);
const media = soma / notas.length;

// Filtrar aprovados (>= 7)
const aprovados = notas.filter(nota => nota >= 7);

// Transformar em texto
const textos = notas.map(nota => `Nota: ${nota}`);
```

#### 1.3 Objetos (equivalente a dicionários Python)

```javascript
// Criar objeto (= dict Python)
const aluno = {
    nome: "Ana",
    idade: 20,
    notas: [7, 8.5, 9]
};

// Acessar (= aluno["nome"] ou aluno.get("nome") em Python)
console.log(aluno.nome);       // "Ana"
console.log(aluno["idade"]);   // 20

// Iterar sobre chaves (= for chave in dicionario: em Python)
for (let chave of Object.keys(aluno)) {
    console.log(chave, aluno[chave]);
}

// Desestruturação (sem equivalente direto em Python)
const { nome, idade } = aluno;
```

#### 1.4 Template literals (equivalente a f-strings Python)

```javascript
// JavaScript — template literal com crases
const nome = "Ana";
const idade = 20;
console.log(`${nome} tem ${idade} anos`);

// Python — f-string (referência)
// print(f"{nome} tem {idade} anos")
```

---

### Parte 2 — Leitura: DOM para iniciantes com diagrama visual (20 min)

Objetivo: entender o DOM como a ponte entre HTML e JavaScript.

---

#### 2.1 O DOM é uma árvore

Cada tag HTML vira um **nó** na árvore do DOM. O JavaScript navega e modifica essa árvore.

```
                    document
                       │
                      html
                    /      \
                 head       body
                  │        /    \
                title   header   main
                          │      /   \
                         h1  section  section
                             (kpis)   (grafico)
                            /    \
                       article  article
                      (card 1) (card 2)
```

#### 2.2 Fluxo de trabalho com o DOM

```
1. SELECIONAR  →  2. LER/MODIFICAR  →  3. CRIAR/REMOVER
querySelector()    textContent           createElement()
querySelectorAll() innerHTML             appendChild()
getElementById()   style.color           removeChild()
                   classList.add()        
```

#### 2.3 Exemplo completo: atualizar KPI dinamicamente

```html
<!-- HTML (do Módulo 7) -->
<article class="kpi-card" id="kpi-total">
    <h2>Total de Registros</h2>
    <p class="kpi-valor">—</p>
</article>
```

```javascript
// JavaScript: calcular e exibir KPI a partir dos dados
const dados = [
    { id: 1, valor: 150 },
    { id: 2, valor: 230 },
    { id: 3, valor: 180 }
];

// Calcular total (similar a sum() em Python)
const total = dados.reduce((acc, item) => acc + item.valor, 0);

// Selecionar e atualizar o card
const kpiValor = document.querySelector("#kpi-total .kpi-valor");
kpiValor.textContent = total.toLocaleString("pt-BR");
// Resultado: "560" exibido no card
```

---

### Parte 3 — Tarefa: adicionar interatividade à dashboard (40 min)

Objetivo: adicionar filtros, eventos e interatividade à estrutura HTML/CSS criada no Módulo 7.

---

#### Instruções

1. Abra os arquivos `index.html` e `style.css` do Módulo 7
2. Crie um arquivo `script.js` e vincule-o ao HTML: `<script src="script.js" defer></script>`
3. Para cada funcionalidade abaixo, siga o ciclo AI: **Requisito → Gerar → Aprender → Revisar**

#### Funcionalidade 1 — Carregar dados e popular KPIs (15 min)

**Requisito para a AI:**

> **Contexto:** Tenho uma dashboard em HTML/CSS com cards de KPI (Módulo 7). Os KPIs estão com valores placeholder. Sei JavaScript básico: variáveis, funções, arrays, objetos e DOM.
>
> **Objetivo:** Criar um array de objetos simulando dados de vendas e uma função que calcula total, média e valor máximo, exibindo nos cards de KPI.
>
> **Detalhes:** Usar `document.querySelector` para selecionar os cards; usar `reduce`, `Math.max` e divisão para calcular as métricas. Executar a função quando a página carregar (`DOMContentLoaded`).
>
> **Restrições:** JavaScript puro. Sem bibliotecas.

**Ciclo AI:**
- **Aprender:** "Como `reduce` funciona passo a passo? É parecido com acumulador no `while` do Python?"
- **Revisar:** "O que acontece se o array estiver vazio? A divisão por zero é tratada?"

#### Funcionalidade 2 — Filtro por categoria com dropdown (15 min)

**Requisito para a AI:**

> **Contexto:** Já tenho dados de vendas em um array de objetos e uma tabela HTML gerada dinamicamente. Quero adicionar um dropdown de filtro.
>
> **Objetivo:** Criar um `<select>` com as categorias únicas dos dados. Quando o usuário selecionar uma categoria, a tabela deve ser atualizada mostrando apenas os dados daquela categoria. A opção "Todas" mostra todos os dados.
>
> **Detalhes:** Usar `filter()` para filtrar os dados; usar evento `change` no dropdown; reconstruir a tabela a cada filtro.
>
> **Restrições:** JavaScript puro. Sem bibliotecas.

**Ciclo AI:**
- **Aprender:** "Qual a diferença entre `filter` e `find`? Quando usar cada um?"
- **Revisar:** "O filtro funciona se a categoria tiver acento (ex.: 'Eletrônicos')?"

#### Funcionalidade 3 — Clique em botão para ordenar (10 min)

**Requisito para a AI:**

> **Contexto:** Já tenho tabela de dados funcionando com filtro. Quero adicionar um botão para ordenar os dados por valor.
>
> **Objetivo:** Botão que alterna entre ordenação crescente e decrescente por valor. A tabela é reconstruída a cada clique.
>
> **Restrições:** JavaScript puro. Sem bibliotecas.

**Ciclo AI:**
- **Aprender:** "Como o `sort()` funciona com arrow function? É parecido com `sort(key=lambda...)` do Python?"
- **Revisar:** "O botão indica visualmente a direção atual da ordenação?"

---

### Parte 4 — Prática AI: gerar validação de formulário, pedir testes, verificar (20 min)

Objetivo: praticar geração de código, testes e depuração com AI.

---

#### Instruções

**Etapa 1 — Gerar validação:**

> **Contexto:** Minha dashboard tem um formulário simples com campos: nome (texto) e valor mínimo (número). O formulário filtra os dados exibidos.
>
> **Objetivo:** Função de validação que verifica: nome não vazio, valor mínimo é número positivo. Se inválido, exibe mensagem de erro ao lado do campo.
>
> **Restrições:** JavaScript puro. Sem bibliotecas.

**Etapa 2 — Pedir testes:**

> "Gere 3 casos de teste para essa função de validação. Para cada teste, diga:
> 1. Qual entrada você usou
> 2. Qual resultado esperado
> 3. Qual resultado real
>
> Inclua: um caso válido, um com nome vazio e um com valor negativo."

**Etapa 3 — Verificar:**

O aluno executa manualmente os 3 testes e compara com o esperado.

**Etapa 4 — Depuração (desafio):**

O aluno insere um bug de propósito no código (ex.: trocar `>` por `>=` na validação) e pede à AI:

> "Inseri um bug nesta função de validação. O campo aceita valor 0 quando não deveria. Encontre o bug."

Avalie: a AI encontrou? Explicou corretamente?

---

### Parte 5 — Tabela-resumo do ciclo AI por habilidade (referência)

| Etapa | Habilidade | Exemplo concreto neste módulo |
|---|---|---|
| 1. Requisito | Escrever requisito | "Função que lê dados de vendas e gera tabela HTML" |
| 2. Gerar | Gerar com AI | Enviar requisito e receber JavaScript funcional |
| 3. Aprender | Pedir explicação | "Qual a diferença entre `forEach` e `map`?" |
| 4. Revisar | Depuração com AI | "Inseri um bug, a AI encontra?" |
| 4. Revisar | Pedir testes | "Gere 3 testes para essa função de filtro" |

---

## Resumo Geral

| # | Parte | Tipo | Duração |
|---|---|---|---|
| — | Aula ativa: JS essencial, DOM, prática AI (tabela de dados) | Presencial com instrutora | 1h |
| 1 | JavaScript essencial para quem já viu Python | Assíncrono — leitura | 20 min |
| 2 | DOM para iniciantes com diagrama visual | Assíncrono — leitura | 20 min |
| 3 | Adicionar interatividade à dashboard (KPIs, filtro, ordenação) | Assíncrono — tarefa prática | 40 min |
| 4 | Validação de formulário + testes com AI | Assíncrono — prática AI | 20 min |
| 5 | Tabela-resumo do ciclo AI | Referência | — |

---

## Referências

| Recurso | Localização |
|---|---|
| Notebooks de Python (Aulas 01–05) | `01_python/` |
| Conteúdo de Python | `01_python/CONTEUDO.md` |
| Plano de aula de Estatística | `02_estatistica/Plano_de_aula.md` |
| Conteúdo de Visualização de Dados | `03_visualizacao/CONTEUDO.md` |
| Conteúdo de Banco de Dados | `04_banco_dados/CONTEUDO.md` |
| Módulo 1 — Primeiro Contato com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| Módulo 2 — Revisão com AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Módulo 6 — UX e Prototipação | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
| Módulo 7 — HTML e CSS com AI | `05_dev_com_ai/modulo07_html_css_com_ai/` |
