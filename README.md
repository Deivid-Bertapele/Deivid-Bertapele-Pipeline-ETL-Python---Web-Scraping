# 🚀 Pipeline ETL - Mercado Livre Notebooks Analysis

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

Um pipeline ETL completo para análise de notebooks no Mercado Livre, incluindo coleta de dados, transformação e visualização.

## 📋 Índice

- [Visão Geral](#-visão-geral)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias](#-tecnologias)
- [Instalação](#-instalação)
- [Uso](#-uso)
- [Estrutura do Projeto](#-estrutura-do-projeto)


## 🌟 Visão Geral

Este projeto implementa um pipeline ETL (Extract, Transform, Load) para coletar, processar e analisar dados de notebooks disponíveis no Mercado Livre. O pipeline inclui:

- Coleta de dados usando Scrapy
- Transformação e limpeza dos dados
- Armazenamento em banco de dados SQLite
- Visualização interativa com Streamlit

## ✨ Funcionalidades

- **Coleta de Dados**: Extração automática de informações de notebooks
- **Dashboard Interativo**: Visualização de KPIs e análises
- **Análise de Preços**: Comparação de preços por marca
- **Avaliação de Satisfação**: Análise de reviews e ratings
- **Filtros Inteligentes**: Filtragem de produtos por faixa de preço
- **Análise Exploratória**: Detalhes com insights e visualizações

## 🛠️ Tecnologias

- **Python 3.8+**
- **Pandas**: Processamento e análise de dados
- **Scrapy**: Web scraping
- **Streamlit**: Interface de visualização
- **SQLite**: Armazenamento de dados
- **Jupyter Notebook**: Análise exploratória de dados
- **Matplotlib/Seaborn**: Visualização de dados

## 📥 Instalação

1. Clone o repositório:
```bash
git clone [URL_DO_REPOSITÓRIO]
cd PIPELINE_ETL_PYTHON_SCRAPY
```

2. Crie e ative um ambiente virtual:
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

## 🚀 Uso

1. Execute o spider para coletar dados:
```bash
cd src/notebooks
scrapy crawl notebooks -O data/data.jsonl
```

2. Execute o pipeline ETL:
```bash
python src/transformLoad/main.py
```

3. Inicie o dashboard:
```bash
streamlit run src/dashboards/app.py
```

## 📁 Estrutura do Projeto

```
PIPELINE_ETL_PYTHON_SCRAPY/
├── data/                  # Dados coletados e processados
├── src/
│   ├── dashboards/       # Aplicação Streamlit
│   ├── notebooks/        # Notebooks de análise e spiders
│   └── transformLoad/    # Scripts de transformação
├── requirements.txt      # Dependências do projeto
└── README.md            # Documentação
```
------

![scrpay01](https://github.com/user-attachments/assets/f65fc04d-8130-43e8-a6d0-f2f4f96aae10)

![scrpay02](https://github.com/user-attachments/assets/4e19721d-a9cd-4b95-9542-db6f335ab937)



