# Projeto Integrador — Visualização de Dados

## Sobre o Conteúdo

Módulo final do curso. O aluno finaliza a dashboard, documenta seu processo de uso da AI ao longo de toda a trilha e apresenta o projeto para a turma. Este módulo não introduz conceitos novos — é dedicado a **polir, documentar e apresentar** o trabalho construído ao longo dos módulos anteriores.

**Formato:** Aula ativa de mentoria + conteúdo assíncrono de finalização
**Carga horária total:** 3h (1h aula ativa + até 2h assíncrono)
**Pré-requisitos:** Todos os módulos anteriores concluídos, com a dashboard em andamento (Módulos 6–9)
**Instrutores:** Todos os instrutores da trilha

---

## 🎯 Aula Ativa (1h)

### Bloco 1 — Revisão e correções finais com mentoria (30 min)

#### Dinâmica

Sessão de mentoria individual/em pequenos grupos. Cada aluno apresenta o estado atual da sua dashboard e recebe feedback dos instrutores para ajustes finais.

**Roteiro de revisão:**

O aluno abre sua dashboard e, junto com o instrutor, percorre o checklist:

**Funcionalidade**
- [ ] A página carrega sem erros no console do navegador
- [ ] Os KPIs são populados dinamicamente a partir dos dados
- [ ] A tabela é gerada a partir do array de dados
- [ ] Os filtros (dropdown/botão) funcionam e atualizam tabela e gráficos
- [ ] Pelo menos 3 gráficos Chart.js estão funcionando
- [ ] Os gráficos correspondem a análises da trilha de ciência de dados

**Estrutura e estilo**
- [ ] HTML semântico: `header`, `main`, `section`, `article`, `footer`
- [ ] CSS responsivo: layout funciona em desktop e celular
- [ ] Hierarquia visual: KPIs no topo, gráfico principal em destaque
- [ ] Cores consistentes e com contraste acessível

**Dados**
- [ ] Os dados são compatíveis com a trilha (Python, Estatística, Visualização, BD)
- [ ] As métricas estatísticas estão corretas (médias, totais, máximos)
- [ ] A fonte dos dados está indicada no rodapé

**Tratamento de erros**
- [ ] Dados vazios mostram mensagem apropriada
- [ ] Estado de loading visível durante processamento

#### Correções rápidas com AI

Se o instrutor identificar um problema, o aluno **corrige usando o ciclo AI** — não o instrutor. O instrutor aponta o problema; o aluno formula o requisito, gera a correção com AI e valida.

---

### Bloco 2 — Documentar o uso de AI no projeto (15 min)

#### O que é o Diário de Campo?

Um documento curto (1–2 páginas) onde o aluno registra como usou a AI ao longo do projeto. Não é um relatório formal — é uma reflexão honesta sobre o processo.

**Estrutura do Diário de Campo:**

```markdown
# Diário de Campo — [Nome do Aluno]

## 3 Melhores Prompts que Usei

### Prompt 1: [título descritivo]
**Módulo:** [em qual módulo usou]
**Prompt enviado:**
> [cole o prompt exato]

**Por que foi bom:**
[1–2 frases explicando por que esse prompt gerou um resultado útil]

### Prompt 2: [título descritivo]
...

### Prompt 3: [título descritivo]
...

## 1 Erro que a AI Cometeu e Como Corrigi

**Módulo:** [em qual módulo aconteceu]
**O que pedi:**
> [prompt enviado]

**O que a AI errou:**
[descreva o erro]

**Como corrigi:**
[o que você fez para resolver — reformulou o prompt? corrigiu manualmente? pediu revisão?]

## 1 Coisa que Aprendi Graças à Explicação da AI

**Módulo:** [em qual módulo aconteceu]
**O que perguntei:**
> [pergunta feita à AI]

**O que aprendi:**
[explique o conceito que entendeu graças à resposta da AI]

**Como usei esse conhecimento depois:**
[onde aplicou esse aprendizado no projeto]
```

#### Atividade em aula

O aluno começa a preencher o Diário de Campo durante a aula, revisando as conversas que teve com a AI ao longo dos módulos. Não precisa terminar em aula — pode finalizar no conteúdo assíncrono.

---

### Bloco 3 — Apresentação para a turma (15 min)

#### Formato da apresentação

Cada aluno tem **3–5 minutos** para apresentar. Pode ser:

- **Demo ao vivo:** abre a dashboard no navegador e navega, mostrando filtros, gráficos e interações
- **Slides (2–3):** capturas de tela da dashboard + destaques do Diário de Campo

#### Roteiro sugerido (3–5 min)

| Tempo | Conteúdo |
|---|---|
| 0:00 – 1:00 | **O que a dashboard mostra:** que dados, que métricas, para que público |
| 1:00 – 2:30 | **Demo:** navegar pela dashboard mostrando KPIs, filtros, gráficos |
| 2:30 – 4:00 | **Destaque do Diário de Campo:** melhor prompt OU erro da AI OU aprendizado |
| 4:00 – 5:00 | **Perguntas da turma** |

#### Critérios de avaliação da apresentação

| Critério | O que é avaliado |
|---|---|
| **Funcionalidade** | A dashboard funciona? KPIs, tabela, filtros e gráficos operam corretamente? |
| **Integração com a trilha** | Os dados e gráficos são compatíveis com o que foi trabalhado na trilha de ciência de dados? |
| **UX e design** | A interface segue os princípios de UX do Módulo 6? Hierarquia, agrupamento, responsividade? |
| **Uso da AI** | O aluno demonstra que usou a AI de forma crítica? Sabe explicar escolhas? Identificou erros? |
| **Comunicação** | A apresentação é clara, objetiva e respeita o tempo? |

---

## 📖 Conteúdo Assíncrono (até 2h)

### Parte 1 — Finalizar a página: ajustes visuais, responsividade, testes (50 min)

Objetivo: polir a dashboard para a entrega final.

---

#### 1.1 Ajustes visuais

Revise e corrija os seguintes pontos:

**Tipografia e espaçamento**
- [ ] Títulos com tamanho hierárquico (`h1` > `h2` > `h3`)
- [ ] Espaçamento consistente entre seções (`margin` e `padding` padronizados)
- [ ] Texto legível: tamanho mínimo de `16px` para corpo, `14px` para rótulos

**Cores**
- [ ] Paleta consistente em toda a dashboard (referência: `03_visualizacao/`, Aula 10)
- [ ] Cores de gráficos Chart.js alinhadas com a paleta geral
- [ ] Contraste de texto suficiente (mínimo 4.5:1)

**Gráficos**
- [ ] Todos os gráficos têm título visível
- [ ] Legendas posicionadas de forma que não sobreponham dados
- [ ] Tooltips exibem informação útil ao passar o mouse

#### 1.2 Responsividade

Teste a dashboard em diferentes larguras:

| Largura | Dispositivo | O que verificar |
|---|---|---|
| 1200px+ | Desktop | Layout completo, KPIs lado a lado, gráficos em grid |
| 768px–1024px | Tablet | KPIs podem quebrar em 2 colunas, gráficos em coluna única |
| 375px | Celular | Tudo em coluna única, filtros acessíveis, gráficos legíveis |

**Como testar no navegador:**
1. Abra a dashboard no Chrome/Edge
2. Pressione `F12` para abrir DevTools
3. Clique no ícone de dispositivos (ou `Ctrl+Shift+M`)
4. Selecione diferentes tamanhos de tela

**Se algo quebrar, use a AI:**

> "Minha dashboard quebra em tela de 375px. A seção de KPIs não empilha corretamente. Aqui está o CSS atual: [cole o CSS]. Corrija para que os cards fiquem empilhados no celular."

#### 1.3 Testes funcionais

Para cada funcionalidade, execute o teste manualmente:

| Funcionalidade | Teste | Resultado esperado |
|---|---|---|
| KPIs | Verificar se os valores correspondem aos dados | Total, média e máximo corretos |
| Tabela | Verificar se todas as linhas aparecem | Mesma quantidade de linhas que o array de dados |
| Filtro | Selecionar cada opção do dropdown | Tabela e gráficos atualizam corretamente |
| Ordenação | Clicar no botão de ordenar | Dados reorganizados e direção indicada visualmente |
| Gráficos | Passar mouse sobre barras/pontos | Tooltip exibe valor correto |
| Responsivo | Redimensionar a janela | Layout se adapta sem quebrar |
| Dados vazios | Filtrar por categoria sem dados | Mensagem "Nenhum dado encontrado" |

---

### Parte 2 — Escrever o Diário de Campo (40 min)

Objetivo: documentar o processo de uso da AI ao longo do projeto.

---

#### Instruções

1. Revise suas conversas com a AI ao longo dos módulos (se salvou o histórico)
2. Preencha o Diário de Campo seguindo a estrutura apresentada na aula ativa
3. Seja honesto — o objetivo não é mostrar perfeição, mas reflexão

#### Conteúdo obrigatório

**3 melhores prompts que usou e por quê**

Escolha os prompts que geraram os melhores resultados. Para cada um:
- Em qual módulo usou (Módulo 1 a 9)
- O prompt exato que enviou
- Por que foi eficaz (era específico? dava contexto? pedia formato claro?)

**Dica:** bons prompts geralmente seguem o template do Módulo 1 (Contexto, Objetivo, Detalhes, Formato).

**1 erro que a AI cometeu e como corrigiu**

Descreva uma situação em que a AI gerou algo errado. Pode ser:
- Código com bug
- Sugestão de tag HTML inadequada
- Explicação incorreta
- Gráfico com tipo errado para o dado

Explique como você identificou o erro e o que fez para resolver.

**1 coisa que aprendeu graças à explicação da AI**

Descreva um conceito que você realmente entendeu porque pediu explicação à AI. Pode ser:
- "Entendi a diferença entre `forEach` e `map` quando a AI explicou que `map` retorna um novo array"
- "Entendi por que `flexbox` é melhor que `float` para layout quando a AI mostrou o exemplo"
- "Entendi como `reduce` acumula valores quando a AI comparou com o acumulador do `while` do Python"

---

### Parte 3 — Preparar apresentação (30 min)

Objetivo: preparar uma apresentação de 3–5 minutos (demo ao vivo ou 2–3 slides).

---

#### Opção A — Demo ao vivo

1. Abra a dashboard no navegador
2. Planeje a navegação: qual seção mostrar primeiro, em que ordem
3. Ensaie em 3–5 minutos, cronometrando
4. Prepare-se para perguntas da turma

**Roteiro de demo:**
- Abrir a dashboard → mostrar visão geral (título, KPIs, layout)
- Interagir com um filtro → mostrar tabela e gráficos atualizando
- Mostrar um gráfico de perto → explicar o que ele comunica
- Destacar 1 ponto do Diário de Campo (melhor prompt, erro ou aprendizado)

#### Opção B — Slides (2–3)

| Slide | Conteúdo |
|---|---|
| 1 | Captura de tela da dashboard + título + "Que dados mostra e para quem" |
| 2 | Detalhes: quais gráficos usou, que métricas calculou, como os filtros funcionam |
| 3 | Destaque do Diário de Campo: melhor prompt OU erro da AI OU aprendizado |

**Dica:** use a própria AI para ajudar a estruturar os slides:

> "Tenho 3 minutos para apresentar minha dashboard de dados. Ela tem: [descreva]. Me ajude a organizar o roteiro da apresentação em 3 slides."

---

## 🎯 Entrega Final

O aluno entrega **três artefatos** que representam o trabalho de toda a trilha:

### ✅ 1. Dashboard funcional

**Arquivos:** `index.html`, `style.css`, `script.js`

| Requisito | Referência |
|---|---|
| HTML semântico (`header`, `main`, `section`, `article`, `footer`) | Módulo 7 |
| CSS responsivo (flexbox, media queries) | Módulo 7 |
| Dados carregados em array de objetos JS | Módulo 8 |
| KPIs dinâmicos (total, média, máximo) | Módulos 8 + `02_estatistica/` |
| Tabela HTML gerada dinamicamente | Módulo 8 |
| Filtro por categoria funcionando | Módulo 8 |
| Pelo menos 3 gráficos Chart.js | Módulo 9 + `03_visualizacao/` |
| Gráficos correspondentes à trilha de ciência de dados | Módulo 9 + `03_visualizacao/` |
| Tratamento de loading e dados vazios | Módulo 9 |
| Layout responsivo testado em desktop e celular | Módulos 7 + 9 |

### ✅ 2. Diário de Campo

**Formato:** Arquivo `.md` ou documento de texto

| Seção | Conteúdo |
|---|---|
| 3 melhores prompts | Prompt exato + módulo + por que foi bom |
| 1 erro da AI | O que pediu, o que a AI errou, como corrigiu |
| 1 aprendizado com AI | O que perguntou, o que aprendeu, como usou depois |

### ✅ 3. Apresentação

**Formato:** Demo ao vivo (3–5 min) ou slides (2–3)

| Critério | Peso |
|---|---|
| Dashboard funciona corretamente | Essencial |
| Integração com a trilha de ciência de dados é visível | Essencial |
| Princípios de UX aplicados | Importante |
| Uso crítico da AI demonstrado | Importante |
| Apresentação clara e dentro do tempo | Desejável |

---

## Resumo Geral

| # | Parte | Tipo | Duração |
|---|---|---|---|
| — | Aula ativa: mentoria, Diário de Campo, apresentação | Presencial | 1h |
| 1 | Finalizar página: visuais, responsividade, testes | Assíncrono — prática | 50 min |
| 2 | Escrever Diário de Campo | Assíncrono — reflexão | 40 min |
| 3 | Preparar apresentação | Assíncrono — preparação | 30 min |

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
| Módulo 9 — Dados no Frontend e Integração | `05_dev_com_ai/modulo09_dados_frontend_integracao/` |
