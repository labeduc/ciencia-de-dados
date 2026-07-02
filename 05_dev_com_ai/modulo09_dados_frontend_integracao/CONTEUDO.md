# Exibir e Organizar Dados no Frontend + Integração Completa com AI

## Sobre o Conteúdo

Módulo final da trilha de front end, que combina aula ativa (1h) e conteúdo assíncrono (até 2h). O aluno aprende a criar gráficos interativos com Chart.js a partir dos dados trabalhados ao longo de toda a trilha de ciência de dados, integra todas as peças do projeto (Python, Estatística, Visualização, Banco de Dados, UX, HTML/CSS, JavaScript) e executa o ciclo AI de forma **autônoma**, sem instrução passo a passo.

**Formato:** Leitura em Markdown (`.md`) + prática de codificação
**Carga horária total:** 3h (1h aula ativa + até 2h assíncrono)
**Pré-requisitos:**
- Python (`01_python/`): lógica, funções, listas e dicionários
- Estatística (`02_estatistica/`): médias, medianas, correlações, projeções
- Visualização (`03_visualizacao/`): tipos de gráficos × objetivo de comunicação, Pandas, Seaborn, Matplotlib, Plotly
- Banco de Dados (`04_banco_dados/`): SQL, consultas, modelagem relacional
- Módulo 6 — UX (`modulo06_*`): wireframe e requisitos da dashboard
- Módulo 7 — HTML/CSS (`modulo07_*`): estrutura HTML/CSS da dashboard
- Módulo 8 — JavaScript (`modulo08_*`): DOM, eventos, dados em array, filtros, tabelas dinâmicas
- Módulos de AI (`modulo01_*`, `modulo02_*`): ciclo Requisito → Gerar → Aprender → Revisar
**Instrutora responsável:** Larissa

---

## 🎯 Aula Ativa (1h)

### Bloco 1 — Criar gráficos a partir de dados com Chart.js (20 min)

#### O que é Chart.js?

Chart.js é uma biblioteca JavaScript gratuita e leve que cria gráficos interativos dentro de um elemento `<canvas>` no HTML. É a forma mais simples de trazer para o front end os mesmos tipos de gráficos que o aluno já criou com Seaborn, Matplotlib e Plotly na trilha de visualização (`03_visualizacao/`).

**Correspondência com a trilha de Visualização:**

| Tipo de gráfico | Seaborn/Matplotlib (`03_visualizacao/`) | Plotly (`03_visualizacao/`) | Chart.js (este módulo) |
|---|---|---|---|
| Barras | `countplot()`, `barplot()` — Aula 06 | `px.bar()` — Aula 15 | `type: 'bar'` |
| Linhas | `lineplot()` — Aula 07 | `px.line()` — Aula 15 | `type: 'line'` |
| Pizza | `plt.pie()` — Aula 09 | `px.pie()` — Aula 15 | `type: 'pie'` |
| Dispersão | `scatterplot()` — Aula 08 | `px.scatter()` — Aula 15 | `type: 'scatter'` |
| Área | `stackplot()` — Aula 07 | (Plotly area) | `type: 'line'` com `fill` |

#### Incluir Chart.js no projeto

```html
<!-- Adicionar no <head> do index.html -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
```

#### Estrutura básica de um gráfico

```html
<!-- HTML: canvas onde o gráfico será desenhado -->
<canvas id="grafico-vendas" width="400" height="200"></canvas>
```

```javascript
// JavaScript: criar gráfico de barras
const ctx = document.getElementById('grafico-vendas').getContext('2d');
const grafico = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Jan', 'Fev', 'Mar', 'Abr', 'Mai', 'Jun'],
        datasets: [{
            label: 'Vendas (R$)',
            data: [12500, 15800, 9200, 18400, 11300, 21000],
            backgroundColor: '#4CAF50'
        }]
    },
    options: {
        responsive: true,
        plugins: {
            title: {
                display: true,
                text: 'Vendas Mensais'
            }
        }
    }
});
```

**Anatomia do Chart.js:**

| Parte | O que configura |
|---|---|
| `type` | Tipo de gráfico: `'bar'`, `'line'`, `'pie'`, `'scatter'`, `'doughnut'` |
| `data.labels` | Rótulos do eixo X (ou fatias da pizza) |
| `data.datasets` | Arrays de dados, cada um com `label`, `data`, cores |
| `options` | Título, legenda, responsividade, escalas dos eixos |

---

### Bloco 2 — Idealizar a integração completa do projeto (10 min)

#### Mapa de integração

O aluno já construiu todas as peças. Agora é o momento de conectá-las:

```
┌─────────────────────────────────────────────────────────────┐
│                    PROJETO DE INTEGRAÇÃO                     │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  DADOS (origem)                                              │
│  ├── Python: lógica e funções (01_python/)                   │
│  ├── Estatística: métricas e análises (02_estatistica/)      │
│  ├── Visualização: tipos de gráficos (03_visualizacao/)      │
│  └── Banco de Dados: tabelas e SQL (04_banco_dados/)         │
│                                                              │
│  INTERFACE (destino)                                         │
│  ├── UX: wireframe e requisitos (modulo06)                   │
│  ├── HTML/CSS: estrutura e estilo (modulo07)                 │
│  ├── JavaScript: DOM, eventos, filtros (modulo08)            │
│  └── Chart.js: gráficos interativos (ESTE MÓDULO)           │
│                                                              │
│  AI (ferramenta transversal)                                 │
│  ├── Requisitos: template estruturado (modulo01)             │
│  ├── Revisão: questionar e depurar (modulo02)                │
│  └── Ciclo autônomo: definir → gerar → aprender → revisar   │
│                                                              │
├─────────────────────────────────────────────────────────────┤
│  ENTREGÁVEL FINAL                                            │
│  Dashboard funcional com dados reais, gráficos interativos,  │
│  filtros, KPIs dinâmicos e layout responsivo                 │
└─────────────────────────────────────────────────────────────┘
```

#### Checklist de integração

O aluno verifica quais peças já estão prontas e quais precisam ser finalizadas:

- [ ] **Dados:** array de objetos JS com dados compatíveis com a trilha de ciência de dados
- [ ] **KPIs:** cards populados dinamicamente (total, média, máximo — `02_estatistica/`)
- [ ] **Tabela:** dados renderizados em tabela HTML com filtro e ordenação (Módulo 8)
- [ ] **Gráficos:** pelo menos 2 gráficos Chart.js correspondentes às visualizações da trilha
- [ ] **Filtros:** dropdown ou botões que atualizam tabela e gráficos simultaneamente
- [ ] **Responsividade:** layout funciona em desktop e celular (Módulo 7)
- [ ] **Semântica/Acessibilidade:** HTML semântico, `alt`, `aria-label` (Módulo 7)

---

### Bloco 3 — Ciclo AI completo e autônomo (25 min)

Neste bloco, o aluno trabalha de forma **autônoma**. Não há instrução passo a passo — apenas o objetivo. O aluno decide o que construir, formula o requisito, gera com AI, aprende e revisa por conta própria.

#### Dinâmica

1. O aluno escolhe **uma feature** que sua dashboard ainda não tem (gráfico, filtro, estado visual, etc.)
2. Executa o ciclo completo sozinho:

| Etapa | O aluno faz |
|---|---|
| 1. Definir | Decide a feature e escreve o requisito usando o template do Módulo 1 |
| 2. Gerar | Envia à AI e recebe o código |
| 3. Aprender | Faz pelo menos 2 perguntas sobre as escolhas da AI |
| 4. Revisar | Pede revisão de acessibilidade, responsividade ou performance |
| 5. Testar | Testa com dados reais e pede à AI pelo menos 2 casos de teste |

3. A instrutora circula e observa, mas **não direciona** — apenas auxilia se o aluno travar

#### Sugestões de features para o ciclo autônomo

| Feature | Complexidade | Conceitos |
|---|---|---|
| Gráfico de linhas de tendência | Média | Chart.js `type: 'line'`, dados temporais |
| Gráfico de pizza de distribuição por categoria | Média | Chart.js `type: 'pie'`, `reduce` para agrupar |
| Filtro que atualiza gráfico e tabela ao mesmo tempo | Alta | `addEventListener`, recriação de Chart, filtro de array |
| Tooltip customizado no gráfico | Média | Chart.js `options.plugins.tooltip` |
| Card de KPI com indicador de variação (↑ ↓) | Média | Cálculo de diferença, `classList` para cor |

#### Encerramento (5 min)

- 2–3 alunos apresentam a feature que construíram
- Orientação para o conteúdo assíncrono: implementar todos os gráficos pertinentes

---

## 📖 Conteúdo Assíncrono (até 2h)

### Parte 1 — Leitura: Chart.js essencial com 3 tipos de gráfico (30 min)

Objetivo: dominar a criação de gráficos de barras, linhas e pizza com Chart.js, fazendo a ponte com os gráficos já criados na trilha de visualização.

---

#### 1.1 Gráfico de barras

Equivalente a `countplot()`/`barplot()` do Seaborn (Aula 06) e `px.bar()` do Plotly (Aula 15).

```javascript
// Dados: quantidade de itens por categoria
// (similar a groupby().count() do Pandas — 03_visualizacao/, Aula 05)
const dadosCategorias = {
    labels: ['Eletrônicos', 'Roupas', 'Alimentos', 'Livros'],
    datasets: [{
        label: 'Quantidade de Produtos',
        data: [45, 82, 63, 29],
        backgroundColor: ['#4CAF50', '#2196F3', '#FF9800', '#9C27B0']
    }]
};

new Chart(document.getElementById('grafico-categorias').getContext('2d'), {
    type: 'bar',
    data: dadosCategorias,
    options: {
        responsive: true,
        plugins: {
            title: { display: true, text: 'Produtos por Categoria' },
            legend: { display: false }
        },
        scales: {
            y: { beginAtZero: true }
        }
    }
});
```

**Variações:**
- Barras horizontais: `indexAxis: 'y'` nas options
- Barras agrupadas: múltiplos objetos no array `datasets` (equivalente a `hue` do Seaborn)
- Barras empilhadas: `options.scales.x.stacked: true` e `options.scales.y.stacked: true`

#### 1.2 Gráfico de linhas

Equivalente a `lineplot()` do Seaborn (Aula 07) e `px.line()` do Plotly (Aula 15).

```javascript
// Dados: evolução mensal de vendas
// (similar a dados temporais trabalhados em 03_visualizacao/, Aula 07)
const dadosTendencia = {
    labels: ['Jan', 'Fev', 'Mar', 'Abr', 'Mai', 'Jun'],
    datasets: [{
        label: 'Vendas 2024',
        data: [12500, 15800, 9200, 18400, 11300, 21000],
        borderColor: '#2196F3',
        backgroundColor: 'rgba(33, 150, 243, 0.1)',
        fill: true,
        tension: 0.3
    }]
};

new Chart(document.getElementById('grafico-tendencia').getContext('2d'), {
    type: 'line',
    data: dadosTendencia,
    options: {
        responsive: true,
        plugins: {
            title: { display: true, text: 'Tendência de Vendas' }
        }
    }
});
```

**Variações:**
- Sem preenchimento: `fill: false`
- Linha reta: `tension: 0`
- Múltiplas séries: múltiplos objetos no array `datasets`
- Área empilhada: `fill: true` + `stacked: true` nos scales

#### 1.3 Gráfico de pizza / rosca

Equivalente a `plt.pie()` do Matplotlib (Aula 09) e `px.pie()` do Plotly (Aula 15).

```javascript
// Dados: distribuição de vendas por região
const dadosDistribuicao = {
    labels: ['Sudeste', 'Sul', 'Nordeste', 'Norte', 'Centro-Oeste'],
    datasets: [{
        data: [42, 23, 20, 8, 7],
        backgroundColor: ['#4CAF50', '#2196F3', '#FF9800', '#9C27B0', '#F44336']
    }]
};

// Pizza
new Chart(document.getElementById('grafico-pizza').getContext('2d'), {
    type: 'pie',
    data: dadosDistribuicao,
    options: {
        responsive: true,
        plugins: {
            title: { display: true, text: 'Vendas por Região (%)' }
        }
    }
});

// Rosca (doughnut) — mesma estrutura, tipo diferente
new Chart(document.getElementById('grafico-rosca').getContext('2d'), {
    type: 'doughnut',
    data: dadosDistribuicao
});
```

**Quando usar pizza vs. barras (referência: `03_visualizacao/`, Aula 09):**
- Pizza: 3–5 fatias no máximo, quando a proporção importa mais que o valor absoluto
- Barras: muitas categorias, quando a comparação exata importa

#### 1.4 Preparar dados para Chart.js a partir da trilha

Os dados trabalhados na trilha de ciência de dados (Python/Pandas, SQL) podem ser convertidos para o formato que o Chart.js espera:

```javascript
// Dados brutos (similar ao que viria de uma consulta SQL ou DataFrame)
const vendas = [
    { mes: "Jan", valor: 12500, categoria: "Eletrônicos" },
    { mes: "Fev", valor: 15800, categoria: "Eletrônicos" },
    { mes: "Mar", valor: 9200, categoria: "Roupas" },
    { mes: "Abr", valor: 18400, categoria: "Eletrônicos" },
    { mes: "Mai", valor: 11300, categoria: "Roupas" },
    { mes: "Jun", valor: 21000, categoria: "Eletrônicos" }
];

// Extrair labels e dados para Chart.js
// (equivalente a df["mes"].tolist() e df["valor"].tolist() do Pandas)
const labels = vendas.map(v => v.mes);
const valores = vendas.map(v => v.valor);

// Agrupar por categoria para gráfico de pizza
// (equivalente a df.groupby("categoria")["valor"].sum() do Pandas)
const porCategoria = vendas.reduce((acc, v) => {
    acc[v.categoria] = (acc[v.categoria] || 0) + v.valor;
    return acc;
}, {});
// Resultado: { Eletrônicos: 67700, Roupas: 20500 }
```

---

### Parte 2 — Tarefa: implementar gráficos pertinentes à análise de dados (40 min)

Objetivo: implementar na dashboard todos os gráficos que sejam relevantes para a análise de dados da trilha de ciência de dados, usando o ciclo AI de forma autônoma.

---

#### Instruções

1. Revise os tipos de gráficos que você criou na trilha de visualização (`03_visualizacao/`):
   - Quais gráficos fazem sentido para os seus dados?
   - Quais métricas estatísticas (`02_estatistica/`) precisam ser exibidas?
   - Quais consultas SQL (`04_banco_dados/`) alimentam cada gráfico?

2. Consulte o wireframe do Módulo 6 — cada área de gráfico tem um requisito associado

3. Implemente cada gráfico usando o ciclo AI de forma **autônoma** — você decide o requisito, as perguntas e a revisão

#### Gráficos sugeridos (escolha pelo menos 3)

| Gráfico | Tipo Chart.js | Dado da trilha | Referência |
|---|---|---|---|
| Vendas/contagens ao longo do tempo | `line` | Séries temporais | `03_visualizacao/`, Aula 07 |
| Distribuição por categoria | `bar` | Agrupamento por categoria | `03_visualizacao/`, Aula 06 |
| Proporção de categorias | `pie` ou `doughnut` | Composição percentual | `03_visualizacao/`, Aula 09 |
| Comparação entre métricas | `bar` agrupado | Múltiplas métricas lado a lado | `03_visualizacao/`, Aula 06 |
| Correlação entre variáveis | `scatter` | Dispersão de duas variáveis | `03_visualizacao/`, Aula 08 |

#### Para cada gráfico (ciclo autônomo)

O aluno executa sozinho:

1. **Definir:** que dado esse gráfico mostra e por que é relevante
2. **Requisito:** escrever e enviar à AI
3. **Gerar:** receber o código
4. **Aprender:** fazer pelo menos 1 pergunta ("Por que esse tipo de gráfico?", "Como mudar as cores?")
5. **Revisar:** "O gráfico é responsivo?", "O tooltip mostra informação útil?"
6. **Integrar:** conectar com os filtros do Módulo 8 (se aplicável)

---

### Parte 3 — Refinamentos com AI: filtros, loading e tratamento de erros (30 min)

Objetivo: polir a dashboard com refinamentos de UX que a AI pode ajudar a implementar.

---

#### 3.1 Filtros interativos que atualizam gráficos

Quando o aluno muda um filtro (dropdown do Módulo 8), os gráficos Chart.js precisam ser atualizados.

**Requisito sugerido para a AI:**

> **Contexto:** Minha dashboard tem um dropdown de filtro por categoria (Módulo 8) e gráficos Chart.js. Quando o filtro muda, a tabela já é atualizada, mas os gráficos não.
>
> **Objetivo:** Quando o usuário selecionar uma categoria no dropdown, os gráficos devem ser atualizados com os dados filtrados.
>
> **Detalhes:** Preciso destruir o gráfico antigo (`chart.destroy()`) e criar um novo com os dados filtrados, ou atualizar os dados existentes (`chart.data.datasets[0].data = novosDados; chart.update()`).
>
> **Pergunta:** Qual abordagem é melhor: destruir e recriar ou atualizar dados? Por quê?

#### 3.2 Estado de loading

Enquanto os dados são processados ou os gráficos são renderizados, o usuário deve ver um indicador visual.

**Exemplo simples:**

```html
<div id="loading" class="loading">Carregando dados...</div>
```

```css
.loading {
    text-align: center;
    padding: 40px;
    color: #888;
    font-style: italic;
}
.loading.oculto {
    display: none;
}
```

```javascript
// Mostrar loading
document.getElementById('loading').classList.remove('oculto');

// Processar dados e criar gráficos...

// Esconder loading
document.getElementById('loading').classList.add('oculto');
```

#### 3.3 Tratamento de erros

O que acontece se os dados estiverem vazios ou com formato errado?

**Requisito sugerido para a AI:**

> **Contexto:** Minha dashboard renderiza gráficos a partir de um array de dados. Preciso tratar casos em que os dados estão vazios ou inválidos.
>
> **Objetivo:** Se o array estiver vazio, exibir uma mensagem "Nenhum dado encontrado" no lugar do gráfico. Se um valor não for número, ignorar aquele registro.
>
> **Pergunta:** Como validar os dados antes de passar para o Chart.js?

---

### Parte 4 — Autoavaliação: "O que consegui fazer sozinho vs. o que a AI fez por mim?" (20 min)

Objetivo: desenvolver consciência sobre o aprendizado real — o que o aluno internalizou vs. o que apenas copiou.

---

#### 4.1 Questionário de autoavaliação

Para cada item, marque honestamente:

**HTML/CSS (Módulo 7)**

| Habilidade | Consigo fazer sozinho | Preciso da AI | Não sei fazer |
|---|---|---|---|
| Criar estrutura HTML com tags semânticas | ☐ | ☐ | ☐ |
| Estilizar com flexbox (direção, alinhamento, gap) | ☐ | ☐ | ☐ |
| Fazer layout responsivo com media queries | ☐ | ☐ | ☐ |
| Verificar acessibilidade (alt, aria, contraste) | ☐ | ☐ | ☐ |

**JavaScript (Módulo 8)**

| Habilidade | Consigo fazer sozinho | Preciso da AI | Não sei fazer |
|---|---|---|---|
| Declarar variáveis e criar funções | ☐ | ☐ | ☐ |
| Selecionar e modificar elementos do DOM | ☐ | ☐ | ☐ |
| Usar `forEach`, `map`, `filter` em arrays | ☐ | ☐ | ☐ |
| Adicionar evento de clique ou change | ☐ | ☐ | ☐ |
| Gerar tabela HTML a partir de dados | ☐ | ☐ | ☐ |

**Chart.js (Este módulo)**

| Habilidade | Consigo fazer sozinho | Preciso da AI | Não sei fazer |
|---|---|---|---|
| Criar gráfico de barras básico | ☐ | ☐ | ☐ |
| Criar gráfico de linhas com múltiplas séries | ☐ | ☐ | ☐ |
| Criar gráfico de pizza/rosca | ☐ | ☐ | ☐ |
| Atualizar gráfico quando filtro muda | ☐ | ☐ | ☐ |
| Preparar dados (map, reduce) para o Chart.js | ☐ | ☐ | ☐ |

**Uso da AI**

| Habilidade | Consigo fazer sozinho | Preciso de ajuda | Não sei fazer |
|---|---|---|---|
| Escrever requisito claro e completo | ☐ | ☐ | ☐ |
| Questionar escolhas da AI | ☐ | ☐ | ☐ |
| Identificar quando a AI errou | ☐ | ☐ | ☐ |
| Pedir testes e verificar resultados | ☐ | ☐ | ☐ |

#### 4.2 Reflexão

Responda por escrito (2–3 frases cada):

1. **Qual foi a parte mais difícil?** O que travou você e como resolveu?
2. **O que a AI fez melhor que você?** Em que situações a AI foi claramente mais rápida ou precisa?
3. **O que você fez melhor que a AI?** Quando sua decisão foi melhor que a sugestão da AI?
4. **O que você aprenderia diferente?** Se fosse começar de novo, o que faria de forma diferente?

#### 4.3 Plano de estudo pós-curso

Com base na autoavaliação, liste:

- **3 habilidades que quero praticar mais** (as que marcou "Preciso da AI")
- **1 projeto pessoal** onde posso aplicar o que aprendi
- **1 recurso** (tutorial, documentação, curso) para cada habilidade que quero fortalecer

---

## Resumo Geral

| # | Parte | Tipo | Duração |
|---|---|---|---|
| — | Aula ativa: Chart.js, integração, ciclo AI autônomo | Presencial com instrutora | 1h |
| 1 | Chart.js essencial: barras, linhas, pizza | Assíncrono — leitura | 30 min |
| 2 | Implementar gráficos pertinentes à trilha | Assíncrono — tarefa prática | 40 min |
| 3 | Refinamentos: filtros, loading, erros | Assíncrono — prática com AI | 30 min |
| 4 | Autoavaliação | Assíncrono — reflexão | 20 min |

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
| Módulo 7 — HTML e CSS | `05_dev_com_ai/modulo07_html_css_com_ai/` |
| Módulo 8 — JavaScript e Interatividade | `05_dev_com_ai/modulo08_javascript_interatividade/` |
| Chart.js — Documentação oficial | https://www.chartjs.org/docs/ |
