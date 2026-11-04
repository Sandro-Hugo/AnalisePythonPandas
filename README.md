# Análise e Tratamento de Dados de Funcionários com Python & Pandas

Este repositório contém um notebook em Python dedicado ao estudo prático e demonstração de técnicas essenciais de **Data Cleaning** (Limpeza de Dados) e **Análise Exploratória de Dados (EDA)** utilizando a biblioteca **Pandas**.

O projeto simula um cenário real de RH/Financeiro, abordando desde a criação e manipulação de estruturas de dados até o tratamento avançado de valores nulos e agregações departamentais.

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Pandas** (Manipulação e Análise de Dados)
- **NumPy** (Apoio a operações numéricas e valores nulos)
- **Jupyter Notebook** (Ambiente de desenvolvimento)

---

## 📌 Principais Funcionalidades e Conceitos Aplicados

### 1. Geração de Dados Sintéticos e Exportação
- Criação de conjuntos de dados parametrizados (`Series` e `DataFrame`) com 100 registros.
- Exportação e leitura de ficheiros no formato `CSV`.

### 2. Transformação e Engenharia de Atributos
- Seleção e filtragem pontual de colunas.
- Operações vetorizadas para criação de métricas calculadas (ex.: projeção de `Salario_Anual`).
- Ordenação de dados por múltiplos critérios (`sort_values`).

### 3. Filtragem Booleana Avançada
- Aplicação de máscaras lógicas complexas com operadores `&` (AND), `|` (OR) e `~` (NOT).
- Segmentação de colaboradores por faixa etária, salário e status ativo.

### 4. Agrupamento e Agregação Estatística
- Distribuição de frequências relativas e absolutas (`value_counts`).
- Agrupamento multinível (`groupby`).
- Aplicação de *Named Aggregation* (`.agg()`) para calcular métricas departamentais:
  - Total de funcionários por setor;
  - Idade média (com arredondamento);
  - Salário mínimo e máximo por departamento.

### 5. Tratamento de Dados Ausentes (*Data Cleaning*)
- Identificação de valores `NaN` / `None`.
- Imputação estatística de dados nulos utilizando a média da amostra (`fillna`).
- Conversão explícita de tipos de dados (`astype(int)`).
- Remoção estratégica de linhas incompletas com `dropna`.

---

## 📁 Estrutura do Repositório

```text
.
├── pandas.ipynb                        # Jupyter Notebook principal com o código e análises
├── dados_funcionarios.csv              # Dataset sintético completo gerado durante a execução
├── dados_funcionarios_com_nulos.csv    # Dataset com valores nulos para testes de limpeza
└── README.md                           # Documentação do projeto
