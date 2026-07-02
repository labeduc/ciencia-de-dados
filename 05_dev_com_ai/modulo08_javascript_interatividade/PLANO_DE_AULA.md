# Plano de Aula — JavaScript + Interatividade + Dados na Tela

**Módulo:** 8 — JavaScript + Interatividade + Dados na Tela
**Carga horária total:** 3h (1h aula ativa + até 2h conteúdo assíncrono)
**Modalidade:** Aula ativa presencial/online + estudo assíncrono individual
**Público-alvo:** Alunos do LabEduc que concluíram os módulos anteriores e já possuem a dashboard em HTML/CSS (Módulo 7)
**Pré-requisitos:**
- Python (`01_python/`): variáveis, tipos, controle de fluxo, listas, dicionários, funções — base de lógica transferível para JS
- Visualização (`03_visualizacao/`): dados e gráficos que serão renderizados na dashboard
- Banco de Dados (`04_banco_dados/`): dados estruturados que alimentam a interface
- Módulo 6 — UX (`modulo06_ux_prototipacao_ai/`): wireframe e requisitos da dashboard
- Módulo 7 — HTML/CSS (`modulo07_html_css_com_ai/`): estrutura HTML/CSS implementada
- Módulos de AI (`modulo01_*`, `modulo02_*`): template de requisitos, questionamento e revisão
**Instrutora responsável:** Larissa
**Modelo de aprendizagem:** Sala de aula invertida — a aula ativa introduz JavaScript, DOM e o ciclo AI aplicado a dados; o conteúdo assíncrono guia a implementação completa da interatividade.

---

> **Importante para os alunos:** Este módulo conecta os dados da trilha de ciência de dados com a interface que vocês construíram nos Módulos 6 e 7. Vocês já sabem lógica de programação em Python — agora vão aplicar os mesmos conceitos (variáveis, funções, loops, listas) em JavaScript para fazer a dashboard ganhar vida.

---

## 🎯 Aula Ativa (1h)

### Preparação (antes da aula)

O aluno deve ter concluído os seguintes materiais **antes** desta sessão:

| # | Material | Conteúdo relevante |
|---|---|---|
| 1 | Python (`01_python/`) | Variáveis, funções, listas, dicionários, `for`, `map()` — base transferível para JS |
| 2 | Visualização (`03_visualizacao/`) | Dados e gráficos que serão renderizados |
| 3 | Banco de Dados (`04_banco_dados/`) | Dados estruturados para a dashboard |
| 4 | Módulo 7 — HTML/CSS (`modulo07_*`) | Dashboard em HTML/CSS pronta |
| 5 | Módulos de AI (`modulo01_*`, `modulo02_*`) | Ciclo de trabalho com AI |

**O aluno deve trazer para a aula:**
- Arquivos `index.html` e `style.css` do Módulo 7
- Wireframe e requisitos do Módulo 6

### Objetivo Geral

Introduzir JavaScript essencial e manipulação do DOM, e praticar o carregamento e renderização de dados da trilha de ciência de dados na dashboard.

### Objetivos Específicos

Ao final da aula ativa, o aluno será capaz de:

- Declarar variáveis, criar funções e tratar eventos em JavaScript
- Fazer a correspondência entre conceitos de Python e JavaScript
- Selecionar e modificar elementos HTML via DOM
- Carregar dados em um array de objetos e renderizar como tabela HTML usando o ciclo AI

### Conteúdo

| Bloco | Duração | Tópicos |
|---|---|---|
| JS essencial | 15 min | Variáveis (`let`, `const`), funções, arrow functions, tipos, comparação Python → JS, eventos |
| DOM | 10 min | Árvore do DOM, `querySelector`, `textContent`, `innerHTML`, `createElement`, `classList` |
| Prática AI intensiva | 30 min | Carregar dados da trilha e renderizar tabela: ciclo Requisito → Gerar → Aprender → Revisar |
| Encerramento | 5 min | Compartilhamento de resultados; orientação para conteúdo assíncrono |

### Metodologia

- Exposição curta com comparação Python → JS (aluno já sabe lógica, foco na sintaxe)
- Demonstração de DOM com elementos da dashboard existente
- Prática AI intensiva: aluno usa o ciclo completo para gerar e entender código JS real
- Instrutora circula para apoio durante a prática

### Recursos

- Arquivos `index.html` e `style.css` do Módulo 7
- Editor de código: VS Code com Live Server ou editor online
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)
- Referência: `CONTEUDO.md` (nesta mesma pasta)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: contextualização — da estrutura estática à interatividade |
| 0:05 – 0:15 | 10 min | **Exposição:** JS essencial — tabela Python → JS, variáveis, funções, eventos. Foco: "vocês já sabem isso em Python" |
| 0:15 – 0:25 | 10 min | **Exposição + demonstração:** DOM — diagrama da árvore, `querySelector`, modificar texto e estilos, criar elementos |
| 0:25 – 0:35 | 10 min | **Prática AI (etapas 1–2):** aluno escreve requisito para gerar tabela HTML a partir de array de dados; recebe e lê o código |
| 0:35 – 0:45 | 10 min | **Prática AI (etapa 3):** aluno pede explicação — "diferença entre `forEach` e `map`", "como `Object.keys()` funciona" |
| 0:45 – 0:55 | 10 min | **Prática AI (etapa 4):** aluno insere bug na tabela e pede à AI para encontrar; pede 3 casos de teste |
| 0:55 – 1:00 | 5 min | Compartilhamento de 2–3 tabelas; encerramento e orientação para conteúdo assíncrono |

### Avaliação

O aluno sai da aula com:
- Arquivo `script.js` vinculado à dashboard do Módulo 7
- Uma tabela HTML gerada dinamicamente a partir de um array de dados
- Registro do ciclo AI: requisito enviado, código recebido, perguntas feitas, testes e depuração

---

## 📖 Conteúdo Assíncrono (até 2h)

**Arquivo de referência:** `CONTEUDO.md` (nesta mesma pasta)

### Objetivo Geral

Adicionar interatividade completa à dashboard do projeto de integração: KPIs dinâmicos, filtros, ordenação e validação de formulário.

### Objetivos Específicos

Ao final do conteúdo assíncrono, o aluno será capaz de:

- Utilizar a referência Python → JavaScript para consultas rápidas
- Entender o DOM como árvore e navegar/modificar elementos via JavaScript
- Popular KPIs dinamicamente a partir de dados
- Implementar filtros com dropdown e ordenação com botão
- Gerar validação de formulário com AI e verificar com casos de teste

### Conteúdo

| Parte | Título | Tipo | Duração estimada |
|---|---|---|---|
| 1 | JavaScript essencial para quem já viu Python | Leitura de referência | 20 min |
| 2 | DOM para iniciantes com diagrama visual | Leitura | 20 min |
| 3 | Adicionar interatividade à dashboard | Tarefa prática (com ciclo AI) | 40 min |
| 4 | Validação de formulário + testes com AI | Prática AI | 20 min |
| 5 | Tabela-resumo do ciclo AI | Referência | — |

---

### Detalhamento das Partes

#### Parte 1 — JavaScript essencial para quem já viu Python (20 min)

**Objetivo:** Consolidar a correspondência Python → JavaScript como referência de consulta.

**Tópicos:**
- Variáveis: `let` vs. `const` vs. `var` (e por que evitar `var`)
- Arrays e métodos essenciais: `push`, `pop`, `forEach`, `map`, `filter`, `reduce`, `find`, `sort` — cada um com equivalente Python
- Objetos: criação, acesso, iteração, desestruturação — comparação com dicionários Python
- Template literals: equivalente a f-strings do Python

**Resultado esperado:** O aluno tem uma tabela de referência Python → JS para consultar durante a implementação.

---

#### Parte 2 — DOM para iniciantes com diagrama visual (20 min)

**Objetivo:** Entender o DOM como ponte entre HTML e JavaScript.

**Tópicos:**
- DOM como árvore de nós (diagrama da dashboard)
- Fluxo: selecionar → ler/modificar → criar/remover
- Exemplo completo: atualizar KPI dinamicamente a partir de dados

**Resultado esperado:** O aluno sabe selecionar qualquer elemento da dashboard e modificar seu conteúdo ou estilo via JavaScript.

---

#### Parte 3 — Adicionar interatividade à dashboard (40 min)

**Objetivo:** Implementar 3 funcionalidades interativas usando o ciclo AI.

**Funcionalidades:**

| # | Funcionalidade | Ciclo AI | Conceitos JS |
|---|---|---|---|
| 1 | Carregar dados e popular KPIs | Requisito → Gerar → Aprender → Revisar | `reduce`, `Math.max`, `DOMContentLoaded` |
| 2 | Filtro por categoria com dropdown | Requisito → Gerar → Aprender → Revisar | `filter`, evento `change`, reconstrução de tabela |
| 3 | Botão para ordenar por valor | Requisito → Gerar → Aprender → Revisar | `sort` com arrow function, evento `click` |

**Resultado esperado:** Dashboard com KPIs dinâmicos, filtro funcional e ordenação por clique.

---

#### Parte 4 — Validação de formulário + testes com AI (20 min)

**Objetivo:** Praticar geração de código, solicitação de testes e depuração com AI.

**Dinâmica:**
1. Gerar função de validação com AI (nome não vazio, valor positivo)
2. Pedir 3 casos de teste à AI (válido, nome vazio, valor negativo)
3. Executar os testes manualmente e comparar com o esperado
4. Inserir bug de propósito e pedir à AI para encontrar

**Resultado esperado:** O aluno sabe pedir testes à AI e usa depuração assistida para encontrar bugs.

---

#### Parte 5 — Tabela-resumo do ciclo AI (referência)

| Etapa | Habilidade | Exemplo concreto |
|---|---|---|
| 1. Requisito | Escrever requisito | "Função que lê dados de vendas e gera tabela HTML" |
| 2. Gerar | Gerar com AI | Enviar requisito e receber JavaScript funcional |
| 3. Aprender | Pedir explicação | "Qual a diferença entre `forEach` e `map`?" |
| 4. Revisar | Depuração | "Inseri um bug, a AI encontra?" |
| 4. Revisar | Pedir testes | "Gere 3 testes para essa função de filtro" |

---

## Metodologia Geral

- Aula ativa com exposição comparativa Python → JS + prática AI intensiva
- Conteúdo assíncrono com leituras de referência + implementação guiada pelo ciclo AI
- Todos os dados e métricas usados são compatíveis com o que foi trabalhado nos módulos anteriores (Python, Estatística, Visualização, Banco de Dados)
- O ciclo Requisito → Gerar → Aprender → Revisar é aplicado a cada funcionalidade

## Recursos

- Arquivo `CONTEUDO.md` (nesta mesma pasta)
- Dashboard do Módulo 7: `index.html`, `style.css`
- Wireframe e requisitos do Módulo 6
- Materiais anteriores: `01_python/`, `02_estatistica/`, `03_visualizacao/`, `04_banco_dados/`
- Módulos de AI: `modulo01_*`, `modulo02_*`
- Editor de código: VS Code (com Live Server) ou editor online
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)

## Cronograma Sugerido (Assíncrono)

| Bloco | Duração | Atividade |
|---|---|---|
| 0:00 – 0:20 | 20 min | **Leitura (Parte 1):** JavaScript essencial — referência Python → JS |
| 0:20 – 0:40 | 20 min | **Leitura (Parte 2):** DOM para iniciantes — árvore, seleção, modificação |
| 0:40 – 0:55 | 15 min | **Tarefa (Parte 3, func. 1):** Carregar dados e popular KPIs — ciclo AI |
| 0:55 – 1:10 | 15 min | **Tarefa (Parte 3, func. 2):** Filtro por categoria com dropdown — ciclo AI |
| 1:10 – 1:20 | 10 min | **Tarefa (Parte 3, func. 3):** Botão de ordenação — ciclo AI |
| 1:20 – 1:40 | 20 min | **Prática AI (Parte 4):** Validação de formulário → 3 testes → depuração |
| 1:40 – 2:00 | 20 min | Revisão geral do código, ajustes finais e organização dos arquivos |

## Avaliação

O aluno conclui este módulo com:

- **Arquivo `script.js`** vinculado à dashboard com:
  - Dados carregados em array de objetos (simulando dados da trilha de ciência de dados)
  - KPIs populados dinamicamente (total, média, máximo)
  - Tabela HTML gerada a partir dos dados
  - Filtro por categoria funcionando via dropdown
  - Ordenação por valor via botão
- **Validação de formulário** com 3 casos de teste documentados
- **Registro do ciclo AI** para cada funcionalidade: requisito, código, perguntas e revisão

---

## Relação com Outros Módulos

| Componente | Descrição | Localização |
|---|---|---|
| Python | Lógica de programação transferível para JS | `01_python/` |
| Estatística | Métricas calculadas nos KPIs (média, total) | `02_estatistica/` |
| Visualização | Dados e gráficos renderizados na dashboard | `03_visualizacao/` |
| Banco de Dados | Dados estruturados que alimentam a interface | `04_banco_dados/` |
| AI — Módulo 1 | Template de requisitos | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| AI — Módulo 2 | Questionamento e depuração com AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Módulo 6 — UX | Wireframe e requisitos da dashboard | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
| Módulo 7 — HTML/CSS | Estrutura visual da dashboard | `05_dev_com_ai/modulo07_html_css_com_ai/` |
| **Este módulo** | Interatividade e dados na tela | `05_dev_com_ai/modulo08_javascript_interatividade/` |
