# Classificador de SPAM

<div align="center">
  
![wordcloud](img/header.png)
  
</div>

Esse projeto tem como objetivo classificar emails como legítimos (ham) ou falsos (spam). Temos então um problema de classificação binário supervisionado offline. Em particular, estamos trabalhando com um problema de linguagem natural (NLP).

A execução foi separada em duas etapas: [ETL](https://github.com/franklinzppa/spam/blob/main/notebooks/ETL-spam.ipynb) e [modelagem](https://github.com/franklinzppa/spam/blob/main/notebooks/model-spam.ipynb). Na ETL, os dados foram obtidos via requisição, transformados em emails e categorias, e salvos em csv. Na modelagem os dados foram pré-processados, analisados (**análise de sentimentos**, wordcloud, etc) e modelados com **machine learning** e **deep learning**. 

A avaliação foi realizada com validação cruzada estratificada de 5 folds. Os resultados obtidos nos dados de teste com o melhor modelo (SVC) foram

<div align="center">

### Métricas de teste

Acurácia   | **Precisão** | Recall
---------  | -------- | ------ |
99%      | 99%    | **96%** 

</div>