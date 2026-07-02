# Plano de Aula — HTML e CSS com AI Assistants

**Módulo:** 7 — HTML e CSS com AI Assistants
**Carga horária total:** 3h (1h aula ativa + até 2h conteúdo assíncrono)
**Modalidade:** Aula ativa presencial/online + estudo assíncrono individual
**Público-alvo:** Alunos do LabEduc que concluíram os módulos anteriores e o wireframe da dashboard (Módulo 6)
**Pré-requisitos:**
- Python (`01_python/`): lógica e funções (base de programação)
- Visualização (`03_visualizacao/`): tipos de gráficos e boas práticas visuais
- Módulo 6 — UX (`modulo06_ux_prototipacao_ai/`): wireframe da dashboard e requisitos escritos por seção
- Módulos de AI (`modulo01_*`, `modulo02_*`): template de requisitos, questionamento de respostas
**Instrutora responsável:** Larissa
**Modelo de aprendizagem:** Sala de aula invertida — a aula ativa introduz HTML, CSS e o ciclo AI; o conteúdo assíncrono guia a construção completa da dashboard.

---

> **Importante para os alunos:** Este módulo transforma o wireframe do Módulo 6 em código real. Para cada seção da dashboard, você vai seguir um ciclo obrigatório com a AI: **Requisito → Gerar → Aprender → Revisar**. O objetivo não é apenas ter o código pronto, mas entender cada decisão.

---

## 🎯 Aula Ativa (1h)

### Preparação (antes da aula)

O aluno deve ter concluído os seguintes materiais **antes** desta sessão:

| # | Material | Conteúdo relevante |
|---|---|---|
| 1 | Python (`01_python/`) | Base de lógica de programação |
| 2 | Visualização (`03_visualizacao/`) | Tipos de gráficos que serão exibidos na dashboard |
| 3 | Módulo 6 — UX (`modulo06_*`) | Wireframe da dashboard com requisitos escritos por seção |
| 4 | Módulo 1 — AI (`modulo01_*`) | Template de requisitos para interagir com AI |
| 5 | Módulo 2 — AI (`modulo02_*`) | Como questionar a AI sobre decisões e pedir revisão |

**O aluno deve trazer para a aula:**
- Wireframe da dashboard (papel ou digital)
- Requisitos escritos para cada seção do wireframe
- Checklist preenchido do Módulo 6

### Objetivo Geral

Introduzir HTML semântico e CSS essencial, e praticar o ciclo de trabalho com AI (Requisito → Gerar → Aprender → Revisar) na construção de um componente real da dashboard.

### Objetivos Específicos

Ao final da aula ativa, o aluno será capaz de:

- Criar a estrutura básica de uma página HTML com tags semânticas
- Estilizar elementos com CSS: box model, flexbox e media queries
- Aplicar o ciclo de trabalho com AI para gerar, entender e revisar código HTML/CSS
- Produzir um card de KPI funcional e responsivo usando o ciclo AI

### Conteúdo

| Bloco | Duração | Tópicos |
|---|---|---|
| HTML semântico | 15 min | Tags essenciais (`header`, `main`, `section`, `article`, `footer`); HTML semântico vs. `div` genérico; estrutura da dashboard |
| CSS essencial | 15 min | Box model (margin, border, padding); Flexbox (display, direction, justify, align, gap, wrap); Responsividade (`@media`, unidades relativas) |
| Prática AI intensiva | 25 min | Ciclo completo: requisito de card de KPI → gerar com AI → pedir explicação → revisar acessibilidade |
| Encerramento | 5 min | Compartilhamento de cards; orientação para conteúdo assíncrono |

### Metodologia

- Exposição curta de HTML e CSS com exemplos aplicados à dashboard (máx. 30 min)
- Prática AI intensiva: aluno aplica o ciclo completo em um componente real
- A cada etapa do ciclo, a instrutora circula para apoio e verificação

### Recursos

- Editor de código: VS Code ou editor online (CodePen, JSFiddle)
- Wireframe do Módulo 6 (cada aluno traz o seu)
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)
- Referência: `CONTEUDO.md` (nesta mesma pasta)

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: contextualização — do wireframe ao código |
| 0:05 – 0:15 | 10 min | **Exposição:** HTML semântico — tags essenciais, estrutura da dashboard, exemplo de página base |
| 0:15 – 0:25 | 10 min | **Exposição:** CSS essencial — box model (diagrama visual), flexbox (propriedades-chave), responsividade com `@media` |
| 0:25 – 0:30 | 5 min | **Demonstração:** instrutora mostra o ciclo AI com um componente simples |
| 0:30 – 0:40 | 10 min | **Prática AI (etapas 1–2):** aluno escreve requisito do card de KPI e envia à AI; recebe e lê o código gerado |
| 0:40 – 0:48 | 8 min | **Prática AI (etapa 3):** aluno pede explicação — "Por que usou flexbox?", "O que `flex: 1 1 250px` faz?" |
| 0:48 – 0:55 | 7 min | **Prática AI (etapa 4):** aluno pede revisão — semântica, acessibilidade, comportamento no celular |
| 0:55 – 1:00 | 5 min | Compartilhamento de 2–3 cards; encerramento e orientação para conteúdo assíncrono |

### Avaliação

O aluno sai da aula com:
- Um card de KPI funcional e responsivo, gerado com apoio da AI
- Registro das 4 etapas do ciclo (requisito enviado, código recebido, perguntas feitas, revisão obtida)

---

## 📖 Conteúdo Assíncrono (até 2h)

**Arquivo de referência:** `CONTEUDO.md` (nesta mesma pasta)

### Objetivo Geral

Construir a estrutura HTML/CSS completa da dashboard do projeto de integração, aplicando o ciclo AI obrigatório para cada seção do wireframe.

### Objetivos Específicos

Ao final do conteúdo assíncrono, o aluno será capaz de:

- Utilizar a referência rápida de HTML e CSS para consultas durante a implementação
- Construir a estrutura completa da dashboard com tags semânticas e layout responsivo
- Aplicar o ciclo AI (Requisito → Gerar → Aprender → Revisar) para cada seção
- Validar o HTML produzido quanto a semântica e acessibilidade

### Conteúdo

| Parte | Título | Tipo | Duração estimada |
|---|---|---|---|
| 1 | Guia visual HTML + CSS | Leitura de referência | 30 min |
| 2 | Construir HTML/CSS da dashboard (com ciclo AI) | Tarefa prática | 60 min |
| 3 | Ciclo AI obrigatório por seção | Integrado à Parte 2 | — |
| 4 | Semântica e acessibilidade | Leitura complementar | 30 min |

---

### Detalhamento das Partes

#### Parte 1 — Guia visual HTML + CSS (30 min)

**Objetivo:** Consolidar os conceitos de HTML e CSS como referência para a prática.

**Tópicos:**
- Estrutura mínima de uma página HTML
- Tags semânticas: quando usar cada uma (tabela comparativa `div` vs. tag semântica)
- Atributos de acessibilidade: `lang`, `alt`, `aria-label`, `role`
- Seletores CSS: tag, classe, ID, descendente
- Propriedades CSS mais usadas: texto, espaçamento, borda, fundo, layout, tamanho, sombra
- Flexbox: guia visual com diagramas ASCII (row, column, space-between, wrap)
- Media queries: breakpoints para desktop, tablet e celular

**Resultado esperado:** O aluno tem uma referência prática para consultar durante a implementação.

---

#### Parte 2 — Construir HTML/CSS da dashboard (60 min)

**Objetivo:** Implementar as 5 seções do wireframe em HTML/CSS, uma por uma, usando o ciclo AI.

**Seções:**

| # | Seção | Ciclo AI |
|---|---|---|
| 1 | Cabeçalho com título e filtros | Requisito → Gerar → Aprender → Revisar |
| 2 | Cards de KPI (2–3 indicadores) | Requisito → Gerar → Aprender → Revisar |
| 3 | Área do gráfico principal | Requisito → Gerar → Aprender → Revisar |
| 4 | Áreas dos gráficos secundários | Requisito → Gerar → Aprender → Revisar |
| 5 | Rodapé com fonte de dados | Requisito → Gerar → Aprender → Revisar |

**Para cada seção, o aluno:**
1. Escreve requisito usando o template (Contexto, Objetivo, Detalhes, Restrições, Formato)
2. Envia à AI e recebe HTML + CSS
3. Questiona escolhas ("Por que usou X?", "O que Y faz?")
4. Pede revisão de semântica, acessibilidade e responsividade

**Resultado esperado:** Dashboard completa em HTML/CSS com 5 seções implementadas e validadas.

---

#### Parte 3 — Ciclo AI obrigatório (integrado à Parte 2)

**Tabela-resumo do ciclo por habilidade:**

| Etapa | Habilidade | Exemplo concreto |
|---|---|---|
| 1. Requisito | Escrever requisito | "Card com título, número grande e borda colorida, responsivo" |
| 2. Gerar | Gerar com AI | Enviar requisito e receber código HTML + CSS |
| 3. Aprender | Pedir explicação | "Por que usou flexbox aqui?" |
| 4. Revisar | Pedir revisão | "O layout quebra no celular, o que está errado?" |
| 4. Revisar | Testar acessibilidade | "Revise meu HTML quanto a semântica e acessibilidade" |

---

#### Parte 4 — Semântica e acessibilidade (30 min)

**Objetivo:** Entender a importância de HTML semântico e acessibilidade, e validar a dashboard produzida.

**Tópicos:**
- Por que semântica importa (leitor de tela, SEO, manutenção)
- Checklist de acessibilidade para a dashboard (7 itens)
- Como pedir revisão de acessibilidade à AI (template de pedido)

**Resultado esperado:** O aluno validou sua dashboard com o checklist de acessibilidade e corrigiu os pontos necessários.

---

## Metodologia Geral

- Aula ativa com exposição curta + prática AI intensiva (ciclo completo em 1 componente)
- Conteúdo assíncrono com referência de consulta + implementação guiada pelo ciclo AI
- O ciclo Requisito → Gerar → Aprender → Revisar é **obrigatório** para cada seção
- Integração com wireframe e requisitos do Módulo 6

## Recursos

- Arquivo `CONTEUDO.md` (nesta mesma pasta)
- Wireframe e requisitos do Módulo 6: `05_dev_com_ai/modulo06_ux_prototipacao_ai/`
- Módulos de AI: `modulo01_primeiro_contato_ai/`, `modulo02_revisao_com_ai/`
- Editor de código: VS Code ou editor online
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)

## Cronograma Sugerido (Assíncrono)

| Bloco | Duração | Atividade |
|---|---|---|
| 0:00 – 0:30 | 30 min | **Leitura (Parte 1):** Guia visual HTML + CSS — tags, seletores, flexbox, media queries |
| 0:30 – 0:45 | 15 min | **Tarefa (Parte 2, seção 1):** Cabeçalho — ciclo AI completo |
| 0:45 – 1:00 | 15 min | **Tarefa (Parte 2, seção 2):** Cards de KPI — ciclo AI completo |
| 1:00 – 1:10 | 10 min | **Tarefa (Parte 2, seção 3):** Gráfico principal — ciclo AI completo |
| 1:10 – 1:20 | 10 min | **Tarefa (Parte 2, seção 4):** Gráficos secundários — ciclo AI completo |
| 1:20 – 1:30 | 10 min | **Tarefa (Parte 2, seção 5):** Rodapé — ciclo AI completo |
| 1:30 – 2:00 | 30 min | **Leitura (Parte 4):** Semântica e acessibilidade — checklist + revisão final com AI |

## Avaliação

O aluno conclui este módulo com:

- **Dashboard em HTML/CSS** — arquivo `index.html` + `style.css` com as 5 seções obrigatórias (cabeçalho, KPIs, gráfico principal, gráficos secundários, rodapé)
- **Layout responsivo** — a dashboard se adapta a desktop e celular
- **HTML semântico** — uso correto de `header`, `main`, `section`, `article`, `footer`
- **Registro do ciclo AI** — para cada seção: requisito enviado, código gerado, perguntas feitas e revisão obtida
- **Checklist de acessibilidade** — preenchido e com correções aplicadas

---

## Relação com Outros Módulos

| Componente | Descrição | Localização |
|---|---|---|
| Python | Base de lógica de programação | `01_python/` |
| Estatística | Métricas para KPIs | `02_estatistica/` |
| Visualização | Tipos de gráficos exibidos na dashboard | `03_visualizacao/` |
| Banco de Dados | Consultas SQL que alimentam os dados | `04_banco_dados/` |
| AI — Módulo 1 | Template de requisitos | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| AI — Módulo 2 | Questionamento de respostas da AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| Módulo 6 — UX | Wireframe e requisitos da dashboard | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
| **Este módulo** | Implementação HTML/CSS da dashboard | `05_dev_com_ai/modulo07_html_css_com_ai/` |
