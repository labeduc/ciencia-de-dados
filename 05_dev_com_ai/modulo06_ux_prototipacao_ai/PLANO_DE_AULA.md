# Plano de Aula — UX e Design de Interfaces + AI para Prototipação

**Módulo:** 6 — UX e Design de Interfaces + AI para Prototipação
**Carga horária total:** 3h (1h aula ativa + até 2h conteúdo assíncrono)
**Modalidade:** Aula ativa presencial/online + estudo assíncrono individual
**Público-alvo:** Alunos do LabEduc que concluíram os módulos de Python, Estatística, Visualização e Banco de Dados
**Pré-requisitos:**
- Python (`01_python/`): variáveis, tipos, controle de fluxo, estruturas de dados, funções
- Estatística (`02_estatistica/`): medidas de tendência central, correlação, projeções
- Visualização (`03_visualizacao/`): tipos de gráficos, Pandas, Seaborn, Matplotlib, Plotly
- Banco de Dados (`04_banco_dados/`): SQL, modelagem relacional, consultas com JOIN
- Módulos de AI (`05_dev_com_ai/modulo01_*`, `modulo02_*`): interação com AI, template de requisitos, questionamento de respostas
**Instrutora responsável:** Larissa
**Modelo de aprendizagem:** Sala de aula invertida — a aula ativa é dedicada à prática; o conteúdo assíncrono aprofunda os conceitos e guia a construção do entregável.

---

> **Importante para os alunos:** Este módulo marca a transição de "analisar dados" para "projetar uma interface que mostra os dados para outras pessoas". Tudo o que você aprendeu nos módulos anteriores será integrado em uma dashboard. Antes de escrever qualquer código, você vai projetar a interface no papel.

---

## 🎯 Aula Ativa (1h)

### Preparação (antes da aula)

O aluno deve ter concluído os seguintes módulos **antes** desta sessão:

| # | Módulo | Conteúdo relevante para este módulo |
|---|---|---|
| 1 | Python (`01_python/`) | Lógica, funções e estruturas de dados que serão usados na implementação |
| 2 | Estatística (`02_estatistica/`) | Métricas para KPIs: médias, medianas, extremos, correlação |
| 3 | Visualização (`03_visualizacao/`) | Tipos de gráficos e quando usar cada um; Plotly para interatividade |
| 4 | Banco de Dados (`04_banco_dados/`) | Tabelas e consultas SQL que alimentam a dashboard |
| 5 | AI — Módulo 1 (`modulo01_*`) | Template de requisitos para interagir com a AI |
| 6 | AI — Módulo 2 (`modulo02_*`) | Como questionar a AI sobre decisões e alternativas |

### Objetivo Geral

Introduzir os princípios de UX Design, criar um wireframe rápido da dashboard do projeto de integração e usar o AI Assistant para obter sugestões de usabilidade.

### Objetivos Específicos

Ao final da aula ativa, o aluno será capaz de:

- Explicar o que é UX e por que pensar no usuário antes de codar evita retrabalho
- Aplicar os princípios de hierarquia visual, agrupamento lógico e simplicidade
- Criar um wireframe rápido usando papel, Paint ou ferramenta simplificada
- Descrever uma interface em texto e usar a AI para receber sugestões de melhoria

### Conteúdo

| Bloco | Tópicos |
|---|---|
| O que é UX | UX vs. UI; por que UX importa para dashboards de dados; princípios básicos |
| Exemplos bom vs. ruim | Comparação de dashboards: título, KPIs, gráficos, cores, filtros |
| Wireframe rápido | O que é wireframe; ferramentas (papel, Paint, Excalidraw, Figma); anatomia de uma dashboard |
| Prática em aula | Aluno desenha wireframe da dashboard com título, filtros, KPIs e gráficos |
| Prática AI | Aluno descreve a interface em texto → AI sugere estrutura e melhorias de usabilidade |

### Metodologia

- Exposição curta dos princípios de UX com exemplos visuais (máx. 15 min)
- Prática guiada: instrutora demonstra a criação de um wireframe simples
- Prática autônoma: aluno cria seu próprio wireframe
- Interação com AI: aluno descreve interface e avalia sugestões recebidas

### Recursos

- Papel e caneta (para wireframe manual)
- Paint, Draw.io ou Excalidraw (para wireframe digital)
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)
- Referência de tipos de gráficos: `03_visualizacao/CONTEUDO.md`, Aula 01

### Cronograma

| Horário | Duração | Atividade |
|---|---|---|
| 0:00 – 0:05 | 5 min | Abertura: contextualização — de análise de dados para design de interface |
| 0:05 – 0:15 | 10 min | **Exposição:** O que é UX; princípios de hierarquia visual, agrupamento e simplicidade; exemplos bom vs. ruim |
| 0:15 – 0:25 | 10 min | **Prática guiada:** instrutora demonstra a criação de um wireframe de dashboard (papel ou ferramenta digital) |
| 0:25 – 0:40 | 15 min | **Prática autônoma:** aluno desenha o wireframe da sua dashboard com título, filtros, KPIs e áreas de gráficos; anota o que cada seção mostra |
| 0:40 – 0:55 | 15 min | **Prática AI:** aluno descreve a interface em texto, envia à AI e recebe sugestões de usabilidade; avalia quais incorporar |
| 0:55 – 1:00 | 5 min | Compartilhamento de 2–3 wireframes; discussão rápida; orientação para o conteúdo assíncrono |

### Avaliação

O aluno sai da aula com um wireframe inicial da dashboard (papel ou digital) e uma primeira rodada de feedback da AI sobre usabilidade.

---

## 📖 Conteúdo Assíncrono (até 2h)

**Arquivo de referência:** `CONTEUDO.md` (nesta mesma pasta)

### Objetivo Geral

Aprofundar os conceitos de UX, refinar o wireframe da dashboard do projeto de integração e produzir os requisitos escritos para cada seção da interface.

### Objetivos Específicos

Ao final do conteúdo assíncrono, o aluno será capaz de:

- Identificar os 5 erros mais comuns em dashboards de dados e evitá-los
- Desenhar um wireframe completo com todas as seções obrigatórias
- Descrever cada seção em requisitos escritos claros e completos
- Usar a AI para obter críticas de usabilidade estruturadas
- Validar o protótipo com um checklist antes de começar a codificação

### Conteúdo

| Parte | Título | Tipo | Duração estimada |
|---|---|---|---|
| 1 | UX para iniciantes — exemplos bons vs. ruins | Leitura | 30 min |
| 2 | Wireframe do projeto de integração | Tarefa prática | 40 min |
| 3 | Descrever wireframe para AI e pedir críticas | Desafio AI | 30 min |
| 4 | Checklist de revisão do protótipo | Verificação | 20 min |

---

### Detalhamento das Partes

#### Parte 1 — UX para iniciantes (30 min)

**Objetivo:** Entender os fundamentos de UX com exemplos práticos aplicados a dashboards de dados.

**Tópicos:**
- O que torna uma interface "boa" — o usuário completa a tarefa sem pensar na interface
- Os 5 erros mais comuns: excesso de informação, gráfico errado, cores sem significado, falta de contexto, filtros escondidos
- Anatomia de uma dashboard bem estruturada: cabeçalho → KPIs → gráfico principal → gráficos secundários
- Referências cruzadas: tipos de gráficos (`03_visualizacao/`, Aula 01), paleta de cores (`03_visualizacao/`, Aula 10)

**Resultado esperado:** O aluno identifica boas e más práticas de UX e sabe aplicar os princípios ao wireframe.

---

#### Parte 2 — Wireframe do projeto de integração (40 min)

**Objetivo:** Criar o wireframe completo da dashboard com todas as seções obrigatórias e requisitos escritos.

**Seções obrigatórias:**

| Seção | Conteúdo | Referência |
|---|---|---|
| Cabeçalho | Título + filtros | Princípios de UX |
| KPIs | 2–3 indicadores numéricos | Estatística (`02_estatistica/`) |
| Gráfico principal | Visualização de destaque | Visualização (`03_visualizacao/`) |
| Gráficos secundários | 1–2 complementares | Visualização (`03_visualizacao/`) |
| Fonte de dados | Tabelas/consultas SQL | Banco de Dados (`04_banco_dados/`) |

**Resultado esperado:** Wireframe completo com requisitos escritos para cada seção.

---

#### Parte 3 — Desafio AI: críticas de usabilidade (30 min)

**Objetivo:** Usar a AI para validar o wireframe e identificar pontos de melhoria.

**Dinâmica:**
1. Descrever o wireframe seção por seção em texto
2. Enviar à AI com pedido estruturado de avaliação de usabilidade (template no `CONTEUDO.md`)
3. Avaliar sugestões: quais incorporar, quais descartar
4. Atualizar o wireframe com as melhorias escolhidas

**Resultado esperado:** O aluno tem um wireframe revisado pela AI com melhorias de usabilidade incorporadas.

---

#### Parte 4 — Checklist: revisão do protótipo (20 min)

**Objetivo:** Garantir que o wireframe está completo e validado antes da codificação.

**Categorias do checklist:**
- Layout e hierarquia (título, KPIs, gráfico principal, filtros, espaço vazio)
- Dados e gráficos (tipo adequado, rótulos, fontes de dados, métricas)
- Usabilidade (clareza, consistência de cores, sem redundância, revisão da AI)
- Requisitos escritos (completos, claros, independentes do wireframe)

**Resultado esperado:** Checklist preenchido, confirmando que o protótipo está pronto.

---

## Metodologia Geral

- Aula ativa com exposição curta + prática de wireframing + interação com AI
- Conteúdo assíncrono com leitura, tarefa prática, desafio AI e checklist de validação
- Integração explícita com todos os módulos anteriores do curso (Python, Estatística, Visualização, Banco de Dados, AI)
- O wireframe é o artefato central que conecta a análise de dados à implementação da interface

## Recursos

- Arquivo `CONTEUDO.md` (nesta mesma pasta)
- Materiais dos módulos anteriores: `01_python/`, `02_estatistica/`, `03_visualizacao/`, `04_banco_dados/`
- Módulos de AI anteriores: `modulo01_primeiro_contato_ai/`, `modulo02_revisao_com_ai/`
- Ferramentas de wireframe: papel, Paint, Draw.io, Excalidraw ou Figma
- AI Assistant (ChatGPT, Copilot, Gemini ou similar)

## Cronograma Sugerido (Assíncrono)

| Bloco | Duração | Atividade |
|---|---|---|
| 0:00 – 0:30 | 30 min | **Leitura (Parte 1):** UX para iniciantes — exemplos bons vs. ruins, anatomia de dashboard |
| 0:30 – 1:10 | 40 min | **Tarefa (Parte 2):** Criar wireframe completo com seções obrigatórias e escrever requisitos |
| 1:10 – 1:40 | 30 min | **Desafio AI (Parte 3):** Descrever wireframe à AI, receber críticas, incorporar melhorias |
| 1:40 – 2:00 | 20 min | **Checklist (Parte 4):** Revisar protótipo item a item antes de começar a codar |

## Avaliação

### 📦 Entregável

O aluno entrega ao final deste módulo:

1. **Wireframe da dashboard** — esboço visual com todas as seções obrigatórias (cabeçalho, KPIs, gráficos, filtros, fonte de dados)
2. **Requisitos escritos** — para cada seção, 1–2 frases descrevendo: o que mostra, que dado usa e por que o usuário precisa
3. **Registro da avaliação da AI** — sugestões de usabilidade recebidas e quais foram incorporadas
4. **Checklist preenchido** — todos os itens verificados antes de iniciar a codificação

---

## Relação com Outros Módulos

| Componente | Descrição | Localização |
|---|---|---|
| Python | Lógica e funções para implementação | `01_python/` |
| Estatística | Métricas para KPIs (médias, medianas, correlações) | `02_estatistica/` |
| Visualização | Tipos de gráficos e boas práticas visuais | `03_visualizacao/` |
| Banco de Dados | Consultas SQL que alimentam a dashboard | `04_banco_dados/` |
| AI — Módulo 1 | Template de requisitos para interagir com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| AI — Módulo 2 | Questionamento de respostas da AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
| **Este módulo** | UX, wireframe e requisitos da dashboard | `05_dev_com_ai/modulo06_ux_prototipacao_ai/` |
