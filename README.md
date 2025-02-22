## Introdução

Este notebook tem como objetivo realizar uma análise exploratória de dados (EDA) no dataset de uma loja fictícia e gerar insights significativos para o negócio. O case técnico é composto por três níveis:

1. Nível 1: Análise Exploratória (EDA) e Insights
2. Nível 2: Machine Learning Aplicado
3. Nível 3: Integração com IA Generativa

## Nível 1: Análise Exploratória (EDA) e Insights

### Objetivo
Realizar tratamento e preparação dos dados, análise exploratória com estatísticas descritivas relevantes, visualizações informativas e identificação de insights significativos sobre o negócio.

### Etapas
1. **Importação de bibliotecas**: Carregar as bibliotecas necessárias como pandas, matplotlib e seaborn.
2. **Carregamento do dataset**: Carregar o dataset `sample_superstore.csv`.
3. **Tratamento e preparação dos dados**: Converter colunas de data, verificar dados faltantes e criar novas features.
4. **Análise exploratória**: Estatísticas descritivas e visualizações de vendas ao longo do tempo e por categoria de produto.
5. **Identificação de insights**: Documentar 3-5 insights significativos sobre o negócio.

## Nível 2: Machine Learning Aplicado

### Objetivo
Desenvolver modelos de machine learning para prever vendas com base em variáveis como 'Profit', 'Quantity' e 'Discount'.

### Etapas
1. **Preparação dos dados**: Divisão em conjuntos de treinamento e teste.
2. **Treinamento de modelos**: Treinar modelos de Regressão Linear e Random Forest.
3. **Avaliação dos modelos**: Calcular métricas de performance como MAE, R² Score e RMSE.
4. **Comparação de modelos**: Comparar os desempenhos e identificar o modelo mais eficaz.

## Nível 3: Integração com IA Generativa

### Objetivo
Utilizar a API da OpenAI para gerar insights relevantes em linguagem natural com base nas métricas dos modelos de machine learning.

### Etapas
1. **Configuração da API**: Autenticação e configuração da API da OpenAI.
2. **Geração de insights**: Criação de prompts e chamadas à API para gerar insights.
3. **Documentação dos insights**: Coletar e documentar insights gerados pela IA.

## Instruções para Execução

### Requisitos

- Python 3.6 ou superior
- Bibliotecas Python: pandas, matplotlib, seaborn, openai, scikit-learn e numpy

### Instalação de Dependências

Para instalar as dependências, você pode usar o arquivo `requirements.txt`:

```bash
pip install -r requirements.txt
