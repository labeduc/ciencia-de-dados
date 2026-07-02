# Plano de Aula — Exibir e Organizar Dados no Frontend + Integração Completa com AI

**Módulo:** 9 — Exibir e Organizar Dados no Frontend + Integração Completa com AI
**Carga horária total:** 3h (1h aula ativa + até 2h conteúdo assíncrono)
**Modalidade:** Aula ativa presencial/online + estudo assíncrono individual
**Público-alvo:** Alunos do LabEduc que concluíram todos os módulos anteriores e já possuem a dashboard com HTML/CSS e JavaScript (Módulos 7 e 8)
**Pré-requisitos:**
- Python (`01_python/`): lógica, funções, listas, dicionários
- Estatística (`02_estatistica/`): médias, medianas, correlações, projeções
- Visualização (`03_visualizacao/`): tipos de gráficos, Pandas, Seaborn, Matplotlib, Plotly
- Banco de Dados (`04_banco_dados/`): SQL, modelagem, consultas
- Módulo 6 — UX (`modulo06_*`): wireframe e requisitos
- Módulo 7 — HTML/CSS (`modulo07_*`): estrutura e estilo da dashboard
- Módulo 8 — JavaScript (`modulo08_*`): DOM, eventos, dados, filtros, tabela
- Módulos de AI (`modulo01_*`, `modulo02_*`): ciclo Requisito → Gerar → Aprender → Revisar
**Instrutora responsável:** Larissa
**Modelo de aprendizagem:** Sala de aula invertida — a aula ativa introduz Chart.js e o ciclo AI autônomo; o conteúdo assíncrono guia a implementação completa e a reflexão final.

---

> **Importante para os alunos:** Este é o módulo final da trilha de front end. Vocês já dominam o ciclo AI — agora vão usá-lo de forma **autônoma**, sem instrução passo a passo. O objetivo é integrar tudo o que aprenderam (dados, estatística, visualização, banco de dados, UX, HTML/CSS, JavaScript) em uma dashboard funcional.

---

## 🎯 Aula Ativa (1h)

### Preparação (antes da aula)

O aluno deve ter concluído **todos** os módulos anteriores e ter os seguintes artefatos prontos:

| # | Artefato | Origem |
|---|---|---|
| 1 | Wireframe com requisitos por seção | Módulo 6 |
| 2 | `index.html` + `style.css` (dashboard estruturada) | Módulo 7 |
| 3 | `script.js` (dados, KPIs, tabela, filtros, ordenação) | Módulo 8 |
| 4 | Conhecimento do ciclo AI | Módulos 1 e 2 |

### Objetivo Geral

Introduzir Chart.js para criação de gráficos, mapear a integração completa do projeto e praticar o ciclo AI de forma autônoma.

### Objetivos Específicos

Ao final da aula ativa, o aluno será capaz de:

- Criar um gráfico interativo com Chart.js integrado à dashboard existente
- Mapear todas as peças do projeto e identificar o que falta para a integração completa
- Executar o ciclo AI de forma autônoma: definir feature → gerar → aprender → revisar → testar

### Conteúdo

| Bloco | Duração | Tópicos |
|---|---|---|
| Chart.js — gráficos a partir de dados | 20 min | O que é Chart.js; correspondência com Seaborn/Plotly; anatomia de um gráfico; exemplo de barras |
| Integração do projeto | 10 min | Mapa de integração; checklist de peças prontas; planejamento do que falta |
| Ciclo AI autônomo | 25 min | Aluno escolhe feature, executa ciclo completo sem instrução passo a passo |
| Encerramento | 5 min | Apresentação de features; orientação para conteúdo assíncrono |

### Metodologia

- Exposição curta de Chart.js com exemplo prático e correspondência com a trilha de visualização
- Mapa visual de integração: aluno vê como todas as peças se conectam
- Prática autônoma: aluno define feature, executa ciclo AI sozinho; instrutora observa e auxilia apenas se necessário
- Este bloco testa a **autonomia** do aluno com o ciclo AI

### Recursos

- Arquivos `index.html`, `style.css` e `script.js` dos módulos anteriores
- Chart.js via CDN: `https://cdn.jsdelivr.net/npm/chart.js`
- Editor de código: VS Code com Live Server ou editor online
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)
- Referência: `CONTEUDO.md` (nesta mesma pasta)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: visão geral da integração — todas as peças se conectam neste módulo |
| 0:05 – 0:20 | 15 min | **Exposição:** Chart.js — incluir via CDN, `<canvas>`, anatomia (`type`, `data`, `options`); exemplo de gráfico de barras ao vivo; tabela de correspondência Seaborn/Plotly → Chart.js |
| 0:20 – 0:30 | 10 min | **Integração:** mapa visual do projeto; checklist de peças prontas; cada aluno identifica o que falta na sua dashboard |
| 0:30 – 0:55 | 25 min | **Ciclo AI autônomo:** aluno escolhe feature (gráfico, filtro interativo, KPI com variação, etc.), executa o ciclo completo sozinho. Instrutora observa e auxilia só se necessário |
| 0:55 – 1:00 | 5 min | 2–3 alunos apresentam a feature construída; encerramento e orientação para conteúdo assíncrono |

### Avaliação

O aluno sai da aula com:
- Chart.js integrado à dashboard (pelo menos 1 gráfico funcionando)
- Checklist de integração preenchido (peças prontas vs. pendentes)
- Registro do ciclo AI autônomo: feature escolhida, requisito, código, perguntas, revisão e testes

---

## 📖 Conteúdo Assíncrono (até 2h)

**Arquivo de referência:** `CONTEUDO.md` (nesta mesma pasta)

### Objetivo Geral

Implementar todos os gráficos pertinentes à análise de dados na dashboard, adicionar refinamentos de UX e realizar autoavaliação do aprendizado.

### Objetivos Específicos

Ao final do conteúdo assíncrono, o aluno será capaz de:

- Criar gráficos de barras, linhas e pizza/rosca com Chart.js
- Preparar dados (map, reduce) para alimentar os gráficos
- Conectar filtros interativos à atualização de gráficos
- Implementar estados de loading e tratamento de erros
- Avaliar honestamente o que sabe fazer sozinho vs. o que depende da AI

### Conteúdo

| Parte | Título | Tipo | Duração estimada |
|---|---|---|---|
| 1 | Chart.js essencial: barras, linhas, pizza | Leitura de referência | 30 min |
| 2 | Implementar gráficos pertinentes à trilha | Tarefa prática (ciclo AI autônomo) | 40 min |
| 3 | Refinamentos: filtros, loading, erros | Prática com AI | 30 min |
| 4 | Autoavaliação | Reflexão individual | 20 min |

---

### Detalhamento das Partes

#### Parte 1 — Chart.js essencial (30 min)

**Objetivo:** Dominar a criação de 3 tipos de gráfico com Chart.js, com referência cruzada à trilha de visualização.

**Tópicos:**
- Gráfico de barras: básico, horizontal, agrupado, empilhado (↔ Seaborn Aula 06, Plotly Aula 15)
- Gráfico de linhas: série única, múltiplas séries, área preenchida (↔ Seaborn Aula 07, Plotly Aula 15)
- Gráfico de pizza/rosca: distribuição por categoria (↔ Matplotlib Aula 09, Plotly Aula 15)
- Preparar dados para Chart.js: `map` para extrair labels/valores, `reduce` para agrupar (↔ `groupby` do Pandas)

**Resultado esperado:** O aluno sabe criar os 3 tipos de gráfico e converter dados da trilha para o formato Chart.js.

---

#### Parte 2 — Implementar gráficos pertinentes à trilha (40 min)

**Objetivo:** Implementar na dashboard pelo menos 3 gráficos relevantes para a análise de dados.

**O aluno:**
1. Revisa quais gráficos criou na trilha de visualização (`03_visualizacao/`)
2. Decide quais são pertinentes para a dashboard
3. Implementa cada um usando o ciclo AI de forma autônoma
4. Conecta com os dados e filtros existentes (Módulo 8)

**Resultado esperado:** Dashboard com pelo menos 3 gráficos Chart.js integrados, cada um correspondendo a um tipo de análise da trilha de ciência de dados.

---

#### Parte 3 — Refinamentos com AI (30 min)

**Objetivo:** Polir a dashboard com filtros interativos que atualizam gráficos, estados de loading e tratamento de erros.

**Tópicos:**
- Atualizar gráficos quando filtro muda (`chart.destroy()` + recriar ou `chart.update()`)
- Estado de loading visual durante processamento
- Tratamento de dados vazios ou inválidos (mensagem "Nenhum dado encontrado")

**Resultado esperado:** Dashboard robusta que responde a interações do usuário e trata casos excepcionais.

---

#### Parte 4 — Autoavaliação (20 min)

**Objetivo:** Reflexão honesta sobre o aprendizado ao longo de toda a trilha.

**Tópicos:**
- Questionário por habilidade: "Consigo fazer sozinho" / "Preciso da AI" / "Não sei fazer"
  - Categorias: HTML/CSS, JavaScript, Chart.js, Uso da AI
- Reflexão escrita: parte mais difícil, quando a AI foi melhor, quando o aluno foi melhor
- Plano de estudo pós-curso: 3 habilidades para praticar, 1 projeto pessoal, 1 recurso por habilidade

**Resultado esperado:** O aluno sabe exatamente onde está forte e onde precisa praticar mais, e tem um plano concreto de continuidade.

---

## Metodologia Geral

- Aula ativa com exposição curta de Chart.js + prática AI **autônoma** (sem instrução passo a passo)
- Conteúdo assíncrono com referência, implementação guiada pelo ciclo AI, refinamentos e autoavaliação
- Integração explícita de todos os módulos anteriores do curso
- Este é o módulo que valida a autonomia do aluno no ciclo AI

## Recursos

- Arquivo `CONTEUDO.md` (nesta mesma pasta)
- Dashboard dos módulos anteriores: `index.html`, `style.css`, `script.js`
- Chart.js via CDN
- Materiais de toda a trilha: `01_python/`, `02_estatistica/`, `03_visualizacao/`, `04_banco_dados/`
- Módulos de AI: `modulo01_*`, `modulo02_*`
- Módulos de front end: `modulo06_*`, `modulo07_*`, `modulo08_*`
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)

## Cronograma Sugerido (Assíncrono)

| Bloco | Duração | Atividade |
|---|---|---|
| 0:00 – 0:30 | 30 min | **Leitura (Parte 1):** Chart.js essencial — barras, linhas, pizza, preparação de dados |
| 0:30 – 0:50 | 20 min | **Tarefa (Parte 2):** Implementar gráfico 1 e 2 — ciclo AI autônomo |
| 0:50 – 1:10 | 20 min | **Tarefa (Parte 2):** Implementar gráfico 3 + integração com filtros |
| 1:10 – 1:40 | 30 min | **Refinamentos (Parte 3):** Filtros interativos, loading, tratamento de erros — com AI |
| 1:40 – 2:00 | 20 min | **Autoavaliação (Parte 4):** Questionário, reflexão escrita e plano de estudo |

## Avaliação

O aluno conclui este módulo (e a trilha de front end) com:

- **Dashboard completa e funcional:**
  - Estrutura HTML semântica e CSS responsivo (Módulo 7)
  - Dados carregados, KPIs dinâmicos, tabela com filtro e ordenação (Módulo 8)
  - Pelo menos 3 gráficos Chart.js integrados e correspondentes à trilha de visualização
  - Filtros que atualizam tabela e gráficos simultaneamente
  - Tratamento de loading e dados vazios
- **Registro do ciclo AI autônomo** para cada feature implementada
- **Autoavaliação preenchida** com reflexão e plano de estudo pós-curso

---

## Relação com Outros Módulos

| Componente | Descrição | Localização |
|---|---|---|
| Python | Lógica de programação, base de tudo | `01_python/` |
| Estatística | Métricas nos KPIs e análises | `02_estatistica/` |
| Visualização | Tipos de gráficos reproduzidos com Chart.js | `03_visualizacao/` |
| Banco de Dados | Dados que alimentam a dashboard | `04_banco_dados/` |
| AI — Módulo 1 | Template de requisitos | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| AI — Módulo 2 | Questionamento e depuração | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Módulo 6 — UX | Wireframe e requisitos | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
| Módulo 7 — HTML/CSS | Estrutura visual | `05_dev_com_ai/modulo07_html_css_com_ai/` |
| Módulo 8 — JavaScript | Interatividade e dados | `05_dev_com_ai/modulo08_javascript_interatividade/` |
| **Este módulo** | Gráficos, integração completa e autonomia AI | `05_dev_com_ai/modulo09_dados_frontend_integracao/` |
