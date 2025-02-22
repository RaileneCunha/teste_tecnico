## Teste Prático
Este repositório contém a solução para de um case técnico. O projeto é dividido em três notebooks, cada um correspondendo a uma etapa do processo de análise de dados, modelagem de machine learning e geração de insights com IA generativa.

### 1. Estrutura do Projeto
O projeto está organizado da seguinte forma:

superstore_case/
│
├── data/                  
│   └── superstore.csv     
├── eda_insights.ipynb     
├── ml_model.ipynb         
├── ia_generativa.ipynb    
├── ml_results.json        
├── README.md              
└── requirements.txt      

### 2. Requisitos Técnicos
- Python 3.8+
- Bibliotecas Python: As dependências estão listadas no arquivo requirements.txt.
- Google Colab, Jupyter Notebook ou VSCode: Para execução dos notebooks.
- Chave de API da OpenAI: Necessária para o notebook ia_generativa.ipynb. Obtenha uma chave em https://platform.openai.com/.
- Adicione a chave gerada na OpenAI ao executar o notebook ia_generativa.ipynb.

## 3. Como Executar o Projeto
Siga os passos abaixo para configurar e executar o projeto localmente.

#### 1. Clone o Repositório
#### 2. Crie um ambiente virtual
#### 3. Instale as dependências que está no arquivo requirements.txt

## 4. Execute os Notebooks na Ordem
Os notebooks devem ser executados na seguinte ordem:

#### 1° eda_insights.ipynb: Análise exploratória dos dados e geração de insights.
#### 2° ml_model.ipynb: Desenvolvimento e avaliação do modelo de machine learning.
#### 3° ia_generativa.ipynb: Geração de insights em linguagem natural usando IA generativa.

### Passo a Passo:
- Abra o notebook eda_insights.ipynb no Jupyter Notebook, Google Colab ou VSCode.
- Execute todas as células do notebook.
- Repita o processo para ml_model.ipynb e ia_generativa.ipynb.
- No notebook ia_generativa.ipynb, quando solicitado, insira sua chave da API da OpenAI.

## Notebook eda_insights.ipynb
##### Objetivo:
Realizar uma análise exploratória dos dados (EDA) para entender o dataset, identificar padrões e gerar insights relevantes para o negócio.

##### Principais Etapas:
- Carregamento e inspeção dos dados.
- Tratamento de valores nulos e conversão de tipos de dados.
- Análise estatística descritiva.
- Visualizações gráficas:
- Distribuição de vendas.
- Vendas por categoria de produto.
- Correlação entre variáveis.
- Lucro por subcategoria.
- Vendas por região.

#### Geração de 5 insights significativos.

##### Insights Gerados:
1° A maioria das vendas está concentrada em valores baixos, com poucos pedidos de alto valor.
2° A categoria Technology é a mais rentável.
3° Há uma tendência de crescimento nas vendas ao longo do tempo, com picos sazonais.
4° Descontos altos impactam negativamente o lucro.
5° A região West lidera em vendas, enquanto a região South tem o menor volume.

## Notebook ml_model.ipynb
##### Objetivo:
Desenvolver um modelo de machine learning para previsão de vendas e avaliar seu desempenho.

##### Principais Etapas:
- Divisão dos dados em treino (60%), validação (20%) e teste (20%).
- Treinamento de um modelo de Random Forest com ajuste de hiperparâmetros usando GridSearchCV.
- Avaliação do modelo nos conjuntos de validação e teste.
- Cálculo de métricas: MSE, RMSE, MAE e R².
- Interpretação da importância das features.
- Exportação dos resultados para o arquivo ml_results.json.

##### Resultados Obtidos:
- Melhores hiperparâmetros: {'n_estimators': 200, 'max_depth': 20, 'min_samples_split': 2}.
- Métricas no conjunto de teste:
- MSE: 1050.50
- RMSE: 32.40
- R²: 0.84
- Feature mais importante: Quantity (importância de 0.45).

## Notebook ia_generativa.ipynb
##### Objetivo:
Integrar os resultados do modelo de machine learning com IA generativa para gerar insights em linguagem natural.

##### Principais Etapas:
- Carregamento dos resultados do modelo a partir do arquivo ml_results.json.
- Configuração da API da OpenAI.
- Geração de um prompt com base nos resultados do modelo.
- Uso do modelo gpt-3.5-turbo-instruct para gerar insights em linguagem natural.
- Exibição dos insights gerados.

## Racional do Processo
  
### Análise Exploratória (EDA):
A EDA foi essencial para entender a distribuição dos dados, identificar padrões e gerar insights iniciais que orientaram a modelagem.

### Modelagem de Machine Learning:
O modelo de Random Forest foi escolhido por sua robustez, facilidade de interpretação e capacidade de lidar com dados não lineares.
A divisão dos dados em treino, validação e teste garantiu uma avaliação justa e confiável do modelo.

### IA Generativa:
A integração com a OpenAI permitiu transformar os resultados técnicos em insights acionáveis e de fácil compreensão para o negócio.

