# 🔄 Projetos de ETL com Pandas

## 📌 Visão Geral
Este projeto apresenta exemplos de **ETL (Extract, Transform, Load)** desenvolvidos em Python utilizando a biblioteca **pandas**.  
O foco está na preparação e organização de dados para **análise, Business Intelligence e Data Science**.

Os projetos demonstram boas práticas de limpeza, transformação e estruturação de dados, sendo ideais para **portfólio profissional**.

---

## 🎯 Objetivos
- Extrair dados de múltiplas fontes
- Tratar dados brutos e inconsistentes
- Padronizar formatos e tipos de dados
- Criar variáveis derivadas e métricas
- Gerar datasets prontos para análise ou dashboards

---

## 🧩 Conceito de ETL
**ETL** é um processo composto por três etapas:

- **Extract:** leitura de dados (CSV, Excel, bancos, APIs)
- **Transform:** limpeza, padronização e enriquecimento
- **Load:** gravação dos dados tratados para uso final

---

## 🛠️ Tecnologias Utilizadas
- Python 3
- pandas
- numpy
- matplotlib / seaborn
- Jupyter Notebook

---

## 📂 Estrutura do Projeto

├── data/
│ ├── raw/ # Dados brutos
│ ├── processed/ # Dados tratados
│ └── output/ # Dados finais
├── notebooks/
│ └── etl_pipeline.ipynb
├── scripts/
│ └── etl_pipeline.py
├── README.md


---

## 🔹 Etapas do ETL

### 1️⃣ Extract – Extração
Leitura dos dados a partir de arquivos ou fontes externas.

```python
import pandas as pd

df = pd.read_csv("data/raw/dados.csv")
```

2️⃣ Transform – Transformação

Principais transformações realizadas:

Remoção de valores nulos e duplicados

Conversão de tipos de dados

Padronização de textos e datas

Criação de novas colunas

df = df.drop_duplicates()
df['data'] = pd.to_datetime(df['data'])
df['valor_total'] = df['quantidade'] * df['preco_unitario']


3️⃣ Load – Carga

Exportação dos dados tratados para uso final.

df.to_csv("data/output/dados_tratados.csv", index=False)


📊 Exemplos de Projetos ETL

ETL de dados financeiros

ETL de dados de vendas

ETL de dados operacionais

Preparação de dados para Power BI

---

🧪 Boas Práticas Aplicadas

Código modular e reutilizável

Funções separadas por etapa do ETL

Organização clara de diretórios

Validação de dados após transformações

---

👩‍💻 Autora

Projeto desenvolvido para prática e demonstração de habilidades em ETL, Análise de Dados e Python (pandas).
