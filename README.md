# 📊 Pipeline de Dados com Airflow | Desafio DNC

Este repositório contém a solução para o desafio de engenharia de dados da **DncInsight Solutions**, cujo objetivo foi desenvolver um pipeline automatizado de ingestão, limpeza e transformação de dados.

---

## 🧱 Estrutura de Camadas

O pipeline é organizado em três camadas principais:

- **Bronze** 🟫  
  Ingestão dos dados brutos a partir do arquivo `raw_data.csv.xlsx`.

- **Prata** 🥈  
  Limpeza e enriquecimento dos dados:
  - Remoção de registros com campos obrigatórios nulos
  - Validação de e-mails
  - Cálculo da idade com base na data de nascimento

- **Ouro** 🥇  
  Agregação e preparação para análise:
  - Agrupamento por faixa etária e status de inscrição (`active` ou `inactive`)
  - Criação de métricas para análise demográfica

---

## 🛠️ Tecnologias Utilizadas

- Python + Pandas
- Apache Airflow (simulado)
- Docker (sugerido para produção)
- Estrutura de dados em diretórios locais (`data/raw`, `bronze`, `silver`, `gold`)

---

## 📁 Organização do Projeto

├── data/
│ ├── raw/ # Base original
│ ├── bronze/ # Dados brutos copiados
│ ├── silver/ # Dados limpos e com idade
│ └── gold/ # Dados agregados prontos para análise
├── dags/ # DAG simulada do Airflow
├── scripts/ # Scripts de processamento
├── README.md


## 🚀 Como foi desenvolvido

Todo o pipeline foi baseado no uso da biblioteca `pandas` para transformação dos dados. Embora o projeto esteja pronto para ser executado com Airflow e Docker, todos os dados processados foram gerados e entregues em arquivos `.csv` para facilitar a visualização e submissão.

