# HTML e CSS com AI Assistants

## Sobre o Conteúdo

Módulo que combina aula ativa (1h) e conteúdo assíncrono (até 2h), cobrindo os fundamentos de HTML semântico e CSS essencial aplicados à construção da dashboard de dados projetada no Módulo 6. O aluno aprende a estruturar páginas e estilizá-las seguindo um ciclo de trabalho com AI: **Requisito → Gerar → Aprender → Revisar**.

**Formato:** Leitura em Markdown (`.md`) + prática de codificação HTML/CSS
**Carga horária total:** 3h (1h aula ativa + até 2h assíncrono)
**Pré-requisitos:**
- Python (`01_python/`): lógica e funções (base de programação)
- Visualização (`03_visualizacao/`): tipos de gráficos e boas práticas visuais
- Módulo 6 — UX (`05_dev_com_ai/modulo06_ux_prototipacao_ai/`): wireframe da dashboard e requisitos escritos por seção
- Módulos de AI anteriores (`modulo01_*`, `modulo02_*`): template de requisitos, questionamento de respostas
**Instrutora responsável:** Larissa

---

## 🎯 Aula Ativa (1h)

### Bloco 1 — HTML semântico: estrutura da página (15 min)

#### O que é HTML?

HTML (HyperText Markup Language) é a linguagem que define a **estrutura** de uma página web. Não é uma linguagem de programação — é uma linguagem de **marcação** que organiza o conteúdo em elementos.

#### Tags essenciais

| Tag | Função | Exemplo de uso na dashboard |
|---|---|---|
| `<header>` | Cabeçalho da página | Título da dashboard + filtros |
| `<nav>` | Navegação | Menu lateral ou abas de seções |
| `<main>` | Conteúdo principal | Área de KPIs e gráficos |
| `<section>` | Agrupamento temático | Seção de KPIs, seção de gráficos |
| `<article>` | Conteúdo independente | Card de KPI individual |
| `<footer>` | Rodapé | Fonte de dados, créditos |
| `<h1>` a `<h6>` | Títulos hierárquicos | Título da dashboard (`h1`), título de seção (`h2`) |
| `<p>` | Parágrafo de texto | Descrição de um KPI |
| `<div>` | Container genérico | Wrapper de layout (quando não há tag semântica) |
| `<span>` | Container inline | Destaque de valor numérico dentro de texto |

#### O que é HTML semântico?

HTML semântico significa usar a **tag certa para o propósito certo**, em vez de usar `<div>` para tudo. Isso importa porque:

- **Acessibilidade:** leitores de tela usam as tags para navegar (ex.: pular direto para o `<main>`)
- **SEO:** mecanismos de busca entendem melhor a estrutura da página
- **Manutenção:** outro desenvolvedor lê `<header>` e sabe que é o cabeçalho, sem precisar ler o CSS

**Exemplo — estrutura da dashboard do Módulo 6:**

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard — Projeto de Integração</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Dashboard — Projeto de Integração</h1>
        <!-- Área de filtros -->
    </header>

    <main>
        <section class="kpis">
            <article class="kpi-card">
                <h2>Total de Registros</h2>
                <p class="kpi-valor">1.847</p>
            </article>
            <!-- Mais cards de KPI -->
        </section>

        <section class="grafico-principal">
            <h2>Tendência ao Longo do Tempo</h2>
            <!-- Espaço para gráfico -->
        </section>

        <section class="graficos-secundarios">
            <!-- Gráficos complementares -->
        </section>
    </main>

    <footer>
        <p>Fonte: banco de dados do projeto de integração</p>
    </footer>
</body>
</html>
```

---

### Bloco 2 — CSS essencial: box model, flexbox, responsividade (15 min)

#### O que é CSS?

CSS (Cascading Style Sheets) é a linguagem que define a **aparência** de uma página HTML — cores, tamanhos, espaçamentos, posicionamento.

#### Box model

Todo elemento HTML é uma **caixa** com 4 camadas:

```
┌─────────────────────────────────────┐
│            margin                   │
│  ┌───────────────────────────────┐  │
│  │         border                │  │
│  │  ┌─────────────────────────┐  │  │
│  │  │       padding           │  │  │
│  │  │  ┌───────────────────┐  │  │  │
│  │  │  │    conteúdo        │  │  │  │
│  │  │  └───────────────────┘  │  │  │
│  │  └─────────────────────────┘  │  │
│  └───────────────────────────────┘  │
└─────────────────────────────────────┘
```

| Propriedade | O que faz | Exemplo |
|---|---|---|
| `margin` | Espaço **externo** entre elementos | `margin: 16px;` |
| `border` | Borda ao redor do elemento | `border: 2px solid #333;` |
| `padding` | Espaço **interno** entre borda e conteúdo | `padding: 12px;` |
| `width` / `height` | Largura e altura do conteúdo | `width: 300px;` |

**Dica:** Use `box-sizing: border-box;` para que `width` inclua padding e border (evita surpresas de tamanho).

#### Flexbox

Flexbox é o sistema de layout que organiza elementos **em linha ou em coluna**, distribuindo espaço automaticamente.

```css
.kpis {
    display: flex;          /* ativa o flexbox */
    gap: 16px;              /* espaço entre os cards */
    justify-content: center; /* centraliza horizontalmente */
    flex-wrap: wrap;        /* quebra linha se não couber */
}
```

| Propriedade | O que faz |
|---|---|
| `display: flex` | Ativa flexbox no container |
| `flex-direction` | Define a direção: `row` (padrão) ou `column` |
| `justify-content` | Alinha na direção principal (`center`, `space-between`, `flex-start`) |
| `align-items` | Alinha na direção transversal (`center`, `stretch`, `flex-start`) |
| `gap` | Espaço entre os itens |
| `flex-wrap: wrap` | Permite que itens quebrem para a próxima linha |

#### Responsividade básica

Responsividade significa que a página se adapta a **diferentes tamanhos de tela** (desktop, tablet, celular).

```css
/* Desktop: 3 cards lado a lado */
.kpi-card {
    flex: 1 1 250px; /* cresce, encolhe, base de 250px */
}

/* Celular: cards empilhados */
@media (max-width: 768px) {
    .kpis {
        flex-direction: column;
    }
}
```

**Conceitos-chave:**
- `@media (max-width: 768px)` — aplica estilos apenas quando a tela é menor que 768px
- `flex-wrap: wrap` — itens "caem" para a próxima linha automaticamente
- Unidades relativas (`%`, `rem`, `vw`) se adaptam melhor que unidades fixas (`px`)

---

### Bloco 3 — Prática AI intensiva (25 min)

O aluno pratica o ciclo completo de trabalho com AI para construir um componente real da dashboard.

#### O ciclo: Requisito → Gerar → Aprender → Revisar

| Etapa | Habilidade | O que o aluno faz |
|---|---|---|
| 1. Requisito | Escrever requisito | Descreve o componente desejado em texto detalhado |
| 2. Gerar | Gerar com AI | Envia à AI e recebe HTML + CSS |
| 3. Aprender | Pedir explicação | Questiona as escolhas da AI ("Por que usou flexbox aqui?") |
| 4. Revisar | Pedir revisão | Solicita revisão de semântica, acessibilidade e responsividade |

#### Prática em aula: Card de KPI

**Etapa 1 — Requisito:**

O aluno escreve e envia à AI:

> **Contexto:** Estou construindo uma dashboard de dados em HTML e CSS puro. Sei usar tags semânticas (`header`, `main`, `section`, `article`), box model, flexbox e media queries básicas.
>
> **Objetivo:** Criar um card de KPI (indicador-chave) para a minha dashboard.
>
> **Detalhes:** O card deve ter um título curto (ex.: "Total de Registros"), um número grande em destaque (ex.: "1.847"), uma borda colorida à esquerda e ser responsivo (no celular, ocupa 100% da largura).
>
> **Restrições:** Apenas HTML semântico e CSS puro. Sem JavaScript, sem frameworks, sem bibliotecas.
>
> **Formato:** Mostre o HTML e o CSS separados. Não explique ainda.

**Etapa 2 — Gerar:**

O aluno recebe o código da AI e **lê antes de executar**.

**Etapa 3 — Aprender:**

O aluno pergunta à AI:

> "Por que você usou `flexbox` aqui em vez de só `text-align`?"
>
> "O que o `flex: 1 1 250px` faz exatamente?"
>
> "Por que usou `article` em vez de `div` para o card?"

**Etapa 4 — Revisar:**

O aluno pede à AI:

> "Revise meu HTML quanto a semântica e acessibilidade. O que um leitor de tela leria neste card? Há algo que eu deveria melhorar?"
>
> "Teste mentalmente este layout no celular (tela de 375px). O que quebraria?"

#### Encerramento da aula (5 min)

- Compartilhamento de 2–3 cards criados
- Orientação para o conteúdo assíncrono: aplicar o ciclo a cada seção do wireframe

---

## 📖 Conteúdo Assíncrono (até 2h)

### Parte 1 — Leitura: Guia visual HTML + CSS (30 min)

Objetivo: consolidar os conceitos de HTML e CSS com exemplos visuais e interativos.

---

#### 1.1 HTML — Referência rápida

**Estrutura mínima de uma página:**

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Conteúdo vai aqui -->
</body>
</html>
```

**Tags semânticas — quando usar cada uma:**

| Situação | ❌ Genérico | ✅ Semântico |
|---|---|---|
| Cabeçalho da página | `<div class="header">` | `<header>` |
| Menu de navegação | `<div class="menu">` | `<nav>` |
| Conteúdo principal | `<div class="content">` | `<main>` |
| Grupo de conteúdo relacionado | `<div class="section">` | `<section>` |
| Conteúdo independente (card) | `<div class="card">` | `<article>` |
| Rodapé | `<div class="footer">` | `<footer>` |

**Atributos essenciais para acessibilidade:**

| Atributo | Onde usar | Para que serve |
|---|---|---|
| `lang="pt-BR"` | `<html>` | Informa o idioma da página ao leitor de tela |
| `alt="descrição"` | `<img>` | Texto alternativo para imagens (lido pelo leitor de tela) |
| `aria-label="..."` | Qualquer elemento | Rótulo acessível quando não há texto visível |
| `role="..."` | Elementos customizados | Define o papel do elemento para tecnologias assistivas |

#### 1.2 CSS — Referência rápida

**Seletores mais usados:**

| Seletor | Exemplo | O que seleciona |
|---|---|---|
| Tag | `h1 { }` | Todos os `<h1>` |
| Classe | `.kpi-card { }` | Todos os elementos com `class="kpi-card"` |
| ID | `#titulo { }` | O elemento com `id="titulo"` (único) |
| Descendente | `.kpis .kpi-card { }` | Cards dentro da seção de KPIs |

**Propriedades mais usadas para a dashboard:**

| Categoria | Propriedades | Exemplo |
|---|---|---|
| **Texto** | `font-size`, `font-weight`, `color`, `text-align` | `font-size: 2rem; color: #333;` |
| **Espaçamento** | `margin`, `padding`, `gap` | `padding: 16px; gap: 12px;` |
| **Borda** | `border`, `border-radius`, `border-left` | `border-left: 4px solid #4CAF50;` |
| **Fundo** | `background-color`, `background` | `background-color: #f9f9f9;` |
| **Layout** | `display`, `flex-direction`, `justify-content`, `align-items` | `display: flex; gap: 16px;` |
| **Tamanho** | `width`, `max-width`, `min-height` | `max-width: 1200px; width: 100%;` |
| **Sombra** | `box-shadow` | `box-shadow: 0 2px 8px rgba(0,0,0,0.1);` |

**Flexbox — guia visual:**

```
flex-direction: row (padrão)
┌────┐ ┌────┐ ┌────┐
│ 1  │ │ 2  │ │ 3  │
└────┘ └────┘ └────┘

flex-direction: column
┌────┐
│ 1  │
└────┘
┌────┐
│ 2  │
└────┘
┌────┐
│ 3  │
└────┘

justify-content: space-between (row)
┌────┐           ┌────┐           ┌────┐
│ 1  │           │ 2  │           │ 3  │
└────┘           └────┘           └────┘

flex-wrap: wrap (itens caem para a próxima linha)
┌────┐ ┌────┐ ┌────┐
│ 1  │ │ 2  │ │ 3  │
└────┘ └────┘ └────┘
┌────┐ ┌────┐
│ 4  │ │ 5  │
└────┘ └────┘
```

**Media queries — responsividade:**

```css
/* Estilos padrão: desktop */
.container {
    display: flex;
    gap: 16px;
}

/* Tablet */
@media (max-width: 1024px) {
    .container {
        flex-wrap: wrap;
    }
}

/* Celular */
@media (max-width: 768px) {
    .container {
        flex-direction: column;
    }
}
```

---

### Parte 2 — Tarefa: construir a estrutura HTML/CSS da dashboard (60 min)

Objetivo: implementar a estrutura HTML/CSS do wireframe criado no Módulo 6, usando o ciclo AI para cada seção.

---

#### Instruções

1. Abra o wireframe e os requisitos escritos do Módulo 6 (`05_dev_com_ai/modulo06_ux_prototipacao_ai/`)
2. Crie dois arquivos: `index.html` e `style.css`
3. Para **cada seção** do wireframe, siga o ciclo AI obrigatório (detalhado abaixo)
4. Ao final, você terá a estrutura completa da dashboard em HTML/CSS puro

#### Seções a implementar

Implemente as seções na ordem abaixo. Para cada uma, siga o ciclo completo.

| # | Seção | Correspondência no wireframe (Módulo 6) |
|---|---|---|
| 1 | Cabeçalho com título e filtros | Cabeçalho |
| 2 | Cards de KPI | KPIs |
| 3 | Área do gráfico principal | Gráfico principal |
| 4 | Áreas dos gráficos secundários | Gráficos secundários |
| 5 | Rodapé com fonte de dados | Fonte de dados |

---

### Parte 3 — Prática AI obrigatória: o ciclo para cada seção (incluso nos 60 min da Parte 2)

Objetivo: aplicar o ciclo **Requisito → Gerar → Aprender → Revisar** para cada seção da dashboard.

---

#### O ciclo detalhado

Para cada seção do wireframe, o aluno executa as 4 etapas:

**Etapa 1 — Escrever requisito**

Use o template de requisitos do Módulo 1 (`modulo01_primeiro_contato_ai/`) adaptado para HTML/CSS:

> **Contexto:** Estou construindo a dashboard de dados do meu projeto de integração em HTML e CSS puro. Já tenho a estrutura base com `header`, `main`, `section` e `footer`.
>
> **Objetivo:** [Descreva a seção que quer criar]
>
> **Detalhes:** [Layout, conteúdo, comportamento responsivo]
>
> **Restrições:** HTML semântico e CSS puro. Sem JavaScript, sem frameworks.
>
> **Formato:** HTML e CSS separados. Não explique ainda.

**Etapa 2 — Gerar com AI**

Envie o requisito, receba o código e **leia antes de executar**.

**Etapa 3 — Pedir explicação**

Questione as escolhas da AI. Use perguntas como as do Módulo 2 (`modulo02_revisao_com_ai/`), adaptadas para HTML/CSS:

| Habilidade | Perguntas sugeridas |
|---|---|
| **Aprender** | "Por que usou `flexbox` aqui em vez de outro layout?" |
| **Aprender** | "O que essa `media query` faz exatamente?" |
| **Aprender** | "Qual a diferença entre `margin` e `padding` neste caso?" |
| **Aprender** | "Por que usou `rem` em vez de `px`?" |

**Etapa 4 — Pedir revisão**

Solicite revisão de semântica, acessibilidade e responsividade:

| Habilidade | Perguntas sugeridas |
|---|---|
| **Revisar** | "Revise meu HTML quanto a semântica e acessibilidade." |
| **Revisar** | "O que um leitor de tela leria nesta seção?" |
| **Testar** | "O layout quebra no celular (375px)? O que está errado?" |
| **Testar** | "Essa seção funciona se eu mudar o conteúdo para textos mais longos?" |

---

#### Exemplos concretos do ciclo por seção

**Seção: Cards de KPI**

| Etapa | Habilidade | Exemplo |
|---|---|---|
| 1. Requisito | Escrever requisito | "Card com título, número grande e borda colorida à esquerda, responsivo. Três cards lado a lado no desktop, empilhados no celular." |
| 2. Gerar | Gerar com AI | Recebe HTML com `<article class="kpi-card">` + CSS com flexbox |
| 3. Aprender | Pedir explicação | "Por que usou `flexbox` aqui? O que `flex: 1 1 250px` significa?" |
| 4. Revisar | Pedir revisão | "Revise a semântica: `article` é a tag certa para um card de KPI?" |

**Seção: Gráfico principal**

| Etapa | Habilidade | Exemplo |
|---|---|---|
| 1. Requisito | Escrever requisito | "Seção com título h2 e área reservada para gráfico (placeholder retangular com fundo cinza claro e texto 'Gráfico será inserido aqui'). Largura 100% do container." |
| 2. Gerar | Gerar com AI | Recebe HTML com `<section>` + placeholder estilizado |
| 3. Aprender | Pedir explicação | "Por que usou `min-height` em vez de `height` para o placeholder?" |
| 4. Revisar | Pedir revisão | "O layout quebra no celular? O gráfico mantém proporção?" |

**Seção: Cabeçalho com filtros**

| Etapa | Habilidade | Exemplo |
|---|---|---|
| 1. Requisito | Escrever requisito | "Cabeçalho com título h1 à esquerda e 2–3 dropdowns de filtro à direita, alinhados na mesma linha. No celular, filtros ficam abaixo do título." |
| 2. Gerar | Gerar com AI | Recebe HTML com `<header>` + `<select>` + CSS com flexbox |
| 3. Aprender | Pedir explicação | "Por que usou `flex-wrap: wrap` no header?" |
| 4. Revisar | Pedir revisão | "Teste mentalmente no celular: título e filtros se reorganizam corretamente?" |

---

### Parte 4 — Leitura complementar: semântica e acessibilidade (30 min)

Objetivo: entender por que semântica e acessibilidade importam e como validar o HTML produzido.

---

#### 4.1 Por que semântica importa?

| Aspecto | Sem semântica | Com semântica |
|---|---|---|
| **Código** | `<div class="header">` | `<header>` |
| **Leitor de tela** | "Grupo genérico" | "Cabeçalho da página" |
| **SEO** | Motor de busca não entende a estrutura | Motor de busca identifica título, navegação, conteúdo |
| **Manutenção** | Precisa ler o CSS para entender | A tag já diz o propósito |

#### 4.2 Checklist de acessibilidade para a dashboard

- [ ] A página tem `lang="pt-BR"` no `<html>`
- [ ] Há uma hierarquia de títulos lógica (`h1` → `h2` → `h3`, sem pular níveis)
- [ ] Imagens têm `alt` descritivo
- [ ] Cores de texto têm contraste suficiente com o fundo (mínimo 4.5:1)
- [ ] A navegação por teclado funciona (Tab para avançar, Shift+Tab para voltar)
- [ ] Elementos interativos (filtros, botões) têm rótulos acessíveis
- [ ] A página é legível com zoom de 200%

#### 4.3 Como pedir revisão de acessibilidade à AI

> "Revise meu HTML completo quanto a acessibilidade. Verifique:
> 1. Há `lang` no `<html>`?
> 2. A hierarquia de títulos está correta?
> 3. Todas as imagens têm `alt`?
> 4. Os filtros têm `<label>` associado?
> 5. As cores de texto têm contraste suficiente?
> 6. O que um leitor de tela leria ao navegar pela página?"

---

## Resumo Geral

| # | Parte | Tipo | Duração |
|---|---|---|---|
| — | Aula ativa: HTML semântico, CSS essencial, prática AI | Presencial com instrutora | 1h |
| 1 | Guia visual HTML + CSS | Assíncrono — leitura | 30 min |
| 2 | Construir HTML/CSS da dashboard (com ciclo AI) | Assíncrono — prática | 60 min |
| 3 | Ciclo AI obrigatório por seção | Integrado à Parte 2 | — |
| 4 | Semântica e acessibilidade | Assíncrono — leitura | 30 min |

---

## Referências

| Recurso | Localização |
|---|---|
| Notebooks de Python (Aulas 01–05) | `01_python/` |
| Plano de aula de Estatística | `02_estatistica/Plano_de_aula.md` |
| Conteúdo de Visualização de Dados | `03_visualizacao/CONTEUDO.md` |
| Conteúdo de Banco de Dados | `04_banco_dados/CONTEUDO.md` |
| Módulo 1 — Primeiro Contato com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| Módulo 2 — Revisão com AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Módulo 6 — UX e Prototipação | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
