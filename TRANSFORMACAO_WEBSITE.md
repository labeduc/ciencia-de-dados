# Transformando o curso em um website — análise e opções

## Contexto atual do repositório

- **63 notebooks Jupyter (.ipynb)** distribuídos em 5 módulos: `01_python`, `02_estatistica`, `03_visualizacao` (16 aulas + práticas, ~57 MB majoritariamente em imagens PNG geradas pelos gráficos), `04_banco_dados`, `05_dev_com_ai`.
- Cada módulo tem `CONTEUDO.md` e `PLANO_DE_AULA.md` como metadados de curso.
- Estilo editorial já é consistente e "parametrizável": abertura padrão ("Olá Cientista de Dados!"), fechamento padrão, blockquotes de dica/atenção/nota (`> 💡 **Dica:**` etc.), títulos no padrão `# Aula NN - Tema`.
- Hoje o conteúdo só é consumível clonando o repo e abrindo os `.ipynb` (Jupyter, Colab, VS Code).
- Existe material antigo (`99_material-antigo/`) em Markdown puro — provavelmente não deve entrar no site novo.

Esse contexto pesa a favor de qualquer solução que **renderize `.ipynb` diretamente**, sem exigir reescrever o conteúdo em outro formato.

## Critérios usados para comparar as opções

1. **Esforço de migração** — dá pra publicar o que já existe sem reescrever tudo?
2. **Fidelidade ao notebook** — código, saída e gráficos aparecem bem?
3. **Navegação multi-módulo** — sumário/sidebar a partir da estrutura de pastas atual.
4. **Custo/hospedagem** — idealmente gratuito (GitHub Pages).
5. **Fluxo de autoria contínuo** — o Walter continua editando `.ipynb` no dia a dia?

---

## Opção 1 — Quarto (recomendada)

Framework de publicação da Posit (ex-RStudio), renderiza `.ipynb` e `.qmd` nativamente para HTML, com temas Bootstrap prontos, busca embutida, callouts (`:::tip`), suporte a LaTeX/matplotlib/plotly sem configuração extra.

**Prós**
- Lê os notebooks como estão; não precisa reescrever conteúdo.
- Callouts do Quarto mapeiam quase 1:1 com os blockquotes de Dica/Atenção/Nota já usados.
- Gera "book" (sumário lateral por módulo/aula) ou "website" simples — se encaixa bem em 5 módulos com N aulas cada.
- Deploy gratuito via GitHub Actions → GitHub Pages (workflow oficial pronto).
- Também exporta para slides/PDF a partir da mesma fonte, caso um dia queira slides de aula.

**Contras**
- Precisa instalar o CLI do Quarto no ambiente de build (não é só pip).
- Exige um arquivo `_quarto.yml` mapeando a navegação — trabalho único, mas manual para 60+ arquivos (pode ser scriptado).
- Por padrão executa os notebooks no build; se algum notebook depender de dados externos/API, é preciso configurar `execute: freeze: auto` para usar os outputs já salvos.

**Esforço estimado:** baixo–médio (1 `_quarto.yml`, ajustar front-matter YAML em cada notebook ou gerar via script, 1 Action de deploy).

---

## Opção 2 — Jupyter Book (MyST)

Ferramenta focada especificamente em transformar coleções de notebooks em um "livro" navegável — foi desenhada exatamente para o caso de uso deste repositório (curso em notebooks).

**Prós**
- Setup mais simples que Quarto para quem só quer "pasta de notebooks → site de curso".
- `_toc.yml` define a ordem dos capítulos/aulas de forma direta.
- Admonitions nativas (`{tip}`, `{warning}`, `{note}`) — mesmo espírito dos blockquotes atuais.
- Deploy padrão para GitHub Pages via Action oficial (`jupyter-book build` + `ghp-import`).

**Contras**
- Tema visual mais engessado (Sphinx por baixo dos panos) — menos flexível para uma "cara" de produto/marca própria.
- Jupyter Book 1 está em manutenção; a v2 (baseada em MyST) ainda está amadurecendo — vale checar o estado atual antes de comprometer.
- Menos indicado se um dia quiser página de vendas/landing page bonita junto do conteúdo técnico.

**Esforço estimado:** baixo (ferramenta praticamente pronta para este formato de conteúdo).

---

## Opção 3 — MkDocs Material + plugin `mkdocs-jupyter`

Gerador de site de documentação com o tema Material (o mesmo usado por muitos projetos open source), com plugin que renderiza notebooks inline.

**Prós**
- Visual mais "produto" (Material Design), muito polido, com busca full-text ótima out-of-the-box.
- Ecossistema grande de plugins (blog, versionamento com `mike`, i18n, etc.) — útil se o curso crescer para ter blog/anúncios além das aulas.
- Navegação configurada em YAML simples (`mkdocs.yml`), com plugin `awesome-pages` para evitar listar manualmente todos os arquivos.

**Contras**
- Não executa os notebooks por padrão — precisa garantir que os outputs (gráficos) já estejam salvos nos `.ipynb` commitados, ou rodar `nbconvert --execute` antes do build.
- Menos "nativo" para notebooks do que as duas opções acima — é uma ferramenta de docs adaptada, não construída para isso.

**Esforço estimado:** médio (config do `mkdocs.yml`, garantir outputs salvos, eventualmente customizar CSS para a identidade "LabEduc").

---

## Alternativa fora do código: plataforma de LMS pronta

Se o objetivo do "LabEduc" for também vender/matricular alunos, controlar progresso, emitir certificado etc. (não só publicar o conteúdo), vale considerar que nenhuma das opções acima resolve isso — são geradores de site estático de conteúdo. Nesse caso, ferramentas como Hotmart, Teachable ou um LMS (ex.: Moodle) resolveriam a parte de negócio, e o conteúdo Quarto/Jupyter Book poderia ser incorporado via iframe ou exportado como PDF/HTML para dentro dela. Vale confirmar com o Walter se o objetivo é **divulgação do conteúdo** ou **produto comercial completo** antes de escolher.

---

## Comparativo rápido

| Critério | Quarto | Jupyter Book | MkDocs Material |
|---|---|---|---|
| Renderiza `.ipynb` direto | ✅ | ✅ | ✅ (via plugin) |
| Executa notebooks no build | ✅ (configurável) | ✅ | ❌ (usa outputs salvos) |
| Visual/tema customizável | Médio-alto | Baixo | Alto |
| Esforço de setup inicial | Médio | Baixo | Médio |
| Deploy GitHub Pages gratuito | ✅ | ✅ | ✅ |
| Maturidade/comunidade | Alta (Posit) | Alta, mas v2 em transição | Muito alta |

## Recomendação

**Quarto** é o melhor equilíbrio para este repositório: absorve os notebooks como estão, tem visual mais profissional que Jupyter Book, e mantém o fluxo de autoria atual (continuar editando `.ipynb`). **Jupyter Book** é a alternativa mais rápida de configurar se a prioridade for velocidade e não a estética. MkDocs Material entra em jogo se o plano for evoluir para algo mais parecido com um "produto" com blog/marca própria além do conteúdo das aulas.

## Próximos passos sugeridos

1. Decidir entre Quarto e Jupyter Book (ou confirmar interesse em algo mais "produto" via MkDocs).
2. Criar o arquivo de navegação (`_quarto.yml` ou `_toc.yml`) mapeando os 5 módulos e suas aulas.
3. Decidir se `99_material-antigo/` entra no site novo ou fica só como arquivo morto no repo.
4. Configurar GitHub Action de build + deploy para GitHub Pages.
5. Definir se os notebooks serão executados no build (outputs sempre atualizados) ou publicados com os outputs já salvos (mais rápido, sem dependência de dados externos).
