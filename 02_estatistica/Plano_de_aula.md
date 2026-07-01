# Plano de Aula: Curso de Estatística e Análise de Dados

Este repositório contém o planeamento estruturado para o curso de **Estatística Básica e Análise de Dados**, focado na recolha, organização, cálculo descritivo e interpretação analítica de grandes volumes de informação utilizando folhas de cálculo.

---

## 📅 Estrutura Geral do Curso

| Módulo | Conteúdo Principal | Foco Prático |
| :--- | :--- | :--- |
| **1** | Introdução, Recolha e Organização | Estruturação de tabelas e amostragem |
| **2** | Medidas de Tendência Central e Frequências | Cálculos descritivos e fórmulas em planilhas |
| **3** | Ordenação de Dados e Mediana | Análise de impacto e robustez contra outliers |
| **4** | Análise Avançada, Correlação e Projeções | Dispersão, covariância e séries temporais |

---

## 📖 Detalhe dos Módulos

### Módulo 1: Introdução, Recolha e Organização de Dados
* **Objetivos:** Compreender os conceitos fundamentais de estatística; aprender a recolher e estruturar massas de dados; identificar variáveis de referência.
* **Conteúdos Programáticos:**
  * Definição de Estatística, População e Amostra.
  * A importância do tamanho da amostra para representar fielmente uma população.
  * Organização de dados em tabelas: estruturação em linhas (elementos) e colunas (categorias/variáveis).
  * Técnicas de ordenamento (ex: por data) e agrupamento por variáveis para a criação de subconjuntos analíticos.
* **Metodologia / Atividades Práticas:**
  * **Análise de Cenário:** Reflexão sobre a organização financeira pessoal ao longo de um ano (365 dias) e escolha do tamanho amostral adequado.
  * **Exercício de Construção:** Criação de uma tabela de dados com categorias predefinidas e subsequente ordenação/agrupamento justificando o critério analítico escolhido.

### Módulo 2: Medidas de Tendência Central e Frequências
* **Objetivos:** Calcular e identificar informações essenciais em conjuntos de dados; preencher dados em falta; aplicar fórmulas de estatística descritiva em planilhas.
* **Conteúdos Programáticos:**
  * Conceito de Mínimo (`MÍN`) e Máximo (`MÁX`) num conjunto de dados (amplitude primária).
  * Média aritmética (`MÉDIA`): cálculo da posição central (soma dos valores dividida pelo número de itens).
  * Frequência Absoluta (número de ocorrências) e Frequência Relativa (percentagem do total).
  * Moda (`MODO`): identificação do valor com maior recorrência.
  * Frequência Acumulada: soma consecutiva das frequências para análise de impacto progressivo.
* **Metodologia / Atividades Práticas (Google Planilhas / Excel):**
  * **Atividade Prática 1 (Equipa de Voleibol):** Utilização de funções estatísticas para extrair o mais baixo, o mais alto, a média de idades e as modas de tamanhos de vestuário de um grupo.
  * **Atividade Prática 2 (Consumo de Combustível):** Importação de ficheiros CSV para calcular médias de despesas mensais e identificar extremos (maior e menor gasto).
  * **Atividade Prática 3 (Análise Amostral):** Avaliação da variação da frequência relativa à medida que a amostra cresce.

### Módulo 3: Ordenação de Dados e a Mediana
* **Objetivos:** Compreender o impacto do ordenamento na análise de dados; calcular e interpretar a mediana como medida robusta de tendência central.
* **Conteúdos Programáticos:**
  * O conceito de Mediana (`MED`) como o valor que divide o conjunto de dados exatamente ao meio (50% dos dados abaixo, 50% acima).
  * A importância do ordenamento prévio (rol de dados) para o cálculo da mediana.
  * Regras de cálculo para conjuntos de dados com número ímpar de elementos (valor estritamente central).
  * Regras de cálculo para conjuntos de dados com número par de elementos (média aritmética dos dois valores centrais).
  * **Comparação analítica:** Quando utilizar a Média versus quando utilizar a Mediana (sensibilidade a valores discrepantes/*outliers*).
* **Metodologia / Atividades Práticas:**
  * **Estudo de Caso:** Análise do impacto de valores extremos (*outliers*) em um conjunto de salários ou despesas, comparando como a média e a mediana reagem a esses dados discrepantes.
  * **Laboratório de Dados:** Resolução prática de exercícios de cálculo de mediana utilizando conjuntos de dados pares e ímpares extraídos das atividades anteriores.

### Módulo 4: Análise Avançada, Correlação e Projeções
* **Objetivos:** Analisar criticamente distribuições de dados; identificar relações matemáticas entre variáveis; projetar valores futuros ou intermediários com segurança.
* **Conteúdos Programáticos:**
  * **Desvio Padrão e Variância:** Introdução ao conceito de dispersão de dados em torno da média e a sua aplicação prática na deteção de anomalias/fraudes (*Machine Learning*).
  * **Correlação:** Relação matemática entre duas variáveis (Covariância).
    * Coeficiente próximo de `1`: linearidade direta (ambas crescem ou decrescem juntas).
    * Coeficiente próximo de `-1`: linearidade inversa (uma cresce enquanto a outra decresce).
    * **Correlação Espúria:** Situações onde há forte relação matemática, mas nenhuma ligação lógica/causal entre as variáveis.
  * **Interpolação vs. Extrapolação:**
    * *Interpolação:* Estimar valores intermédios dentro de um grupo limitado de dados conhecidos.
    * *Extrapolação:* Assumir que a tendência matemática se manterá para além dos limites conhecidos (alertando para o risco de gerar valores absurdos/inadequados a longo prazo).
* **Metodologia / Atividades Práticas:**
  * **Estudo de Caso Financeiro e Consumo:** Análise de matrizes de dados para verificar se existe correlação entre preços de diferentes combustíveis (álcool vs. gasolina) e o rendimento por quilometragem.
  * **Exercício de Projeção:** Aplicação de conceitos de interpolação e extrapolação baseados em séries temporais de despesas para prever orçamentos futuros.

---

## 🛠️ Recursos Sugeridos para o Professor

* **Software:** Ferramentas digitais de cálculo (Google Planilhas ou Microsoft Excel).
* **Plataforma Interativa:** [Seeing Theory (Brown University)](https://seeing-theory.brown.edu/) para exploração visual e conceitual de dispersão, variância e correlação.
