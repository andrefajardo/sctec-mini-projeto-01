# 📊 SalesInsight PY — Análise e Visualização de Dados de Vendas com Python

> **Projeto Avaliativo** | Módulo 01 - Semana 08  
> **Curso:** Desenvolvimento de IA para Análise Preditiva (Turma T3)  
> **Programa:** SCTEC / Governo de Santa Catarina  

---

## 🎯 Sobre o Projeto

O **SalesInsight PY** é uma solução em Python estruturada em Programação Orientada a Objetos (POO) e funções reutilizáveis, projetada para processar, tratar, analisar e visualizar históricos de vendas corporativas. 

O pipeline consome dados brutos (contendo ruídos, nulos e inconsistências de formatação), realiza um rigoroso processo de sanitização e transformação, calcula métricas de desempenho em múltiplas dimensões e exporta relatórios executivos (CSV/JSON) acompanhados de um painel de gráficos estatísticos em alta resolução (PNG).

---

## 📹 Vídeo de Demonstração

* **Link da Apresentação:** [Insira Aqui o Link do Seu Vídeo - Google Drive ou YouTube]  
*(O vídeo possui duração de até 5 minutos e aborda a execução completa do pipeline, organização das tarefas no Kanban, estrutura de branches do Git e justificativa das decisões técnicas de implementação).*

---

## 📋 Quadro de Organização (Kanban)

O planejamento e o fluxo de desenvolvimento do projeto foram gerenciados utilizando a metodologia Kanban:

* **Quadro Kanban (Link/Imagens):** [Insira Aqui o Link do Trello / GitHub Projects ou caminho da imagem]
* **Estrutura de Colunas:** `Backlog` | `A Fazer` | `Em Andamento` | `Concluído`

---

## 💡 O que o Projeto Analisa

* **Desempenho Temporal:** Evolução da receita total, volume de itens e número de transações agrupadas por Mês e Trimestre.
* **Métricas de Produto e Categoria:** Identificação dos *Top 5 Produtos* e das categorias que geram maior faturamento.
* **Análise Regional:** Comparativo de receita total e ticket médio acumulado por região geográfica.
* **Segmentação de Clientes:** Classificação da base em faixas de valor (*Bronze*, *Prata* e *Ouro*) com base no volume financeiro total consumido.
* **Relação Comercial:** Dispersão e correlação operacional entre quantidade de produtos por transação e a receita total gerada.

---

## 🧠 Conceitos Aplicados (Módulo 01 - Semanas 01 a 08)

O projeto consolida integralmente a grade curricular da primeira etapa da formação:

* **Lógica e Estruturas de Dados:** Variáveis, tipos nativos (`int`, `float`, `str`, `bool`), listas, dicionários e operadores lógicos/relacionais.
* **Funções e POO:** Funções com parâmetros, retornos e *docstrings*; lambdas; funções de ordem superior (`higher-order functions`); e encapsulamento em classe (`AnalisadorDeVendas` com `__init__`, `self` e métodos de instância).
* **Tratamento de Dados e Regex:** Manipulação de arquivos CSV/JSON (`json.dump`, `json.load`); processamento temporal (`datetime`); e limpeza e validação de padrões de texto via expressões regulares (`re.sub`, `re.compile`).
* **Manipulação com Pandas:** Leitura, inspeção estrutural (`shape`, `dtypes`, `isnull`), criação de colunas derivadas, transformação vetorizada e agregações avançadas com `groupby`, `agg` e `reset_index`.
* **Cálculo de Vetores com NumPy:** Vetorização pura, *broadcasting* (escalonamento 0–1), filtragem booleana e funções de agregação (`np.mean`, `np.std`, `np.sum`).
* **Visualização de Dados (Matplotlib & Seaborn):** Gráficos de linhas, barras, dispersão e painel *dashboard* em matriz de subplots ($2 \times 2$), com personalização de paleta, rótulos, títulos e exportação em 150 DPI.
* **Versionamento e GitFlow:** Estrutura de branches (`main`, `develop`, `feat/*`, `docs/*`) com commits semânticos (*Conventional Commits*).

---

## 🛠️ Estrutura do Repositório

```text
salesinsight-py/
├── salesinsight.py         # Código-fonte do pipeline principal e classe AnalisadorDeVendas
├── salesinsight.ipynb      # Notebook interativo para testes e exploração (opcional)
├── vendas.csv              # Dataset sintético de vendas (bruto com inconsistências)
├── README.md               # Documentação técnica do repositório
├── .gitignore              # Filtro de arquivos não versionados pelo Git
├── outputs/                # Artefatos e relatórios gerados pela aplicação
│   ├── metricas_por_mes.csv
│   ├── segmentacao_clientes.csv
│   ├── estatisticas_gerais.json
│   └── graficos/
│       ├── receita_por_mes.png
│       ├── top_produtos.png
│       ├── quantidade_vs_receita.png
│       └── painel_resumo.png
└── planejamento/           # Documentação de gestão e tarefas
    └── tarefas-kanban.md
