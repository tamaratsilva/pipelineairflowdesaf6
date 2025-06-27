# Projeto de Pipeline de Dados - DNC

Este projeto simula um pipeline de dados com as camadas Bronze, Prata e Ouro usando Apache Airflow, pandas e Docker.

- Camada Bronze: dados brutos ingeridos.
- Camada Prata: dados limpos e enriquecidos com idade.
- Camada Ouro: agregação por faixa etária e status.

Todos os dados foram processados com base no arquivo `raw_data.csv.xlsx`.