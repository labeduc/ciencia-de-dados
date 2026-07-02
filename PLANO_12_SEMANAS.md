# Plano de Curso - 12 Semanas

## Distribuição das Aulas

| Categoria | Quantidade | Semanas |
|---|---|---|
| **Python** | 2 aulas | Semanas 1-2 |
| **Estatística** | 1 aula | Semana 3 |
| **Visualização** | 2 aulas | Semanas 4-5 |
| **Banco de Dados** | 2 aulas | Semanas 6-7 |
| **Dev com AI** | 4 aulas | Semanas 8-11 |
| **Projeto Final** | 1 aula | Semana 12 |
| **Total** | 12 aulas | 12 semanas |

---

## Semana 1 — Python: Fundamentos da Linguagem

**Categoria:** Python (Aula 1/2)

**Conteúdo:**
- Aulas 01-02 do módulo `01_python/`
  - Introdução ao Python (variáveis, strings, input/output)
  - Tipos básicos, operações e expressões
  - Exercícios: cálculo de ano de nascimento, fórmula de Bhaskara

**Objetivos:**
- Compreender o que é Python e como executar programas
- Dominar tipos de dados básicos e operadores
- Praticar entrada e saída de dados

**Pré-requisitos:** Noções de lógica de programação

**Materiais:**
- `01_python/Python_AULA01.ipynb`
- `01_python/Python_AULA02.ipynb`
- `01_python/CONTEUDO.md` (Módulo 1)

---

## Semana 2 — Python: Controle de Fluxo e Estruturas de Dados

**Categoria:** Python (Aula 2/2)

**Conteúdo:**
- Aulas 03-04 do módulo `01_python/`
  - Controle de fluxo (if/elif/else, while, break, continue)
  - Estruturas de dados (listas, tuplas, conjuntos, dicionários)
  - Exercícios: ordenação, classificação, conjectura de Collatz, tradutor

**Objetivos:**
- Dominar desvios condicionais e laços de repetição
- Trabalhar com coleções de dados (listas, dicionários)
- Aplicar conceitos em problemas práticos

**Pré-requisitos:** Semana 1 (Python Fundamentos)

**Materiais:**
- `01_python/Python_AULA03.ipynb`
- `01_python/Python_AULA04.ipynb`
- `01_python/CONTEUDO.md` (Módulos 2-3)

---

## Semana 3 — Estatística: Medidas de Tendência Central e Análise

**Categoria:** Estatística (Aula 1/1)

**Conteúdo:**
- Módulos 1-2 do `02_estatistica/`
  - Introdução, recolha e organização de dados
  - Medidas de tendência central (média, mediana, moda)
  - Frequências e análise de dados

**Objetivos:**
- Compreender conceitos fundamentais de estatística
- Calcular médias, medianas e modas
- Organizar dados em tabelas e calcular frequências

**Pré-requisitos:** Semana 1 (Python básico auxilia, mas não obrigatório)

**Materiais:**
- `02_estatistica/Plano_de_aula.md`
- Google Planilhas ou Excel para exercícios práticos

**Atividade Prática:**
- Análise de dados de voleibol (médias, extremos, modas)
- Importação de CSV para calcular médias de despesas

---

## Semana 4 — Visualização: Fundamentos e Pandas

**Categoria:** Visualização (Aula 1/2)

**Conteúdo:**
- Aulas 01-05 do módulo `03_visualizacao/`
  - Teoria de visualização de dados
  - Google Colab e formatos de dados
  - Pandas: carregamento, inspeção, filtragem e agregação

**Objetivos:**
- Entender o papel da visualização no fluxo de ciência de dados
- Dominar o Google Colab como ambiente de desenvolvimento
- Aprender a manipular dados com Pandas

**Pré-requisitos:** Semanas 1-2 (Python) e Semana 3 (Estatística)

**Materiais:**
- `03_visualizacao/aula-01/` a `03_visualizacao/aula-05/`
- `03_visualizacao/CONTEUDO.md` (Módulos 1-2)
- Dataset: `pokemons.csv`

**Atividade Prática:**
- Carregar e explorar dataset de Pokémons
- Filtrar dados por critérios
- Agregar e resumir dados com groupby()

---

## Semana 5 — Visualização: Gráficos com Seaborn e Matplotlib

**Categoria:** Visualização (Aula 2/2)

**Conteúdo:**
- Aulas 06-10 do módulo `03_visualizacao/`
  - Gráficos de barras (countplot, barplot)
  - Gráficos de linhas e áreas
  - Gráficos de dispersão e quadrantes
  - Gráfico de pizza
  - Melhorando visuais (design, cores, hierarquia)

**Objetivos:**
- Criar os principais tipos de gráficos estáticos
- Aplicar boas práticas de design em visualizações
- Escolher o tipo de gráfico adequado ao objetivo

**Pré-requisitos:** Semana 4 (Visualização Fundamentos e Pandas)

**Materiais:**
- `03_visualizacao/aula-06/` a `03_visualizacao/aula-10/`
- `03_visualizacao/pratica-aula-06/` e `03_visualizacao/pratica-aula-08/`
- `03_visualizacao/CONTEUDO.md` (Módulo 3)

**Atividade Prática:**
- Criar gráficos de barras por tipo de Pokémon
- Construir gráfico de dispersão com quadrantes
- Aplicar paleta de cores personalizada

---

## Semana 6 — Banco de Dados: Consultas SQL Básicas

**Categoria:** Banco de Dados (Aula 1/2)

**Conteúdo:**
- Aula 01 do módulo `04_banco_dados/`
  - Introdução a bancos de dados
  - Comando SELECT e suas cláusulas (WHERE, ORDER BY, GROUP BY, HAVING)
  - Operadores de comparação e lógicos
  - Funções de agregação

**Objetivos:**
- Compreender o papel dos bancos de dados relacionais
- Dominar consultas SQL básicas
- Filtrar, ordenar e agrupar dados

**Pré-requisitos:** Semana 3 (Estatística - conceitos de dados)

**Materiais:**
- `04_banco_dados/aulas/Aula01_Banco_Dados.ipynb`
- `04_banco_dados/aulas/Aula01_SQL_Island.ipynb`
- `04_banco_dados/CONTEUDO.md`
- Bancos de dados: `clientes.db`, `videogame_sales.db`

**Atividade Prática:**
- SQL Island: exercícios gamificados com SELECT e WHERE
- Consultar dataset de vendas de videogames

---

## Semana 7 — Banco de Dados: DDL, DML e Relacionamentos

**Categoria:** Banco de Dados (Aula 2/2)

**Conteúdo:**
- Aula 02 do módulo `04_banco_dados/`
  - Comandos INSERT, UPDATE, DELETE
  - DDL: CREATE TABLE, DROP TABLE
  - Restrições (constraints): PRIMARY KEY, FOREIGN KEY
  - JOIN entre tabelas relacionadas

**Objetivos:**
- Criar e manipular tabelas com SQL
- Entender integridade referencial e relacionamentos
- Modelar um banco de dados relacional completo

**Pré-requisitos:** Semana 6 (Banco de Dados Consultas Básicas)

**Materiais:**
- `04_banco_dados/aulas/Aula02_Banco_Dados.ipynb`
- `04_banco_dados/aulas/Aula02_Exercicio2.ipynb`
- `04_banco_dados/aulas/BDEmpregados.pdf`
- `04_banco_dados/CONTEUDO.md`

**Atividade Prática:**
- Modelar banco de dados de RH (BDEmpregados)
- Criar tabelas, inserir dados e fazer consultas com JOIN

---

## Semana 8 — Dev com AI: Primeiro Contato e Revisão

**Categoria:** Dev com AI (Aula 1/4)

**Conteúdo:**
- Módulo 1: Primeiro Contato com AI (assíncrono)
- Módulo 2: Revisão com AI (assíncrono)

**Objetivos:**
- Aprender a interagir produtivamente com AI Assistants
- Usar AI para depurar código e encontrar bugs
- Desenvolver senso crítico para avaliar respostas da AI

**Conteúdo Detalhado:**
- O que é um AI Assistant e como conversar com ele
- Template de requisitos (Contexto, Objetivo, Detalhes, Formato)
- 3 exercícios de Python para resolver manualmente e pedir explicação
- 3 programas com bugs para depurar com ajuda da AI
- Como questionar a AI sobre o código dela

**Pré-requisitos:** Semanas 1-2 (Python completo)

**Materiais:**
- `05_dev_com_ai/modulo01_primeiro_contato_ai/CONTEUDO.md`
- `05_dev_com_ai/modulo02_revisao_com_ai/CONTEUDO.md`

**Atividades:**
- Resolver exercícios de Python (par/ímpar, soma até 0, temperatura)
- Depurar 3 programas com bugs (calculadora, contador, tradutor)
- Gerar código com requisito detalhado e questionar escolhas da AI

---

## Semana 9 — Dev com AI: UX e Prototipação

**Categoria:** Dev com AI (Aula 2/4)

**Conteúdo:**
- Módulo 6: UX e Design de Interfaces + AI para Prototipação
  - Aula ativa (1h): UX, wireframe e prática AI
  - Conteúdo assíncrono: leitura, tarefa de wireframe, desafio AI

**Objetivos:**
- Compreender princípios de UX aplicados a dashboards
- Criar wireframe da dashboard do projeto de integração
- Usar AI para obter críticas de usabilidade

**Conteúdo Detalhado:**
- O que é UX: pensar no usuário antes de codar
- Princípios básicos: hierarquia visual, agrupamento, consistência
- Wireframe: esboço esquemático da interface
- Ferramentas: papel, Paint, Draw.io, Excalidraw, Figma
- Prática AI: descrever interface e receber sugestões

**Pré-requisitos:** Semanas 1-7 (todos os módulos anteriores: Python, Estatística, Visualização, Banco de Dados)

**Materiais:**
- `05_dev_com_ai/modulo06_ux_prototipacao_ai/CONTEUDO.md`

**Entregável:**
- Wireframe da dashboard com seções obrigatórias (cabeçalho, KPIs, gráficos, filtros, fonte de dados)
- Requisitos escritos para cada seção
- Registro da avaliação da AI
- Checklist preenchido

---

## Semana 10 — Dev com AI: HTML e CSS

**Categoria:** Dev com AI (Aula 3/4)

**Conteúdo:**
- Módulo 7: HTML e CSS com AI Assistants
  - Aula ativa (1h): HTML semântico, CSS essencial, prática AI
  - Conteúdo assíncrono: guia visual, tarefa de construção, ciclo AI

**Objetivos:**
- Dominar HTML semântico para estruturação de páginas
- Aplicar CSS essencial (box model, flexbox, responsividade)
- Implementar estrutura HTML/CSS da dashboard usando ciclo AI

**Conteúdo Detalhado:**
- HTML semântico: header, main, section, article, footer
- CSS: box model, flexbox, media queries
- O ciclo AI: Requisito → Gerar → Aprender → Revisar
- Prática em aula: Card de KPI
- Tarefa: construir estrutura completa da dashboard

**Pré-requisitos:** Semana 9 (UX e wireframe)

**Materiais:**
- `05_dev_com_ai/modulo07_html_css_com_ai/CONTEUDO.md`

**Entregável:**
- Arquivos `index.html` e `style.css` com estrutura da dashboard
- Aplicação do ciclo AI para cada seção (cabeçalho, KPIs, gráficos, rodapé)

---

## Semana 11 — Dev com AI: JavaScript e Integração

**Categoria:** Dev com AI (Aula 4/4)

**Conteúdo:**
- Módulo 8: JavaScript + Interatividade
- Módulo 9: Exibir e Organizar Dados no Frontend + Integração

**Objetivos:**
- Aprender JavaScript essencial (comparação Python → JS)
- Manipular o DOM para criar interatividade
- Criar gráficos interativos com Chart.js
- Integrar todas as peças do projeto

**Conteúdo Detalhado:**
- JavaScript: variáveis, funções, eventos, arrays, objetos
- DOM: selecionar e modificar elementos
- Prática AI: carregar dados e renderizar tabela
- Chart.js: gráficos de barras, linhas, pizza
- Integração completa: dados → KPIs → tabela → gráficos → filtros
- Ciclo AI autônomo: aluno decide o que construir

**Pré-requisitos:** Semana 10 (HTML/CSS)

**Materiais:**
- `05_dev_com_ai/modulo08_javascript_interatividade/CONTEUDO.md`
- `05_dev_com_ai/modulo09_dados_frontend_integracao/CONTEUDO.md`

**Entregável:**
- Arquivo `script.js` com interatividade completa
- Pelo menos 3 gráficos Chart.js funcionando
- Filtros que atualizam tabela e gráficos simultaneamente
- Autoavaliação do aprendizado vs. uso da AI

---

## Semana 12 — Projeto Final: Apresentação e Entrega

**Categoria:** Projeto Final (Aula 1/1)

**Conteúdo:**
- Módulo 10: Projeto Integrador — Visualização de Dados
  - Aula ativa (1h): mentoria, Diário de Campo, apresentação
  - Conteúdo assíncrono: finalização, documentação, preparação

**Objetivos:**
- Finalizar a dashboard com ajustes visuais e responsividade
- Documentar o processo de uso da AI (Diário de Campo)
- Apresentar o projeto para a turma

**Conteúdo Detalhado:**
- Revisão e correções finais com mentoria
- Diário de Campo: 3 melhores prompts, 1 erro da AI, 1 aprendizado
- Apresentação de 3–5 minutos (demo ao vivo ou slides)
- Critérios de avaliação: funcionalidade, integração, UX, uso crítico da AI

**Pré-requisitos:** Semanas 1-11 (todo o conteúdo do curso)

**Materiais:**
- `05_dev_com_ai/modulo10_projeto_integrador/CONTEUDO.md`

**Entregáveis Finais:**
1. **Dashboard funcional:** `index.html`, `style.css`, `script.js`
2. **Diário de Campo:** documento com reflexão sobre uso da AI
3. **Apresentação:** demo ao vivo ou slides (2–3)

---

## Fluxo de Aprendizagem

```
Semana 1-2: Python (base de programação)
    ↓
Semana 3: Estatística (base analítica)
    ↓
Semana 4-5: Visualização (comunicação de dados)
    ↓
Semana 6-7: Banco de Dados (persistência e consultas)
    ↓
Semana 8: Dev com AI - Primeiro Contato (ferramenta transversal)
    ↓
Semana 9: Dev com AI - UX (design pensando no usuário)
    ↓
Semana 10: Dev com AI - HTML/CSS (estrutura e estilo)
    ↓
Semana 11: Dev com AI - JavaScript + Integração (interatividade e gráficos)
    ↓
Semana 12: Projeto Final (consolidação e apresentação)
```

---

## Resumo de Entregáveis por Semana

| Semana | Categoria | Entregável Principal |
|---|---|---|
| 1 | Python | Exercícios resolvidos (Aulas 01-02) |
| 2 | Python | Exercícios resolvidos (Aulas 03-04) |
| 3 | Estatística | Planilhas com análises estatísticas |
| 4 | Visualização | Notebooks com análise Pandas do dataset |
| 5 | Visualização | Gráficos criados com Seaborn/Matplotlib |
| 6 | Banco de Dados | Consultas SQL resolvidas (SQL Island) |
| 7 | Banco de Dados | Banco de dados modelado e criado (BDEmpregados) |
| 8 | Dev com AI | Exercícios de depuração e questionamento da AI |
| 9 | Dev com AI | Wireframe da dashboard + requisitos escritos |
| 10 | Dev com AI | Estrutura HTML/CSS da dashboard |
| 11 | Dev com AI | Dashboard funcional com JavaScript + Chart.js |
| 12 | Projeto Final | Dashboard completa + Diário de Campo + Apresentação |

---

## Carga Horária Estimada

| Categoria | Aulas | Carga Horária Total (estimada) |
|---|---|---|
| Python | 2 | ~10h (5h aula + 5h exercícios) |
| Estatística | 1 | ~4h (2h aula + 2h práticas) |
| Visualização | 2 | ~12h (6h aula + 6h práticas) |
| Banco de Dados | 2 | ~8h (4h aula + 4h práticas) |
| Dev com AI | 4 | ~16h (4h aula ativa + 12h assíncrono) |
| Projeto Final | 1 | ~4h (1h aula + 3h finalização) |
| **Total** | **12** | **~54h** |

---

## Pré-requisitos por Semana

| Semana | Pré-requisitos |
|---|---|
| 1 | Noções de lógica de programação |
| 2 | Semana 1 (Python Fundamentos) |
| 3 | Semana 1 (Python básico auxilia, mas não obrigatório) |
| 4 | Semanas 1-2 (Python) e Semana 3 (Estatística) |
| 5 | Semana 4 (Visualização Fundamentos e Pandas) |
| 6 | Semana 3 (Estatística - conceitos de dados) |
| 7 | Semana 6 (Banco de Dados Consultas Básicas) |
| 8 | Semanas 1-2 (Python completo) |
| 9 | Semanas 1-7 (todos os módulos anteriores) |
| 10 | Semana 9 (UX e wireframe) |
| 11 | Semana 10 (HTML/CSS) |
| 12 | Semanas 1-11 (todo o conteúdo do curso) |

---

## Observações Importantes

1. **Progressão Cumulativa:** Cada semana constrói sobre as anteriores. É essencial não pular semanas.

2. **Módulos Assíncronos de AI:** As semanas 8-11 incluem conteúdo assíncrono que o aluno deve realizar fora da aula presencial.

3. **Projeto Integrador:** O projeto final (dashboard) é desenvolvido progressivamente das semanas 9-11, com entrega na semana 12.

4. **Uso de AI:** A partir da semana 8, o uso de AI Assistants é central. O aluno deve praticar o ciclo Requisito → Gerar → Aprender → Revisar consistentemente.

5. **Flexibilidade:** O instrutor pode ajustar o ritmo conforme a turma, mas a ordem lógica dos módulos deve ser mantida.

6. **Materiais Complementares:** Todos os materiais detalhados estão disponíveis nos arquivos `CONTEUDO.md` de cada módulo.
