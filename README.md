# Projeto Telecom X - Análise e Previsão de Churn

Este projeto tem como objetivo analisar o comportamento dos clientes da empresa de telecomunicações Telecom X e criar modelos preditivos para prever a evasão (churn) de clientes.

## Conteúdo do Projeto

* Limpeza e tratamento dos dados
* Análise exploratória
* Visualização de correlações
* Análise de variáveis que influenciam a evasão
* Criação de modelos preditivos
* Avaliação e comparação de modelos
* Conclusões e estratégias de retenção

## Tecnologias e Bibliotecas Utilizadas

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## Instalação

Para instalar as dependências do projeto, utilize:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Estrutura do Projeto

```
├── telecomx_tratado.csv        # CSV com dados tratados e limpos
├── notebooks/
│   ├── desafio_parte1.ipynb    # Notebook da primeira parte: limpeza e análise exploratória
│   ├── desafio_parte2.ipynb    # Notebook da segunda parte: modelagem preditiva
└── README.md                   # Este arquivo
```

## Uso

1. Carregar o arquivo CSV com os dados tratados:

```python
import pandas as pd

# URL do CSV raw no GitHub
url = 'https://raw.githubusercontent.com/ThPontes/telecom-x-parte2/refs/heads/main/telecomx_tratado.csv'
df = pd.read_csv(url, sep=';')
```

2. Explorar os dados e realizar análises descritivas.

3. Aplicar técnicas de visualização, como boxplots, scatter plots e matrizes de correlação.

4. Preparar os dados para modelos de machine learning:

   * Conversão de variáveis categóricas em formato numérico (one-hot encoding)
   * Balanceamento de classes (SMOTE ou oversampling)
   * Normalização ou padronização, caso o modelo utilize métricas baseadas em distância

5. Criar e treinar modelos preditivos, como:

   * Decision Tree
   * K-Nearest Neighbors (KNN)
   * Random Forest (opcional)
   * Regressão Logística (opcional)

6. Avaliar os modelos com métricas como:

   * Acurácia
   * Precisão
   * Recall
   * F1-score
   * Matriz de confusão

7. Analisar a importância das variáveis e identificar fatores mais relevantes para a evasão de clientes.

## Principais Resultados

* Proporção de evasão: aproximadamente 25% dos clientes saíram.
* Fatores mais impactantes no churn: tipo de contrato, tempo de contrato, faturamento mensal, quantidade de serviços contratados.
* Modelos de árvore (Decision Tree) e KNN apresentaram desempenho semelhante, com acurácia entre 72% e 77%.
* Insights para retenção de clientes:

  * Focar em clientes com contratos Month-to-Month e alto faturamento diário.
  * Oferecer pacotes combinados de serviços para reduzir churn.
  * Incentivar métodos de pagamento automáticos e fatura sem papel.

## Conclusão

Este projeto fornece uma base sólida para prever a evasão de clientes e apoiar decisões estratégicas de retenção, além de demonstrar boas práticas em análise de dados e modelagem preditiva.

## Contato

Desenvolvedor: Thiago Pontes
GitHub: [https://github.com/ThPontes](https://github.com/ThPontes)
