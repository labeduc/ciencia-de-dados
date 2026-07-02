# UX e Design de Interfaces + AI para Prototipação

## Sobre o Conteúdo

Módulo que combina aula ativa (1h) e conteúdo assíncrono (até 2h), cobrindo os fundamentos de UX Design aplicados ao projeto de integração do curso de Ciência de Dados. O aluno aprende a pensar no usuário antes de codar, cria wireframes da dashboard que consumirá os dados trabalhados nos módulos anteriores (Python, Estatística, Visualização e Banco de Dados) e usa o AI Assistant para obter críticas de usabilidade.

**Formato:** Leitura em Markdown (`.md`) + prática de wireframing
**Carga horária total:** 3h (1h aula ativa + até 2h assíncrono)
**Pré-requisitos:**
- Conceitos de Python (`01_python/`): variáveis, tipos, controle de fluxo, estruturas de dados, funções
- Estatística (`02_estatistica/`): medidas de tendência central, correlação, projeções
- Visualização (`03_visualizacao/`): tipos de gráficos, Pandas, Seaborn, Matplotlib, Plotly
- Banco de Dados (`04_banco_dados/`): SQL, modelagem relacional, consultas com JOIN
- Módulos de AI anteriores (`05_dev_com_ai/modulo01_primeiro_contato_ai/`, `modulo02_revisao_com_ai/`): como interagir com AI e questionar respostas
**Instrutora responsável:** Larissa

---

## 🎯 Aula Ativa (1h)

### O que é UX: pensar no usuário antes de codar

#### O que é UX Design?

UX (User Experience) é a disciplina que cuida da **experiência do usuário** ao interagir com um produto — neste caso, uma dashboard de dados. Não se trata de deixar bonito; trata-se de deixar **útil, compreensível e eficiente**.

**Por que UX importa para Ciência de Dados?**

- Você pode ter o melhor modelo estatístico e os gráficos mais precisos, mas se o usuário não conseguir encontrar a informação ou não entender o que está vendo, o trabalho foi desperdiçado
- Uma dashboard mal organizada gera interpretações erradas — o layout influencia diretamente as decisões tomadas a partir dos dados
- Pensar no usuário antes de codar evita retrabalho: é mais fácil mover um quadrado no papel do que refatorar um front end inteiro

#### Princípios básicos de UX para dashboards

1. **Hierarquia visual:** as informações mais importantes devem aparecer primeiro e com maior destaque
2. **Agrupamento lógico:** dados relacionados ficam juntos (ex.: filtros em uma área, KPIs em outra, gráficos detalhados abaixo)
3. **Consistência:** mesmos padrões de cores, fontes e espaçamento em toda a interface
4. **Feedback:** o usuário deve saber o que aconteceu quando interage (ex.: filtro aplicado, dado carregando)
5. **Simplicidade:** menos é mais — cada elemento na tela deve ter um propósito claro

#### Exemplos rápidos: bom vs. ruim

| Aspecto | ❌ Ruim | ✅ Bom |
|---|---|---|
| **Título** | Sem título ou "Dashboard1" | "Análise de Vendas — Q4 2024" |
| **KPIs** | Números soltos sem contexto | Cartão com rótulo, valor e variação (↑ 12%) |
| **Gráficos** | 8 gráficos na mesma tela sem hierarquia | 2–3 gráficos principais com filtro para ver detalhes |
| **Cores** | Arco-íris sem significado | Paleta consistente: uma cor de destaque, restante neutro |
| **Filtros** | Escondidos ou inexistentes | Barra lateral ou topo com filtros visíveis |

---

### Wireframe rápido: papel, Paint ou aplicação simplificada

#### O que é um wireframe?

Um wireframe é um **esboço esquemático** da interface — sem cores, sem imagens reais, sem código. Ele mostra:

- **Onde** cada elemento fica na tela (layout)
- **O que** cada área da interface contém (conteúdo)
- **Como** o usuário navega ou interage (fluxo)

#### Ferramentas sugeridas (do mais simples ao mais elaborado)

| Ferramenta | Vantagem | Quando usar |
|---|---|---|
| **Papel e caneta** | Zero fricção, rápido para brainstorm | Primeiras ideias, rascunho individual |
| **Paint / Draw.io** | Gratuito, sem cadastro, fácil de compartilhar | Wireframe digital rápido |
| **Excalidraw** | Visual de "rascunho à mão", colaborativo | Wireframe digital com estilo informal |
| **Figma (gratuito)** | Profissional, componentes reutilizáveis | Protótipo mais detalhado |

#### Atividade em aula: wireframe da dashboard

**Contexto do projeto de integração:** Ao longo do curso, o aluno trabalhou com:
- **Python** (`01_python/`): lógica, funções e estruturas de dados
- **Estatística** (`02_estatistica/`): médias, medianas, correlações e projeções
- **Visualização** (`03_visualizacao/`): gráficos de barras, linhas, dispersão, pizza e interativos com Plotly
- **Banco de Dados** (`04_banco_dados/`): consultas SQL, modelagem relacional

Agora, o aluno vai projetar a interface de uma **dashboard** que apresenta esses dados de forma visual e interativa.

**Instruções:**
1. Escolha uma das ferramentas acima
2. Desenhe uma tela de dashboard com pelo menos:
   - Um título descritivo
   - Uma área de filtros (período, categoria, etc.)
   - 2–3 KPIs (números de destaque)
   - 2–3 áreas para gráficos (indique o tipo: barras, linhas, pizza, etc.)
3. Anote ao lado de cada área: **o que** ela mostra e **por que** o usuário precisa dessa informação

---

### Prática AI: descrever a interface e receber sugestões

**Dinâmica:**
1. O aluno descreve em texto a interface que acabou de desenhar
2. Envia a descrição ao AI Assistant com o seguinte pedido:

> **Contexto:** Estou criando uma dashboard de dados para um projeto de ciência de dados. Já trabalhei com Python, estatística, visualização com Seaborn/Matplotlib/Plotly e banco de dados SQL.
>
> **Objetivo:** Avaliar a usabilidade da minha interface.
>
> **Descrição da interface:**
> [Cole aqui a descrição do seu wireframe: quais seções existem, onde cada uma fica, que tipo de dado ou gráfico cada área mostra]
>
> **Pedido:** Sugira melhorias de usabilidade com base nos princípios de hierarquia visual, agrupamento lógico e simplicidade. Aponte problemas que um usuário iniciante poderia ter ao usar essa dashboard.

3. O aluno avalia as sugestões da AI e decide quais incorporar ao wireframe

---

## 📖 Conteúdo Assíncrono (até 2h)

### Parte 1 — Leitura: UX para iniciantes (30 min)

Objetivo: entender os fundamentos de UX Design com exemplos práticos de interfaces boas e ruins.

---

#### 1.1 O que torna uma interface "boa"?

Uma interface é boa quando o usuário **consegue completar sua tarefa sem pensar em como a interface funciona**. No contexto de uma dashboard de dados, isso significa:

- O usuário encontra a informação que procura em poucos segundos
- Os gráficos comunicam a mensagem sem precisar de explicação extra
- Os filtros são intuitivos e o resultado da filtragem é imediato
- Não há elementos decorativos que distraiam da informação

#### 1.2 Os 5 erros mais comuns em dashboards de dados

**Erro 1: Excesso de informação na mesma tela**
- ❌ Colocar 10 gráficos em uma única página sem hierarquia
- ✅ Destacar 2–3 KPIs no topo e 2–3 gráficos principais; detalhes ficam em abas ou scroll

**Erro 2: Gráfico errado para o dado**
- ❌ Usar pizza para comparar 15 categorias
- ✅ Usar barras horizontais para muitas categorias; pizza apenas para 3–5 fatias
- Referência: tipos de gráficos × objetivo (ver `03_visualizacao/`, Aula 01)

**Erro 3: Cores sem significado**
- ❌ Cada gráfico com uma paleta diferente e cores aleatórias
- ✅ Uma paleta consistente em toda a dashboard; cores de destaque apenas para chamar atenção a pontos importantes
- Referência: paleta personalizada (ver `03_visualizacao/`, Aula 10)

**Erro 4: Falta de contexto nos números**
- ❌ Exibir "1.847" sem rótulo, sem unidade e sem comparação
- ✅ Exibir "1.847 vendas este mês (↑ 12% vs. mês anterior)"

**Erro 5: Filtros escondidos ou confusos**
- ❌ Filtros em menu oculto, sem indicação de filtro ativo
- ✅ Filtros visíveis no topo ou lateral, com indicação clara do estado atual

#### 1.3 Anatomia de uma dashboard bem estruturada

```
┌─────────────────────────────────────────────────────┐
│  TÍTULO DA DASHBOARD              [Filtros: ▼ ▼ ▼]  │
├────────┬────────┬────────┬──────────────────────────┤
│  KPI 1 │  KPI 2 │  KPI 3 │      (espaço vazio       │
│  Valor │  Valor │  Valor │       proposital)         │
├────────┴────────┴────────┴──────────────────────────┤
│                                                      │
│    Gráfico principal (maior, mais importante)        │
│    Ex.: linha de tendência ao longo do tempo          │
│                                                      │
├─────────────────────────┬────────────────────────────┤
│                         │                            │
│   Gráfico secundário    │   Gráfico secundário       │
│   Ex.: barras por       │   Ex.: dispersão de        │
│   categoria             │   correlação               │
│                         │                            │
└─────────────────────────┴────────────────────────────┘
```

**Princípios aplicados:**
- **Hierarquia:** KPIs no topo (vistos primeiro), gráfico principal maior, secundários menores
- **Agrupamento:** filtros juntos, KPIs juntos, gráficos de detalhe juntos
- **Espaço vazio:** respiro visual, não é espaço desperdiçado

---

### Parte 2 — Tarefa: criar wireframe do projeto de integração (40 min)

Objetivo: aplicar os conceitos de UX para desenhar o wireframe completo da dashboard do projeto de integração.

---

#### Instruções

1. Revise os dados e gráficos que você criou nos módulos anteriores:
   - Que tipos de gráficos você produziu? (barras, linhas, dispersão, pizza, interativos)
   - Que dados você consultou no banco de dados? (tabelas, consultas SQL)
   - Que métricas estatísticas você calculou? (médias, medianas, correlações)

2. Decida **quem é o usuário** da sua dashboard:
   - É um gestor que quer ver resultados de alto nível?
   - É um analista que precisa explorar os dados em detalhe?
   - É um público geral que precisa de uma visão simplificada?

3. Desenhe o wireframe com as seguintes seções obrigatórias:

| Seção | Conteúdo | Referência no curso |
|---|---|---|
| **Cabeçalho** | Título da dashboard + área de filtros | Princípios de UX (este módulo) |
| **KPIs** | 2–3 indicadores numéricos de destaque | Estatística (`02_estatistica/`) — médias, medianas, extremos |
| **Gráfico principal** | Visualização mais importante do dataset | Visualização (`03_visualizacao/`) — escolha o tipo mais adequado |
| **Gráficos secundários** | 1–2 visualizações complementares | Visualização (`03_visualizacao/`) — barras, dispersão, pizza |
| **Fonte de dados** | Indicação de onde os dados vêm | Banco de Dados (`04_banco_dados/`) — tabelas e consultas SQL |

4. Para cada seção, escreva um **requisito** de 1–2 frases descrevendo:
   - O que a seção mostra
   - Que dado ou gráfico ela contém
   - Por que o usuário precisa dessa informação

---

### Parte 3 — Desafio AI: descrever o wireframe e pedir críticas de usabilidade (30 min)

Objetivo: usar o AI Assistant para obter uma avaliação crítica do wireframe e identificar pontos de melhoria antes de começar a codar.

---

#### Instruções

1. Escreva uma descrição textual completa do seu wireframe, seção por seção
2. Envie ao AI Assistant usando o template abaixo:

> **Contexto:** Sou aluno de um curso de Ciência de Dados e estou projetando uma dashboard. Nos módulos anteriores, trabalhei com:
> - Python: lógica, funções, listas e dicionários
> - Estatística: médias, medianas, correlação e projeções
> - Visualização: gráficos de barras, linhas, dispersão e interativos com Plotly
> - Banco de Dados: SQL com SQLite, consultas com SELECT, JOIN e GROUP BY
>
> **Descrição do wireframe:**
> [Descreva cada seção: cabeçalho, KPIs, gráfico principal, gráficos secundários, filtros, fonte de dados]
>
> **Pedido:** Analise meu wireframe como um especialista em UX. Para cada seção:
> 1. O layout faz sentido para o tipo de dado exibido?
> 2. A hierarquia visual está correta (informação mais importante primeiro)?
> 3. Um usuário que nunca viu essa dashboard saberia o que fazer?
> 4. Que melhorias de usabilidade você sugere?

3. Avalie as sugestões da AI:
   - Quais fazem sentido para o seu projeto?
   - Quais são excessivas ou fora do escopo?
   - Quais você vai incorporar ao wireframe final?

4. Atualize seu wireframe com as melhorias escolhidas

---

### Parte 4 — Checklist: revisão do protótipo antes de começar a codar (20 min)

Objetivo: garantir que o wireframe está completo e pronto para ser implementado.

---

#### Checklist de revisão

Antes de começar a codar, marque cada item:

**Layout e hierarquia**
- [ ] A dashboard tem um título descritivo que explica o que está sendo mostrado
- [ ] Os KPIs aparecem no topo e são visíveis sem scroll
- [ ] O gráfico mais importante é o maior e/ou está na posição de maior destaque
- [ ] Os filtros estão visíveis e acessíveis (não escondidos em menus)
- [ ] Há espaço vazio intencional (a tela não está sobrecarregada)

**Dados e gráficos**
- [ ] Cada gráfico tem um tipo adequado ao dado que representa (referência: `03_visualizacao/`, Aula 01)
- [ ] Os KPIs têm rótulo, valor e contexto (unidade, variação ou comparação)
- [ ] As fontes de dados estão identificadas (quais tabelas ou consultas SQL alimentam cada seção)
- [ ] As métricas estatísticas usadas estão corretas para o tipo de análise (referência: `02_estatistica/`)

**Usabilidade**
- [ ] Um usuário que nunca viu a dashboard saberia o que cada seção mostra
- [ ] As cores têm significado consistente em toda a interface
- [ ] Não há gráficos redundantes (dois gráficos mostrando a mesma coisa de formas diferentes sem motivo)
- [ ] A AI revisou o wireframe e as sugestões relevantes foram incorporadas

**Requisitos escritos**
- [ ] Cada seção tem um requisito escrito de 1–2 frases
- [ ] Os requisitos descrevem: o que mostra, que dado usa e por que o usuário precisa
- [ ] Os requisitos são claros o suficiente para outra pessoa entender sem ver o wireframe

---

## 📦 Entregável

O aluno entrega:

1. **Wireframe da dashboard** — esboço visual (papel, Paint, Draw.io, Excalidraw ou Figma) com todas as seções obrigatórias
2. **Requisitos escritos** — para cada seção do wireframe, 1–2 frases descrevendo conteúdo, dado utilizado e justificativa
3. **Registro da avaliação da AI** — captura ou cópia das sugestões de usabilidade recebidas e quais foram incorporadas
4. **Checklist preenchido** — todos os itens verificados antes de começar a codificação

---

## Resumo Geral

| # | Parte | Tipo | Duração |
|---|---|---|---|
| — | Aula ativa: UX, wireframe e prática AI | Presencial com instrutor | 1h |
| 1 | Leitura: UX para iniciantes | Assíncrono — leitura | 30 min |
| 2 | Tarefa: wireframe do projeto de integração | Assíncrono — prática | 40 min |
| 3 | Desafio AI: críticas de usabilidade | Assíncrono — prática com AI | 30 min |
| 4 | Checklist: revisão do protótipo | Assíncrono — verificação | 20 min |

---

## Referências

| Recurso | Localização |
|---|---|
| Notebooks de Python (Aulas 01–05) | `01_python/` |
| Plano de aula de Estatística | `02_estatistica/Plano_de_aula.md` |
| Conteúdo de Visualização de Dados | `03_visualizacao/CONTEUDO.md` |
| Plano de aula de Visualização | `03_visualizacao/PLANO_DE_AULA.md` |
| Conteúdo de Banco de Dados | `04_banco_dados/CONTEUDO.md` |
| Plano de aula de Banco de Dados | `04_banco_dados/PLANO_DE_AULA.md` |
| Módulo 1 — Primeiro Contato com AI | `05_dev_com_ai/modulo01_primeiro_contato_ai/` |
| Módulo 2 — Revisão com AI | `05_dev_com_ai/modulo02_revisao_com_ai/` |
