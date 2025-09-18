# 🚢 Desafio Titanic: Previsão de Sobreviventes com Machine Learning

## 🎯 Objetivo do Projeto

Este projeto representa minha primeira aplicação prática e completa de um pipeline de Data Science. O objetivo foi utilizar o famoso dataset do Titanic, disponível no Kaggle, para construir um modelo de Machine Learning capaz de prever se um passageiro sobreviveu ou não ao desastre.

Mais do que apenas alcançar uma alta acurácia, o foco foi aplicar e solidificar os conhecimentos recém-adquiridos em cada etapa do fluxo de trabalho, desde a limpeza e análise dos dados até o treinamento, avaliação e submissão de um modelo preditivo.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Bibliotecas Principais:**
    * **Pandas:** Para manipulação e limpeza dos dados.
    * **Plotly Express & Matplotlib:** Para visualização e Análise Exploratória de Dados (EDA).
    * **Scikit-learn:** Para pré-processamento (`OneHotEncoder`, `MinMaxScaler`) e para a construção dos modelos de Machine Learning (`DecisionTreeClassifier`, `KNeighborsClassifier`).
* **Ambiente:** Google Colab / Jupyter Notebook

## 📂 O Pipeline do Projeto

O notebook segue um fluxo de trabalho estruturado, dividido nas seguintes etapas:

1.  **Análise Exploratória de Dados (EDA):**
    * Investigação inicial para entender a estrutura dos dados, identificar valores ausentes e visualizar a distribuição das variáveis.
    * Criação de gráficos com Plotly para analisar a relação entre as features (como `Sexo`, `Classe` e `Idade`) e a variável alvo (`Survived`).

2.  **Pré-processamento e Limpeza:**
    * Tratamento de valores nulos (imputação) em colunas críticas como `Age` e `Fare`.
    * Combinação estratégica dos dataframes de treino e teste para garantir consistência nas transformações.

3.  **Codificação de Variáveis Categóricas:**
    * Aplicação do `OneHotEncoder` para transformar variáveis categóricas (`Sex`, `Embarked`, `Pclass`) em um formato numérico que o modelo possa entender, utilizando um `ColumnTransformer` para um pipeline organizado.

4.  **Treinamento e Avaliação de Modelos:**
    * Divisão dos dados em conjuntos de treino e validação para uma avaliação justa do desempenho.
    * Treinamento de diferentes modelos de classificação (Árvore de Decisão e KNN).
    * Avaliação e comparação dos modelos com base na acurácia no conjunto de validação para escolher o melhor.

5.  **Geração da Submissão:**
    * Treinamento do modelo campeão com todos os dados de treino disponíveis.
    * Geração do arquivo `submission.csv` no formato exigido pela competição do Kaggle.

## ✨ Principais Aprendizados

* A importância crítica da **Análise Exploratória** para guiar as decisões de pré-processamento.
* A diferença fundamental entre `fit`, `transform` e `fit_transform` e a necessidade de evitar **Data Leakage** ao tratar os dados de treino e teste.
* Como construir um pipeline de transformação robusto com `ColumnTransformer`.
* A importância de separar um **conjunto de validação** para avaliar o modelo de forma imparcial e diagnosticar o overfitting.

---
