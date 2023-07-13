# ml-4-cyber-def

Este repositório contém uma coleção de Jupyter Notebooks que implementam modelos de Machine Learning para classificação de ciberataques, além de métricas em formato csv (Comma-separated values) e uma planilha que engloba os resultados. Os notebooks foram criados como parte de um projeto de pesquisa em segurança da informação e foram utilizados para treinar e avaliar diferentes algoritmos de aprendizado de máquina, bem como técnicas de pré-processamento e refinamento de hiper-parâmetros para identificar e classificar tipos de ciberataques.

## Notebooks

- [preprocessing.ipynb](Programas/preprocessing.ipynb): Notebook responsável pela preparação e pré-processamento dos dados do dataset CSE-CIC-IDS2018 utilizados no treinamento dos modelos.

- [preprocessing-kdd.ipynb](Programas/preprocessing-kdd.ipynb): Notebook responsável pela preparação e pré-processamento dos dados do dataset KDD-1999 utilizados no treinamento dos modelos.

- [ASSEMBLE_FINAL.ipynb](Programas/ASSEMBLE_FINAL.ipynb): Notebook que realiza o treinamento automatizado de todos os modelos de Machine Learning para classificação de ciberataques e gera as métricas para análise.

- [ASSEMBLE_FINAL_NO_PREPROC.ipynb](Programas/ASSEMBLE_FINAL_NO_PREPROC.ipynb): Notebook que realiza o treinamento automatizado de todos os modelos de Machine Learning para classificação de ciberataques e gera as métricas para análise com os datasets que não passaram pelas etapas de pré-processamento.

- Outros Notebooks: Os demais notebooks testam o funcionamento dos algoritmos separadamente, implementando os algoritmos Random Forest, Decision Treee, Naive Bayes, Support Vector Machines, XGBoost, K-Neighbors e Rede Neural.

## Conjunto de Dados

Os conjuntos de dados utilizados para treinamento e teste dos modelos foram o [KDD-1999](https://kdd.org/kdd-cup/view/kdd-cup-1999) e o [CSE-CIC-IDS2018](https://registry.opendata.aws/cse-cic-ids2018).

## Métricas

As seguintes métricas são geradas a partir dos modelos de classificação treinados:

- Acurácia: proporção de instâncias corretamente classificadas em relação ao total de instâncias.

- Precisão: proporção de instâncias positivas corretamente classificadas em relação ao total de instâncias classificadas como positivas.

- Recall (Revocação): proporção de instâncias positivas corretamente classificadas em relação ao total de instâncias reais positivas.

- F1-Score: média harmônica entre precisão e recall, fornecendo uma medida equilibrada entre as duas métricas anteriores.

- ROC-AUC: medida de desempenho utilizada para avaliar a qualidade de um modelo de classificação binária. A curva ROC é obtida pela representação da taxa de verdadeiros positivos (TPR ou recall) em relação à taxa de falsos positivos (FPR ou 1 - Especificidade) para vários valores do limiar de classificação.

A planilha [Métricas Finais.ods](Métricas/Métricas%20Finais.ods) centraliza todos os arquivos .csv, contendo os resultados dos 3 cenários de análise. 

