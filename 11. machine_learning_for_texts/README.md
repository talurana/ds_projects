# RU: Проект по классификации комментариев для интернет-магазина «Викишоп»

### Данный проект создан в рамках курса Яндекс Практикум: DataScience

Проект направлен на создание инструмента, позволяющего классифицировать комментарии пользователей интернет-магазина «Викишоп» на токсичные и нетоксичные. В конечном итоге, комментарии с токсичностью будут передаваться на модерацию.

## Основной функционал, реализованный в проекте:
- Анализ и предобработка текстовых данных
- Обучение моделей машинного обучения и нейронных сетей, включая BERT, для классификации токсичности комментариев

## Используемые библиотеки:
- os, re
- numpy, pandas
- matplotlib, seaborn
- wordcloud
- spacy, nltk
- sklearn
- lightgbm
- torch, transformers

## Задачи проекта:

### Основная задача:
Обучение модели для классификации комментариев на токсичные и нетоксичные с использованием метрики F1-score не менее 0.75.

### В рамках проекта необходимо сделать:
1. Загрузить и подготовить данные для анализа и обучения.
2. Выполнить анализ имеющихся текстовых данных.
3. Обучить различные модели, включая логистическую регрессию, CatBoost, LGBM и BERT.
4. Сравнить результаты моделей и сделать выводы по эффективности их работы.

### В ходе проекта были выполнены следующие шаги:
- Первичный анализ данных:
    - Подготовлена текстовая информация для дальнейшего анализа, включая обработку дисбаланса классов.
    - Построены визуализации и рассчитаны статистические показатели по длине, количеству слов и сентименту предложений.
- Обработка текстовых данных:
    - Выполнена очистка текста и лемматизация для улучшения качества моделей.
    - Рассчитаны признаки TF-IDF для текстовых данных.
- Обучение моделей:
    - Обучены и протестированы модели логистической регрессии, CatBoost, LGBM и BERT.
    - Модель BERT показала наилучший результат на тестовой выборке с F1-score 0.78.

### Вывод:
- Проект продемонстрировал эффективность использования предобученной модели BERT для задачи классификации текстов.
- Модель показала превосходные результаты, что позволяет рекомендовать её для использования в реальной системе интернет-магазина «Викишоп» для выявления токсичных комментариев.


## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)


# EN: Comment Classification Project for the "Wikishop" Online Store

### This project was created as part of the Yandex Practicum: DataScience course

The project aims to create a tool that classifies user comments for the "Wikishop" online store as toxic or non-toxic. Ultimately, comments identified as toxic will be sent for moderation.

## Core functionality implemented in the project:
- Analysis and preprocessing of text data
- Training of machine learning models and neural networks, including BERT, for toxic comment classification

## Libraries used:
- os, re
- numpy, pandas
- matplotlib, seaborn
- wordcloud
- spacy, nltk
- sklearn
- lightgbm
- torch, transformers

## Project tasks:

### Main goal:
To train a model that classifies comments as toxic or non-toxic with an F1-score of at least 0.75.

### The project involves:
1. Loading and preparing data for analysis and training.
2. Analyzing existing text data.
3. Training various models, including logistic regression, CatBoost, LGBM, and BERT.
4. Comparing model results and evaluating their effectiveness.

### The following steps were taken in the course of the project:
- Initial data analysis:
    - Text information was prepared for further analysis, including handling class imbalance.
    - Visualizations and statistical metrics were calculated for lengths, word counts, and sentiment of comments.
- Text data processing:
    - Text cleaning and lemmatization were performed to enhance model quality.
    - TF-IDF features for text data were calculated.
- Model training:
    - Logistic regression, CatBoost, LGBM, and BERT models were trained and tested.
    - The BERT model achieved the best result on the test sample with an F1-score of 0.78.

### Conclusion:
- The project demonstrated the effectiveness of using a pre-trained BERT model for text classification tasks.
- The model showed excellent results, making it recommendable for actual implementation in the "Wikishop" online store system for detecting toxic comments.

## Author:

- Tarasova Uliana
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)
