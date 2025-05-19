# Olist E-commerce Data Project

**Teste Técnico - Programa Trainee triggo.ai de Excelência em Engenharia de Dados e DataOps 2025.**

## 📌 Objetivo

Analisar o conjunto de dados históricos de vendas de uma empresa brasileira de e-commerce (Olist) para extrair insights relevantes e resolver desafios de negócio com foco em Engenharia de Dados.

## ⚙️ Tecnologias Utilizadas

- **Linguagens:** SQL / Python  
- **Ambiente:** Jupyter Notebook  
- **Bibliotecas:**  
    ```bash
    !pip install pandas matplotlib seaborn haversine
    ```

## 🎲 Dataset Utilizado 

Foi utilizado o dataset o **Brazilian E-commerce Public Dataset by Olist** disponível no Kaggle. Este dataset contém informações sobre aproximadamente 100 mil pedidos realizados entre 2016 e 2018, incluindo dados de clientes, produtos, vendedores, entregas e avaliações.

- [Olist Brazilian E-commerce Dataset - Kaggle]( https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## 🗃️ Etapas do Projeto

- Preparação dos Dados 
    - Leitura e tratamento dos dados
    - Modelagem e integração dos dados 

- Análise Exploratória de Dados e Visualizações
    - Volume de pedidos, sazonalidade, tempo de entrega, relação entre frete e distância, categorias com maior faturamento e estados com maior ticket médio
    - Criação de gráficos para facilitar a interpretação dos dados 

## 📁 Estrutura do Projeto 
```bash
    .
    ├── data/ #-> Dados brutos Olist
    │   ├── olist_customers_dataset.csv
    │   └── ...
    ├── image
    │   └── modelagem.png
    ├──  olist_ecommerce.ipynb
    ├── requirements.txt #-> Bibliotecas utilizadas 
    └── README.md
```

## 🚀 Como Executar
1. Clone o repositório: ```git clone https://github.com/livalves/Olist-ecommerce-data-project.git```
2. Instale as bibliotecas necessárias ```pip install -r requirements.txt```
3. Acesse o arquivo principal: ```olist_ecommerce.ipynb``` 


# 📊 Concluindo análises

- **Volume de Pedidos por Mês:** 
    Observa-se um aumento no volume de pedidos entre os meses de outubro e dezembro, indicando uma tendência sazonal nas vendas. Esse padrão está alinhado com datas comemorativas e eventos promocionais, como a Black Friday e o Natal.

- **Tempo de entrega dos pedidos:**
    A maioria dos pedidos é entregue entre 5 e 15 dias. Há casos isolados de entregas que ultrapassam esse intervalo, indicando variações pontuais no processo logístico.

- **Valor do frete x Distância:**
    Existe uma correlação positiva moderada (coeficiente de 0,39) entre a distância de entrega e o valor do frete. Isso sugere que, em geral, o frete tende a aumentar com a distância percorrida. No entanto, outros fatores, como peso e dimensões do produto, também influenciam significativamente o custo do frete.

- **Categorias dos produtos mais vendidos:**
    - Beleza e Saúde
    - Relógios e Presentes
    - Cama, Mesa e Banho

- **Estados com maior com maiores médias de pedidos:**
    Os estados brasileiros que possuem o maior valor médio de pedidos são: a Paraíba, Acre e Rondônia. É possível observar que os estados do norte e nordeste possuem um valor médio mais alto em relação a outras regiões.
