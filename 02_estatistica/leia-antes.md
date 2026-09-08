# 🌅 Uma Tardezinha na Beira do Guaíba
### Estatística e Análise de Dados contadas como uma história

Material para jovens do ensino médio que querem aprender estatística e análise de dados de um jeito prático, sem fórmula assustadora logo de cara — usando uma história de um passeio na orla do Guaíba pra ensinar os conceitos.

## 📂 O que tem aqui

| Arquivo | O que é |
|---|---|
| `material_teorico.md` | A história completa, em texto, com todas as explicações teóricas e diagramas ilustrativos. Ideal pra ler primeiro, ou pra estudar sem precisar rodar código. |
| `curso_estatistica_guaiba.ipynb` | O notebook interativo (Jupyter/Google Colab). A mesma história, mas com código pra rodar, gráficos gerados na hora e exercícios práticos. |
| `dados/cafe.csv` | Base real de pesquisa com o tipo de café preferido por 43 pessoas. Usado nos capítulos de frequência e amostragem. |
| `dados/combustivel.csv` | Histórico real de 65 abastecimentos de um carro, usado no estudo de caso de análise de dados (distância, litros, valor). |
| `images/` | Diagramas e gráficos usados no `material_teorico.md` (população/amostra, frequência, medidas de posição, tipos de gráfico, desvio padrão, correlação/regressão e o estudo de caso do combustível). |

## 🚀 Como abrir no Google Colab

**Link direto (já configurado para este repositório):**

👉 [Abrir no Google Colab](https://colab.research.google.com/github/labeduc/ciencia-de-dados/blob/main/02_estatistica/curso_estatistica_guaiba.ipynb)

Ou, manualmente:
1. Acesse [colab.research.google.com](https://colab.research.google.com/).
2. Clique em **Arquivo → Abrir notebook → GitHub**.
3. Cole `labeduc/ciencia-de-dados` na busca, escolha a branch `main` e abra `02_estatistica/curso_estatistica_guaiba.ipynb`.

**Importante:** antes de rodar as células que leem os arquivos `dados/cafe.csv` e `dados/combustivel.csv`, você precisa deixá-los acessíveis pro Colab. Duas formas simples:
- **Opção A (mais fácil):** no Colab, clique no ícone de pasta 📁 na barra lateral esquerda, depois no ícone de upload, e envie os dois arquivos da pasta `dados/` do seu computador.
- **Opção B (clonando o repositório, sem precisar fazer upload manual):** adicione uma célula no topo do notebook com:
  ```python
  !git clone https://github.com/labeduc/ciencia-de-dados.git
  %cd ciencia-de-dados/02_estatistica
  ```
  Depois disso, as células que leem `dados/cafe.csv` e `dados/combustivel.csv` funcionam direto, sem precisar fazer upload manual.

## 📖 Como usar este material

1. Leia (ou vá lendo aos poucos) o `material_teorico.md` — ele te dá o contexto da história e as explicações completas de cada conceito.
2. Abra o notebook e vá rodando célula por célula, na ordem, testando os números, mudando valores e observando o que muda.
3. No final, use o "esqueleto de código" do último capítulo pra fazer sua própria mini análise, com dados do seu dia a dia.

## 🎓 Conceitos cobertos

População e amostra • organização de dados em tabelas (série/observação) • frequência absoluta, relativa e acumulada • moda, média, mediana, mínimo e máximo • desvio padrão e variância • correlação (e correlação espúria) • regressão linear, interpolação e extrapolação • análise quantitativa e qualitativa • metodologia de análise de dados em 6 passos • gráficos de barras, pizza, pontos, linha e histograma.

## 🙌 Baseado em

Este material é uma reformulação, com nova história e narrativa, do curso "Introdução à Estatística para Ciência de Dados" e "Análise de Dados", reaproveitando conceitos e dados reais (café e combustível) usados originalmente em aula.
