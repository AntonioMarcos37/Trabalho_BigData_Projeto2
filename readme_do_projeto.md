# Trabalho Prático Individual — Tópicos de Big Data em Python

## Autor
* **Nome:** Antonio Marcos Silva de Oliveira
* **Matrícula:** 202402574302

## Objetivo
Construir um pequeno pipeline de dados reproduzível utilizando **Pandas** e **PySpark** para realizar a inspeção inicial, limpeza, tratamento de inconsistências, validação de regras de negócio, análise exploratória e consultas SQL sobre o dataset `vendas_bigdata_2026.csv`, gerando informações confiáveis para tomada de decisão no varejo.

## Tecnologias Utilizadas
* **Python 3.10+**
* **Pandas & NumPy:** Manipulação, limpeza e análise tabular.
* **Matplotlib & Seaborn:** Visualização de dados e geração de gráficos.
* **PySpark (DataFrames & Spark SQL):** Processamento distribuído e consultas SQL.
* **Scikit-Learn:** Boas práticas de pré-processamento e prevenção de vazamento de dados (Data Leakage) com `Pipeline`.

## Estrutura do Projeto
```text
Antonio_Marcos_Silvade_Oliveira_bigdata/
├── trabalho_bigdata.ipynb
├── README.md
└── resultado/
    └── resumo_regioes.csv
```

## Como Executar
1. Instale as dependências necessárias:
   ```bash
   pip install pandas numpy pyspark matplotlib seaborn scikit-learn jupyter
   ```
2. Certifique-se de que o arquivo `vendas_bigdata_2026.csv` esteja no mesmo diretório do notebook (`trabalho_bigdata.ipynb`).
3. Abra o Jupyter Notebook ou JupyterLab e execute todas as células do arquivo `trabalho_bigdata.ipynb` sequencialmente de cima para baixo.
4. O arquivo consolidado será gerado automaticamente em `resultado/resumo_regioes.csv`.

## Principais Conclusões
* **Liderança Regional:** A região **Sudeste** lidera o faturamento total e o volume de pedidos, seguida pelas regiões Sul e Nordeste.
* **Canais e Pagamentos:** O canal digital (**Site** e **App**) concentra a maior parte da receita, com predominância de pagamentos via **Pix** e **Cartão de Crédito**.
* **Qualidade de Dados:** A etapa de preparação corrigiu duplicatas, padronizou nomes de regiões com espaços e caixas divergentes, tratou datas inválidas e ajustou divergências financeiras conforme a regra de negócio, assegurando a rastreabilidade analítica de todo o pipeline.