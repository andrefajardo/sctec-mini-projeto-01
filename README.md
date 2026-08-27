# 📊 SalesInsight PY — Análise e Visualização de Dados de Vendas com Python

> **Projeto Avaliativo** | Módulo 01 - Semana 08  
> **Curso:** Desenvolvimento de IA para Análise Preditiva (Turma T3)  
> **Programa:** SCTEC / Governo de Santa Catarina  

---

## 🎯 Sobre o Projeto

O **SalesInsight PY** é uma solução em Python estruturada em Programação Orientada a Objetos (POO) e funções reutilizáveis, projetada para processar, tratar, analisar e visualizar históricos de vendas corporativas. 

O pipeline consome dados brutos (contendo ruídos, nulos e inconsistências de formatação), realiza um rigoroso processo de sanitização e transformação, calcula métricas de desempenho em múltiplas dimensões e exporta relatórios executivos (CSV/JSON) acompanhados de um painel de gráficos estatísticos em alta resolução (PNG).

A estrutura de diretórios foi construída manualmente, logo, para a fiel reprodução e operação da aplicação será necessário recriá-la conforme descrição (ilustração) no final deste arquivo.

---

## 📹 Vídeo de Demonstração

* 🎬 **Link da Apresentação:** [Clique aqui para o download do vídeo da apresentação](https://github.com/andrefajardo/sctec-mini-projeto-01/raw/refs/heads/main/planejamento/video_mini_projeto.mp4)  
*(O vídeo possui duração de até 5 minutos e aborda a execução completa do pipeline, organização das tarefas no Kanban, estrutura de branches do Git e justificativa das decisões técnicas de implementação).*

---

## 📋 Quadro de Organização (Kanban)

O planejamento e o fluxo de desenvolvimento do projeto foram gerenciados utilizando a metodologia Kanban:

* **Quadro Kanban (Link/Imagens):** [Link das imagens do Trello](https://github.com/andrefajardo/sctec-mini-projeto-01/tree/main/planejamento)
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
sctec-mini-projeto-01/
├── databases/                         # Scripts de geração e base de dados original
│   ├── sales_dataset_generator.ipynb  # Notebook gerador do dataset sintético
│   ├── sales_dataset_generator.py     # Módulo Python com a função de geração do dataset
│   └── vendas.csv                     # Dataset bruto de vendas
├── outputs/                           # Artefatos gerados pela aplicação
│   ├── graficos/                      # Visualizações e gráficos exportados
│   │   ├── distribuicao_vendas.png
│   │   ├── receita_por_categoria.png
│   │   ├── top_5_produtos.png
│   │   └── vendas_por_mes.png
│   ├── relatorio_final.json           # Relatório consolidado em formato JSON
│   └── vendas_processado.csv          # Base de dados limpa e tratada
├── planejamento/                      # Documentação de gestão, evidências e entregáveis
│   ├── Mini-Projeto Avaliativo.docx
│   ├── tela_trello_01.png
│   ├── tela_trello_02.png
│   ├── tela_trello_03.png
│   └── video_mini_projeto.mp4
├── salesinsight-py/                   # Notebooks e scripts do pipeline principal
│   └── salesinsight.ipynb             # Notebook interativo de análise e visualização
└── README.md                          # Documentação técnica do repositório
