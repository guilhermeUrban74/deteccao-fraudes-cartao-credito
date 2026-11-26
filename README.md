# Detecção de Fraudes em Cartões de Crédito com Machine Learning

## Sobre o projeto

Este projeto tem como objetivo desenvolver modelos de Machine Learning capazes de identificar transações fraudulentas em cartões de crédito, utilizando técnicas de classificação e análise de dados.

O desafio principal é trabalhar com um conjunto de dados altamente desbalanceado, no qual as transações fraudulentas representam uma pequena parcela do total.

## Objetivos

- Analisar e explorar os dados.
- Identificar o desbalanceamento entre transações normais e fraudulentas.
- Preparar os dados para treinamento.
- Desenvolver e comparar modelos de Machine Learning.
- Avaliar os resultados utilizando métricas de classificação.
- Interpretar as decisões dos modelos com SHAP.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Google Colab

## Modelos desenvolvidos

- Regressão Logística
- Random Forest
- XGBoost
- Random Forest otimizado com GridSearchCV

## Resultados

| Modelo | ROC-AUC | PR-AUC | Precisão | Recall | F1-score |
|---|---:|---:|---:|---:|---:|
| Regressão Logística | 0.9711 | 0.7113 | 0.06 | 0.92 | 0.11 |
| Random Forest | 0.9529 | 0.8543 | 0.96 | 0.74 | 0.84 |
| XGBoost | 0.9811 | 0.8327 | 0.35 | 0.87 | 0.49 |
| Random Forest Otimizado | 0.9766 | 0.8177 | 0.82 | 0.83 | 0.82 |

*As métricas de Precisão, Recall e F1-score referem-se à classe de transações fraudulentas, utilizando o limite padrão de classificação de 0,5.*

## Análise e conclusões

O Random Forest apresentou o melhor equilíbrio entre precisão e recall, alcançando F1-score de 0.84 e PR-AUC de 0.8543.

O XGBoost apresentou o maior ROC-AUC, com 0.9811.

Também foram realizados testes com diferentes limites de decisão e otimização de hiperparâmetros utilizando GridSearchCV.

A análise SHAP foi utilizada para compreender a influência das variáveis nas previsões do modelo.

## Dataset

O conjunto de dados utilizado contém 284.807 transações, sendo 492 fraudulentas.

Fonte: [Credit Card Fraud Detection Dataset](https://storage.googleapis.com/download.tensorflow.org/data/creditcard.csv)

O dataset é carregado diretamente pelo notebook, não sendo necessário armazenar o arquivo CSV no repositório.

## Aprendizados

Este projeto proporcionou experiência prática com análise exploratória de dados, preparação de dados, classificação, avaliação de modelos, tratamento de dados desbalanceados, otimização de hiperparâmetros e explicabilidade em Machine Learning.
