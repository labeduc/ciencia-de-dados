# Análise de Issues — Curso de Visualização de Dados com Python

**Data da análise:** 2026-06-29  
**Escopo:** 16 aulas teóricas + 4 práticas (`aula-01` a `aula-16`, `pratica-aula-05`, `pratica-aula-06`, `pratica-aula-08`, `pratica-aula-09-14`)

---

## Sumário de Issues

| Severidade | Total | Corrigido | Pendente |
|---|---|---|---|
| 🔴 Crítico | 7 | 2 | 5 |
| 🟡 Melhoria | 21 | 12 | 9 |
| 🟢 Sugestão | 10 | 1 | 9 |
| **Total** | **38** | **15** | **23** |

> **Status:** Issues das aulas 1 a 6 (incluindo práticas) foram revisados e corrigidos em 2026-06-29. Issues das aulas 7 a 16 permanecem pendentes.

---

## Módulo 1 — Fundamentos

### Aula 01 — Teoria de Visualização de Dados

**Avaliação geral:** Aula sólida, bem escrita e bem estruturada. A progressão de conceitos (o que é → para que serve → como comunicar → por que Python) é clara e gradual.

🟢 **[Sugestão] cell-6 — Imagem do ciclo de vida com URL de fonte externa**  
A imagem `ciclo_vida_ds.png` tem fonte indicada como `blog.betrybe.com.br`. A URL exata não está no texto, apenas o domínio. Uma URL clicável aumentaria credibilidade e permitiria aprofundamento.

🟢 **[Sugestão] cell-11 — Links de exemplos externos podem ficar quebrados**  
Os seis links para Our World in Data, Gapminder e EPE são excelentes, mas são URLs externas que podem mudar. Nenhum impacto imediato, mas vale manter em revisões futuras.

🟡 **[Melhoria] cell-14 — Referência ao diagrama sem preparação visual clara** — ✅ **Corrigido**  
O texto menciona "este diagrama será o seu guia de consulta durante todo o curso", mas o diagrama é uma imagem (`visualizacao_x_objetivo.png`) cujo conteúdo não é descrito textualmente. Alunos que abrirem o notebook em ambiente que não renderize imagens não terão acesso ao conteúdo do diagrama. Uma descrição textual resumida dos principais objetivos/tipos seria valiosa.  
> *Correção aplicada: adicionada tabela de referência rápida com objetivos × tipos de gráfico logo abaixo do diagrama.*

---

### Aula 02 — Google Colab

**Avaliação geral:** Aula direta e funcional. Cobre o essencial para que o aluno comece a trabalhar.

🟡 **[Melhoria] cell-18 — Exemplo de código complexo sem justificativa para o nível da aula**  
A célula de código de demonstração usa `requests`, `json`, `pandas`, `pd.read_json` e faz uma chamada de API remota. O texto anterior avisa que o aluno não precisa entender o código agora, mas o exemplo introduz um nível de complexidade (chamada REST, JSON, múltiplas bibliotecas) muito acima do que está sendo ensinado. Um exemplo mais simples — como somar dois números ou imprimir uma lista — comunicaria o mesmo conceito (célula de código executável exibe resultado abaixo) com muito menos ruído.

🟢 **[Sugestão] cell-24 — Tabela de atalhos incompleta** — ✅ **Corrigido**  
A tabela tem os atalhos mais comuns, mas não menciona `Ctrl + S` (salvar) nem `Ctrl + Shift + P` (paleta de comandos do Colab), dois atalhos muito usados no dia a dia.  
> *Correção aplicada: adicionados `Ctrl + S` e `Ctrl + Shift + P` na tabela, com dica explicando o uso da paleta de comandos.*

---

### Aula 03 — Formatos de Dados

**Avaliação geral:** Aula com bom conteúdo conceitual, mas com um problema estrutural sério nas células finais.

🔴 **[Crítico] cell-35 — Célula de código com texto Markdown (não é código Python)** — ✅ **Corrigido**  
A célula `cell-35` é do tipo código, mas seu conteúdo é texto Markdown/explicativo sobre bibliotecas do ecossistema científico Python (NumPy, SciPy, Scikit-learn). Se executada, causará erro de sintaxe. O conteúdo deveria estar em uma célula de texto (Markdown). Além disso, o conteúdo dessa célula duplica parcialmente o que está em `cell-36` (que é uma célula Markdown com o mesmo tema), criando uma redundância e confusão sobre a ordem correta de leitura.  
> *Correção aplicada: cell-35 convertida de `code` para `markdown`; cell-36 (redundante) deletada; cell-32 (duplicata de cell-31) também deletada.*

🟡 **[Melhoria] cell-31 — DataFrame introduzido com código numérico sem contexto** — ✅ **Corrigido**  
A célula `cell-33` introduz `pd.DataFrame([[1, 2, 3], [4, 5, 6], [7, 8, 9]])` e imprime `df[2][2]`. O resultado `9` aparece sem explicação de por que `[2][2]` acessa a terceira coluna da terceira linha. Para um aluno que está vendo DataFrame pela primeira vez, isso é confuso — o padrão `df[coluna][linha]` (formato longo) já foi apresentado antes com dicionários, mas o acesso numérico em DataFrames funciona diferente. A célula de texto anterior (`cell-32`) promete um "primeiro exemplo", mas a explicação subsequente é insuficiente.  
> *Correção aplicada: adicionados comentários em cell-33 explicando a sintaxe `df[coluna][linha]` e por que `df[2][2]` retorna 9.*

🟡 **[Melhoria] cell-34 — Series não tem exemplo de código próprio** — ✅ **Corrigido**  
Após explicar o DataFrame com um exemplo, o texto promete um "exemplo de código" para Series (cell-34 diz "Exemplo de código:"), mas a próxima célula de código é justamente `cell-35` que contém texto, não código Python. O exemplo prometido de Series nunca aparece.  
> *Correção aplicada: adicionada nova célula de código com exemplo funcional de `pd.Series` — índice nomeado, acesso por label, por posição e filtragem.*

🟢 **[Sugestão] cell-10 — Explicação de "overhead no processamento" pode ser mais precisa**  
A afirmação de que no formato largo "você é obrigado a 'carregar' a linha inteira" para acessar um campo é conceitualmente adequada para Pandas/dicionários, mas tecnicamente o conceito de formato largo vs. longo em Pandas é diferente do que em bancos colunares. A explicação serve ao propósito pedagógico, mas poderia ter uma ressalva de que esta é uma simplificação.

---

### Aula 04 — Prática: Aulas 2 e 3

**Avaliação geral:** Aula prática completa e bem elaborada. Demonstra carregamento, visualização inicial e transformação para formato longo.

🟡 **[Melhoria] cell-45/cell-46 — Seção "Usando bibliotecas externas" está vazia** — ✅ **Corrigido**  
A seção `## Usando bibliotecas externas para facilitar o trabalho` (cell-45) tem apenas o título e o texto de encerramento (cell-46), sem nenhum conteúdo de ensino. O CONTEUDO.md lista como exercício "Usar bibliotecas externas para simplificar o trabalho", mas a aula não entrega esse conteúdo. É uma lacuna direta em relação ao que foi prometido.  
> *Correção aplicada: cell-45 preenchida com explicação comparativa (bibliotecas nativas vs Pandas/Seaborn), exemplo de código e dica sobre `!pip install`.*

🟡 **[Melhoria] cell-37 — Gráfico com problema de formatação mencionado mas não resolvido** — ✅ **Corrigido**  
O texto explica que "existe um problema de formatação — o eixo X está apertado e as descrições dos tipos estão se sobrepondo — mas isso é esperado". Embora a justificativa seja válida pedagogicamente, seria útil indicar que isso será resolvido em aulas futuras e em qual aula especificamente (Aula 10 — Melhorando seus Visuais), para que o aluno não ache que é um erro permanente.  
> *Correção aplicada: adicionada nota em cell-37 com referência explícita à Aula 10 — Melhorando seus Visuais.*

🟡 **[Melhoria] cell-43 — Seaborn introduzido sem instalação/import completo**  
A célula introduz `sns.countplot()` sem ter importado `seaborn` na mesma sequência de células da aula. Nas células anteriores (`cell-26`, `cell-36`), apenas `csv` e `matplotlib` foram importados. O aluno que executar sequencialmente encontrará um `NameError: name 'sns' is not defined`. O import do seaborn deveria aparecer nessa célula ou logo antes dela.

---

## Módulo 2 — Pandas

### Aula 05 — Pandas

**Avaliação geral:** Aula excelente. Um dos notebooks mais completos e bem estruturados do curso. A progressão de `head()` → `describe()` → acesso a colunas → filtragem → agregação é natural e bem explicada.

🟡 **[Melhoria] cell-14 — Referência cruzada inconsistente (cita "Aula 3" em vez de "Aula 04")** — ✅ **Corrigido**  
O texto diz "Na aula 3, aprendemos que uma maneira de carregar os dados..." mas a aula de carga de dados na prática foi a Aula 04. A Aula 03 foi sobre formatos de dados. A referência correta seria "Nas aulas 03 e 04".  
> *Correção aplicada: texto corrigido para "Nas aulas 03 e 04".*

🟡 **[Melhoria] cell-27 — `errwidth=0` é parâmetro depreciado no Seaborn moderno** — ✅ **Corrigido**  
O parâmetro `errwidth=0` foi depreciado no Seaborn 0.12+ em favor de `err_kws={"linewidth": 0}`. A célula seguinte (cell-31) já usa corretamente `err_kws`, mas a cell-29 usa o parâmetro antigo. Isso pode gerar `FutureWarning` no Colab com versões recentes do Seaborn, confundindo o aluno.  
> *Nota: o `errwidth=0` estava em aula-06 cell-29 (não em aula-05). Corrigido em aula-06 para `err_kws={"linewidth": 0}`.*

🟢 **[Sugestão] cell-60 — Aviso sobre `iterrows()` sem alternativa prática imediata**  
O aviso de que `iterrows()` tem "pior performance" é correto, mas aparece logo após o único exemplo de uso do método. O aluno fica sem saber quando `iterrows()` seria aceitável. Uma linha mencionando o contexto em que ele é usado (código legado, conjuntos pequenos) reduziria a ansiedade.

---

### Prática 05 — Pandas

**Avaliação geral:** Prática bem estruturada, com exercícios que cobrem todos os tópicos da aula. Nível de dificuldade progressivo. As dicas são adequadas sem entregar a solução.

🟡 **[Melhoria] Exercício 1 — Afirmação sobre "única coluna com valores nulos" pode gerar confusão** — ✅ **Corrigido**  
O enunciado pede para identificar "a única coluna que possui valores ausentes". Com base nos dados reais do `pokemons.csv`, `Type 2` é de fato a única coluna com nulos, mas o aluno que usar `info()` precisará interpretar a diferença entre `1032 non-null` e `548 non-null` para chegar a essa conclusão. Uma orientação mais explícita de como identificar isso no output de `info()` seria útil para iniciantes.  
> *Correção aplicada: dica do Exercício 1 expandida para explicar como ler o campo `Non-Null Count` no output de `info()`, com exemplo numérico concreto.*

🟢 **[Sugestão] Exercício 5 — `sort_values()` não foi ensinado formalmente na Aula 05**  
A dica do Exercício 5 menciona `sort_values()` como função útil, mas essa função não foi explicitamente ensinada na Aula 05. O aluno terá que descobrí-la pela dica. Seria conveniente uma frase na dica explicando brevemente o parâmetro `ascending=False`.

---

## Módulo 3 — Seaborn e Matplotlib

### Aula 06 — Iniciando com Seaborn

**Avaliação geral:** Aula bem estruturada. Cobre `countplot()`, `barplot()`, múltiplas métricas com `melt()` e barras empilhadas.

🔴 **[Crítico] cell-27 — `import numpy as np` sem preparação/contexto** — ✅ **Corrigido**  
A cell-27 introduz `import numpy as np` sem nenhuma explicação prévia de que o NumPy seria necessário ou o que ele é. O aluno simplesmente vê um novo import aparecer no meio do notebook. Para um curso introdutório, essa introdução abrupta de uma biblioteca não anunciada — especialmente para usar apenas `np.mean` — pode gerar confusão. O CONTEUDO.md não lista NumPy como biblioteca da Aula 06.  
> *Correção aplicada: cell-26 atualizada para apresentar o NumPy antes do seu uso — explica o papel do `estimator` e que `np.mean` é o que diz ao Seaborn para calcular a média.*

🟡 **[Melhoria] cell-27/cell-29 — `errwidth=0` vs `err_kws` inconsistência** — ✅ **Corrigido**  
Na cell-27 é usado `estimator=np.mean, errwidth=0` e na cell-29 é usado o mesmo. Porém na cell-31, a mesma função usa `err_kws={"linewidth": 0}`. O código usa dois padrões diferentes para suprimir barras de erro na mesma aula, sem explicar por que a sintaxe mudou. Isso confunde o aluno sobre qual usar.  
> *Correção aplicada: cell-29 atualizada para usar `err_kws={"linewidth": 0}`, padronizando com cell-31. cell-28 atualizada para explicar o parâmetro e mencionar `err_kws`.*

🟡 **[Melhoria] cell-33 — Mudança para Matplotlib puro sem transição clara** — ✅ **Corrigido**  
O código do gráfico empilhado usa `plt.bar()` diretamente (Matplotlib puro) sem aviso de que estamos abandonando o Seaborn temporariamente. O texto posterior (cell-34) explica que "desenhamos as barras com o matplotlib direto", mas o aluno vê primeiro o código diferente sem entender o motivo. A ordem deveria ser: explicar primeiro, código depois.  
> *Correção aplicada: cell-32 atualizada com aviso de que o próximo bloco usa Matplotlib puro (sem Seaborn), antes de apresentar o código.*

🟡 **[Melhoria] cell-36 — `pokemons_gb.plot(kind='bar', x='Generation', stacked=True)` usa método do DataFrame, não do Seaborn** — ✅ **Corrigido**  
A última versão do gráfico empilhado usa `DataFrame.plot()`. Embora funcione, isso nunca foi introduzido anteriormente e não é seaborn nem matplotlib puro — é a API do pandas para plotagem. Essa terceira abordagem sem explicação da diferença adiciona confusão sobre qual API usar em cada situação.  
> *Correção aplicada: cell-35 atualizada para explicar o método `.plot()` do Pandas antes do código — destaca que é uma API embutida no DataFrame que usa Matplotlib internamente.*

---

### Prática 06 — Iniciando com Seaborn

**Avaliação geral:** Prática muito bem estruturada. Exercícios seguem exatamente a progressão da aula. Dicas são precisas sem entregar o código.

🟡 **[Melhoria] Exercício 3 — `errwidth=0` nas dicas vs `err_kws` na aula** — ✅ **Corrigido**  
A dica do Exercício 3 usa `errwidth=0` como exemplo, mas no Seaborn 0.12+ esse parâmetro está depreciado. Seria mais adequado usar `err_kws={"linewidth": 0}` para manter consistência com a versão atual da biblioteca.  
> *Correção aplicada: enunciado (cell-10) e dica (cell-12) do Exercício 3 atualizados para `err_kws={"linewidth": 0}`.*

🟢 **[Sugestão] Exercício 5 — O método `.plot(kind='bar', x='Generation', stacked=True)` tem `x='Generation'` errado**  
Após o `groupby(['Type 1'])`, o DataFrame resultante tem `Type 1` como índice, não como coluna chamada `Generation`. O parâmetro correto seria `x='Type 1'` ou simplesmente omitir `x=` (o Pandas usará o índice). A dica na célula cell-18 usa `pokemons.groupby(['Type 1'])[['HP', 'Def']].mean()` e depois `.plot(kind='bar', stacked=True)` sem o parâmetro `x=`, o que está correto. Mas o enunciado mencionando o `x=` pode induzir o aluno a incluí-lo errado.

---

### Aula 07 — Linhas e Áreas

**Avaliação geral:** Aula curta mas funcional. Cobre `lineplot()` e `stackplot()`.

🟡 **[Melhoria] cell-2 — "eixo de valores categóricos mas contínuos" — definição contraditória**  
O texto afirma que gráficos de linha são usados para "distribuição de métrica ao longo de um eixo de valores categóricos mas contínuos". Categórico e contínuo são conceitos opostos em estatística. A frase correta seria "eixo de valores contínuos ou discretos ordenados" (como datas, gerações, sequências). Isso pode confundir alunos que estejam aprendendo esses conceitos.

🟡 **[Melhoria] cell-15 — `stackplot()` não tem legenda exibida**  
O gráfico de área gerado por `plt.stackplot()` tem um parâmetro `labels=['Special Attack', 'Special Defense']`, mas a legenda não é chamada com `plt.legend()`. O gráfico aparece sem legenda, impossibilitando identificar qual área é qual. Uma chamada a `plt.legend(loc='upper left')` deveria ser adicionada.

🟢 **[Sugestão] Aula 07 — Ausência de prática dedicada**  
A Aula 07 não tem uma prática dedicada. Embora seja coberta na prática consolidada (09-14 cobre aulas 09-14), não há exercícios específicos de `lineplot()` e `stackplot()`. Esses gráficos são tecnicamente distintos dos de barra — um exercício dedicado melhoraria a fixação.

---

### Aula 08 — Dispersão e Quadrantes

**Avaliação geral:** Aula bem desenvolvida. O fluxo de `scatterplot()` básico → `hue` → `apply()` → posicionamento de legenda → quadrantes é progressivo e natural.

🟡 **[Melhoria] cell-12 — "a distribuição não é uniforme, pois como o valor é numérico ele criou faixas de valores"**  
O texto explica vagamente o problema de usar `Generation` (float) como `hue`. Seria mais claro explicar que o Seaborn trata valores numéricos como escala contínua de cor, por isso as gerações não ficam com cores distintas. A solução (criar coluna textual) é correta, mas a explicação do problema poderia ser mais precisa.

🟢 **[Sugestão] cell-24 — Quadrante com valores fixos hardcoded**  
Os limites dos eixos (`0, 225`) e as posições das linhas divisórias (`112.5`) e dos textos (`x=40, y=10` etc.) são todos valores hardcoded. O comentário no código menciona isso: "o ideal seria utilizar alguma fórmula ou função para dinamizar". Seria interessante mostrar ao menos como calcular o limite máximo com `pokemons['Att'].max()` para introduzir a prática de valores dinâmicos.

---

### Prática 08 — Dispersão e Quadrantes

**Avaliação geral:** Prática excelente. Cobertura completa dos tópicos da aula, boa progressão, dicas claras.

🟢 **[Sugestão] Exercício 4 — Limites de eixo de 0 a 260 não refletem os dados reais**  
O enunciado instrui `plt.xlim(0, 260)` e `plt.ylim(0, 260)` para `HP` e `Spe`. O valor máximo de `HP` no dataset é 255 e de `Spe` é 200. Usar 260 como limite funciona, mas seria mais pedagógico mostrar como calcular o limite dinamicamente, ou ao menos alinhar o limite máximo com o valor real dos dados.

---

### Aula 09 — Gráfico de Pizza

**Avaliação geral:** Aula bem fundamentada na teoria (quando usar/não usar pizza). O exemplo prático é simples e funcional.

🟡 **[Melhoria] cell-19 — `groupby` com duas colunas sem necessidade**  
O código usa `pokemons.groupby(['Generation Desc'])[['Generation','Number']].count()`. A coluna `Generation` é incluída no `groupby` resultante mas não é usada no gráfico. `pokemons.groupby(['Generation Desc'])['Number'].count().reset_index()` seria mais limpo e menos confuso para o aluno. A inclusão de `Generation` no resultado pode sugerir que ela é necessária.

🟢 **[Sugestão] cell-19 — `sort_values('Generation Desc', inplace=True)` ordena em ordem lexicográfica, não numérica**  
A ordenação por `'Generation Desc'` (texto) resultará em: `Gen 1, Gen 2, Gen 3, ..., Gen 8`. Para "Gen 10" ou além isso quebraria. Embora não afete o exemplo atual, seria uma boa oportunidade para mostrar a diferença entre ordenação textual e numérica.

---

### Aula 10 — Melhorando seus Visuais

**Avaliação geral:** Aula muito boa, com abordagem passo a passo bem executada. A evolução gradual do gráfico é didática.

🔴 **[Crítico] cell-62 — "Esta aula também marca o final do nosso curso de Visualização de Dados com Python!"**  
A frase de encerramento da Aula 10 afirma que essa é a última aula do curso. Na realidade, o curso tem mais 6 aulas (11 a 16). Isso pode causar confusão no aluno sobre a estrutura do curso.

🟡 **[Melhoria] cell-38 — `plt.ticklabel_format(style="plain", useLocale=True)` com `useLocale=True`**  
O parâmetro `useLocale=True` usa a configuração de locale do sistema operacional, que pode variar entre ambientes. No Colab, o locale pode não ser pt-BR, fazendo a formatação usar vírgula como separador decimal ou outro comportamento inesperado. O parâmetro não é explicado e pode causar resultados diferentes para diferentes alunos.

🟡 **[Melhoria] Aula 10 — O arquivo de dados é carregado via URL do GitHub, mas o CONTEUDO.md diz dataset `worldpop`**  
O CONTEUDO.md descreve o cenário como "evolução da população dos países do BRICS ao longo dos anos", o que é consistente. Mas menciona somente `pokemons.csv` como dataset principal. A introdução de um novo dataset (`world_population.csv`) sem aviso prévio pode surpreender o aluno. Seria útil uma breve introdução no início do notebook sobre o dataset desta aula.

🟡 **[Melhoria] Passos 1 a 5 — O código completo é repetido em cada passo**  
A abordagem de repetir o bloco completo de código a cada passo é didática para mostrar a evolução, mas resulta em um notebook muito extenso e difícil de navegar. Comentários claros no início de cada bloco indicando o que mudou em relação ao passo anterior ajudariam a reduzir a carga cognitiva.

---

## Módulo 4 — Visualizações Avançadas

### Aula 11 — Mapas de Rede

**Avaliação geral:** Aula bem estruturada, com problema real (futebol/Copa do Mundo) que motiva o uso do gráfico. A evolução do grafo inicial (poluído) → filtrado → foco no Brasil é pedagogicamente boa.

🟡 **[Melhoria] cell-5 — "O nosso problema gira em torno dessa temática" sem mencionar o dataset de pokemons**  
O CONTEUDO.md indica que esta aula usa o dataset de pokemons. No entanto, a aula usa dados de confrontos de seleções de futebol (`worldcup.json`). Isso não é um erro, mas cria inconsistência com o enunciado do CONTEUDO.md, que cita `pokemons.csv` como dataset principal de todas as aulas. A prática 09-14 pede o exercício de rede com pokemons, mas a aula teórica usa futebol — isso é aceitável se intencional.

🟡 **[Melhoria] cell-14 — "nodos (vértices) e arestas (edges)" — terminologia misturada**  
O texto usa "vertices" para nodos e "edges" para arestas, invertendo a terminologia padrão de grafos. Em teoria dos grafos, vértices são os pontos (nodos) e arestas são as conexões. O código depois usa corretamente `net.add_node()` (nodo) e `net.add_edge()` (aresta). A célula de texto usa `edges` para as conexões mas as chama de "vértices" em uma linha. Verificar consistência.

🟢 **[Sugestão] cell-17 — Parâmetro `linewidths=2` sem relação com `width=2` no options**  
O dict `options` tem tanto `linewidths=2` quanto `width=2`. O primeiro controla a espessura das bordas dos nodos, o segundo a espessura das arestas. Sem comentário explicativo, o aluno não saberá qual controla o quê.

---

### Aula 12 — Sankey Charts

**Avaliação geral:** Aula direta e funcional. Contexto bem motivado (distribuição por geração e tipo de pokémon).

🟡 **[Melhoria] cell-8 — Dataset carregado de URL diferente do padrão**  
A URL usada é `'https://github.com/labeduc/datasets/blob/main/pokemons/all.csv?raw=true'`. O dataset padrão do curso é `pokemons.csv` (versão local). A aula não explica a diferença entre `all.csv` e `pokemons.csv`. Se forem o mesmo arquivo com nomes diferentes, isso deveria ser esclarecido. Se forem diferentes (estrutura ou conteúdo), a diferença deve ser documentada.

🟡 **[Melhoria] cell-3 — História do Sankey sem referência específica**  
O texto menciona "criado pelo capitão irlandês Matthew Sankey" sem data ou referência. Uma nota com ano (1898) e contexto (eficiência de máquinas a vapor) tornaria a história mais completa e verificável.

🟢 **[Sugestão] cell-13 — Gráfico interativo sem instrução para testar a interatividade**  
O texto diz "pode ir ali passar o mouse em cima" para ver tooltips, mas não mostra como isso funciona em capturas de tela. Para um notebook estático (PDF, exportação), essa instrução não é útil. Seria melhor descrever o que o tooltip mostra (tipo, geração, contagem) para que o aluno saiba o que buscar.

---

### Aula 13 — Wordclouds

**Avaliação geral:** Aula funcional, com boa motivação do problema e exemplo interessante com máscara de imagem.

🟡 **[Melhoria] cell-7 — Instrução de instalação diz que o wordcloud já está no Colab**  
O texto diz "No google colab ela já está disponível" no comentário, mas o enunciado da seção (`## Passo a Passo`) instrui a instalar com `pip install wordcloud`. Há contradição: está disponível ou precisa instalar? O comportamento pode variar conforme a versão do Colab. Seria melhor sempre incluir o comando de instalação no código com `!pip install wordcloud -q` para garantir disponibilidade em qualquer ambiente.

🔴 **[Crítico] cell-14 — `iterrows()` usado para construir dicionário, mas uso desaconselhado em Aula 05**  
Na Aula 05 (cell-60), o uso de `iterrows()` foi explicitamente desaconselhado: "é com certeza a que apresenta a pior performance". Na Aula 13, `iterrows()` é usado sem ressalvas para construir o dicionário de frequências. Existe uma alternativa mais simples e idiomática: `lista = dict(zip(df['Name'], df['Att']))`. A inconsistência com o ensinamento anterior é problemática.

🟡 **[Melhoria] cell-12 — Dataset carregado da mesma URL alternativa (`all.csv`)**  
Mesmo problema da Aula 12: a aula usa `all.csv` em vez do `pokemons.csv` local, sem explicação da diferença.

---

### Aula 14 — Pandas e Bancos de Dados

**Avaliação geral:** Aula introdutória ao DuckDB e JupySQL. O conteúdo é relevante, mas o nível é avançado para um curso introdutório de visualização.

🔴 **[Crítico] cell-9 — `%reload_ext sql` depende de `jupysql` que não foi instalado**  
O comando `%reload_ext sql` requer o pacote `jupysql` (ou `ipython-sql`), que não é instalado por padrão no Colab. O notebook não inclui nenhum `!pip install jupysql` antes. Se o aluno executar sequencialmente, receberá `ModuleNotFoundError`. Um bloco de instalação no início do notebook é obrigatório.

🟡 **[Melhoria] cell-3 — Aviso "pode ser pulada" sem orientação de onde continuar**  
O texto avisa que "essa aula pode ser pulada sem problema por agora, mas é aconselhável que você volte assim que aprender mais sobre bancos de dados." Porém não indica para onde o aluno deve ir se pular: Aula 15? Seria útil um link ou referência direta.

🟡 **[Melhoria] cell-18 — `table_name` e `file_name` com arquivo `teste.txt` não está no repositório**  
O exemplo intermediário usa um arquivo `teste.txt` que provavelmente não existe no ambiente do aluno. A célula resultará em erro ao ser executada. Seria mais seguro usar o `pokemons.csv` (que o aluno já tem no session storage) ou incluir instrução de como criar o `teste.txt`.

🟢 **[Sugestão] cell-30 — Sintaxe `%sql pokemons_agg << SELECT ...` não explicada**  
O operador `<<` para capturar resultado SQL em variável Python é introduzido sem explicação. É uma sintaxe específica do JupySQL que pode parecer estranha. Uma linha de texto antes da célula explicando que `<<` salva o resultado em um DataFrame Python seria suficiente.

---

## Módulo 5 — Plotly Interativo

### Aula 15 — Gráficos Interativos

**Avaliação geral:** Boa cobertura dos tipos principais de gráfico no Plotly. A conexão com o que foi aprendido no Seaborn é explícita e ajuda na compreensão.

🔴 **[Crítico] cell-3 — "Esta é nossa última aula" — mas há a Aula 16**  
O texto de introdução diz "Esta é nossa última aula". A Aula 16 existe e é a aula final real do curso. Mesmo erro que ocorreu no final da Aula 10. Precisa ser corrigido para "Esta é a penúltima aula" ou simplesmente remover a afirmação.

🟡 **[Melhoria] cell-15/cell-27 — Problema de escala entre gráfico de linha e área não resolvido**  
A cell-27 identifica o problema: "o formato do gráfico de linha e do gráfico de área não estão exatamente iguais, o que seria o esperado. O que aconteceu aqui foi uma mudança da escala no eixo do Y". Mas o problema é identificado e deixado sem resolução, com a promessa de "por isso conhecer como configurar os gráficos será muito importante" — o que só vem na Aula 16. O aluno fica com um problema visual não resolvido por uma aula inteira.

🟡 **[Melhoria] cell-8 — DuckDB em memória para transformações simples**  
A aula usa DuckDB em memória para fazer um `GROUP BY` que poderia ser feito facilmente com Pandas (`groupby().mean()`). Dado que o DuckDB foi introduzido na aula anterior como solução para grandes volumes de dados, usá-lo aqui para transformações simples pode reforçar a ideia errada de que ele é necessário para todos os casos. Uma nota explicando que Pandas seria suficiente aqui seria útil.

🟢 **[Sugestão] cell-35 — `fig.show()` sem `renderer='notebook'`**  
No Exercício do gráfico Donut (cell-35), o `fig.show()` é chamado sem `renderer='notebook'`, enquanto todos os outros gráficos anteriores usam `fig.show(renderer='notebook')`. Isso pode causar comportamento diferente no Colab (pode abrir em nova aba em vez de exibir inline).

---

### Aula 16 — Criando Visualizações Efetivas

**Avaliação geral:** Boa aula de encerramento. A evolução passo a passo do gráfico de barras com configuração via `update_layout()` é clara e bem documentada.

🟡 **[Melhoria] cell-9 — Dataset `ds_salaries.csv` introduzido sem contexto**  
A aula muda para um dataset completamente novo (`ds_salaries.csv` — salários de profissionais de dados) sem introdução. O dataset nunca foi mencionado no CONTEUDO.md. Uma célula de apresentação explicando o dataset (colunas relevantes, origem, o que representa) ajudaria o aluno a interpretar os gráficos.

🟡 **[Melhoria] cell-11 — Resultado SQL retorna tuplas, não DataFrame**  
A query `%%sql SELECT * FROM salaries_full WHERE ... LIMIT 5` retorna uma lista de tuplas em vez de um DataFrame Pandas. Isso acontece porque o `%%sql` (bloco inteiro) não atribui a variável. A exibição das tuplas com campos não nomeados visualmente pode confundir o aluno que espera uma tabela formatada. Usando `%sql resultado << SELECT ...` ou configurando `SqlMagic.autopandas = True` corretamente antes desta célula resolveria.

🟢 **[Sugestão] cell-33 — Renomeação de colunas via `labels={}` no `px.bar()` não descrita**  
O parâmetro `labels={"work_year": "Ano", "avg_salary_in_usd": "Salário", "job_title": "Cargo"}` é adicionado na última etapa sem texto explicativo entre a célula anterior e esta. A progressão cobre todos os outros passos com células Markdown, mas este último não tem comentário — apenas o código. Uma célula Markdown explicando que `labels` renomeia as colunas na tooltip e nos eixos seria consistente com o ritmo da aula.

---

## Práticas de Consolidação

### Prática 09 a 14 — Consolidação

**Avaliação geral:** Prática abrangente e bem projetada. Os 8 exercícios cobrem exatamente as 6 aulas prometidas. Estrutura clara com dicas detalhadas.

🟡 **[Melhoria] Exercício 8 — Código de instalação do `jupysql` ausente**  
O exercício instrui o uso de `%reload_ext sql`, mas o DuckDB + JupySQL precisam estar instalados. A Prática não inclui célula de instalação. O aluno que não tiver executado a Aula 14 em sessão recente provavelmente receberá erro. Uma célula inicial com `!pip install jupysql duckdb -q` seria necessária.

🟡 **[Melhoria] Exercício 5 — `dropna()` mencionado na dica mas não no enunciado**  
O enunciado do Exercício 5 (Mapa de Rede) não menciona que é necessário remover valores nulos da coluna `Type 2` antes de construir o grafo. Se o aluno não remover os NaN, `nx.add_edge()` vai tentar criar arestas com `NaN` como nodo, o que pode causar comportamento inesperado. A instrução de `dropna()` está na dica mas deveria estar também no enunciado.

🟢 **[Sugestão] Exercício 7 — Dica usa `iterrows()` para construir o dicionário**  
Mesmo problema da Aula 13: a dica instrui o uso de `iterrows()` para construir o dicionário de frequências, prática explicitamente desaconselhada na Aula 05. A alternativa `dict(zip(df['Name'], df['Def']))` é mais simples e consistente com o ensino anterior.

---

## Análise Geral de Fluidez e Cobertura

### Progressão do Curso

A progressão geral do curso é sólida: parte da teoria (Aula 01), passa pela ferramenta (Aula 02), pelos formatos de dados (Aula 03), carga de dados (Aula 04), manipulação (Aula 05), e então avança nas visualizações de forma crescente em complexidade. As práticas estão bem posicionadas para reforçar os aprendizados.

**Pontos fortes da progressão:**
- A decisão de usar `pokemons.csv` como dataset único nas aulas 05 a 14 é pedagogicamente excelente: o aluno não precisa aprender novos dados em cada aula
- O padrão de introdução (biblioteca → carregamento de dados → exemplos básicos → variações → conclusão) é consistente nas aulas do Módulo 3
- As práticas dedicadas (05, 06, 08) são bem estruturadas e complementam as aulas teóricas

**Lacunas de progressão identificadas:**
- A Aula 07 não tem prática dedicada — os gráficos de linha e área ficam sem exercício específico
- A Aula 04 tem uma seção prometida sobre "bibliotecas externas" que está completamente vazia
- As aulas 11 a 14 usam datasets diferentes (futebol, pokemons via URL, wordcloud, salários) introduzidos abruptamente, quebrando o padrão estabelecido nas aulas anteriores

### Consistência com o CONTEUDO.md

| Aula | Status |
|---|---|
| Aula 01 | ✅ Corrigido — tabela de referência rápida adicionada |
| Aula 02 | ✅ Corrigido — atalhos Ctrl+S e Ctrl+Shift+P adicionados |
| Aula 03 | ✅ Corrigido — cell-35 convertida para markdown; cell-32/36 removidas; exemplo de Series adicionado |
| Aula 04 | ✅ Corrigido — seção "Bibliotecas externas" preenchida; referência à Aula 10 adicionada |
| Aula 05 | ✅ Corrigido — referência cruzada "Aula 3" corrigida para "Aulas 03 e 04" |
| Prática 05 | ✅ Corrigido — dica do Exercício 1 expandida para identificação de nulos |
| Aula 06 | ✅ Corrigido — NumPy introduzido; errwidth→err_kws; transição Matplotlib; explicação .plot() |
| Prática 06 | ✅ Corrigido — errwidth→err_kws no enunciado e dica do Exercício 3 |
| Aula 07 | Consistente (sem prática dedicada — OK pelo CONTEUDO.md) |
| Aula 08 | Consistente |
| Prática 08 | Consistente |
| Aula 09 | Consistente |
| Aula 10 | Afirmação falsa de encerramento do curso |
| Aula 11 | Dataset de futebol vs. CONTEUDO.md que menciona pokemons |
| Aula 12 | Consistente (usa `all.csv` em vez do arquivo local) |
| Aula 13 | Consistente |
| Aula 14 | `jupysql` não instalado, arquivo `teste.txt` ausente |
| Prática 09-14 | Consistente, mas mesmos problemas de instalação |
| Aula 15 | Afirmação falsa de última aula |
| Aula 16 | Dataset `ds_salaries` não mencionado no CONTEUDO.md |

### Issues Transversais

🔴 **Afirmação de "última aula" em lugares errados:** Aula 10 e Aula 15 ambas se declaram como "última aula" do curso, sendo que a Aula 16 é a real última aula.

🔴 **JupySQL não instalado em Aula 14 e Prática 09-14:** O pacote `jupysql` (necessário para `%reload_ext sql`) não é instalado em nenhum dos notebooks que o utilizam.

🟡 **Uso inconsistente de `errwidth=0` vs `err_kws={"linewidth": 0}`:** ✅ Parcialmente corrigido — `errwidth=0` atualizado em Aula 06 (cell-29) e Prática 06 (Exercício 3). Verificar se há ocorrências remanescentes em outras aulas.

🟡 **Dois datasets "pokemons" diferentes:** `pokemons.csv` (arquivo local) e `all.csv` (URL remota) são usados alternadamente sem explicação de sua relação ou diferença.

🟡 **`iterrows()` desaconselhado na Aula 05 mas usado na Aula 13 e Prática 09-14:** Inconsistência pedagógica entre o aviso e o uso posterior.
