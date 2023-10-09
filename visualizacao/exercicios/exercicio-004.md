**Enunciado do Exercício**

---

**Decodificação de Campos Categóricos em um Dataset de Salários na Carreira de Ciência de Dados**

**Contexto:**
Você recebeu um dataset que contém informações sobre salários na carreira de Ciência de Dados. O dataset inclui várias características, como anos de experiência, grau de instrução, cidade, cargo, entre outros. Entretanto, você notou que muitos desses campos são categóricos e estão codificados, dificultando a compreensão imediata dos dados.

**Objetivo:**
O seu desafio é decodificar esses campos categóricos e transformá-los em uma representação mais amigável para análise.

**Instruções:**

1. **Análise Inicial:**
   - Carregue o dataset e realize uma análise exploratória inicial para identificar quais campos são categóricos e estão codificados.

2. **Decodificação:**
   Para os campos categóricos codificados, utilize o seguinte mapeamento:
   - **Nivel de Experiencia:** 
     * 'EN' -> 'Júnior'
     * 'MI' -> 'Pleno'
     * 'SE' -> 'Sênior'
     * 'EX' -> 'Executivo'
   - **Tipo de Emprego:** 
     * 'PT' -> '20 horas'
     * 'FT' -> '40 horas'
     * 'CT' -> 'Por Contrato'
     * 'FL' -> 'Free Lance'
   - **Estilo de Contratação:**
     * '0' -> 'Presencial'
     * '50' -> 'Híbrido'
     * '100' -> 'Remoto'
   - **Tamanho da Empresa:**
     * 'S' -> '0 - 50 Empregados'
     * 'M' -> '50 - 250 Empregados'
     * '100' -> '250+ Empregados'

3. **Análise Pós-Decodificação:**
   - Gere estatísticas descritivas para cada campo decodificado.
   - Crie visualizações (como gráficos de barras ou box plots) para entender a distribuição dos salários de acordo com os campos decodificados.

4. **Relatório:**
   - Escreva um breve relatório descrevendo suas observações e insights após a decodificação. Em particular, destaque padrões relacionados ao salário com base em diferentes categorias.

**Dicas:**
- Certifique-se de que após a decodificação, os dados permaneçam consistentes.
- Use bibliotecas como Pandas e Matplotlib ou Seaborn para manipulação e visualização de dados.

---

Ao concluir este exercício, você terá aprimorado suas habilidades em pré-processamento de dados e decodificação de campos categóricos, que são tarefas fundamentais em muitos projetos de ciência de dados.
