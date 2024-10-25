# RU: Прогнозированию оттока клиентов для оператора связи «ТелеДом»

### Данный проект создан в рамках курса Яндекс Практикум: DataScience

Проект направлен на создание модели, позволяющей спрогнозировать, разорвёт ли абонент договор. Это поможет оператору связи «ТелеДом» предложить специальные условия для удержания клиентов.

## Основной функционал, реализованный в проекте:
- Исследовательский анализ и предобработка данных
- Анализ корреляционных связей между признаками
- Использование машинного обучения для построения моделей (GradientBoostingClassifier, RandomForestClassifier, LGBMClassifier)
- Реализация пайплайна для предобработки данных (обработка пропусков, нормализация и кодирование признаков)
- Подбор гиперпараметров моделей с помощью RandomizedSearchCV
- Оценка качества моделей на основе метрик AUC-ROC и Accuracy

## Используемые библиотеки:
- gc, os, re
- numpy, pandas
- matplotlib, seaborn
- scipy, phik, shap
- sklearn
- lightgbm

## Задачи проекта:

### Основная задача:
Обучение модели для прогнозирования оттока клиентов с использованием метрики AUC-ROC не менее 0.85.

### В рамках проекта необходимо сделать:
1. Загрузить и осмотреть данные из различных источников.
2. Выполнить исследовательский анализ данных и объединить их в единый датафрейм.
3. Предобработать данные и подготовить признаки для моделирования.
4. Обучить несколько моделей машинного обучения и выбрать наилучшую по результатам кросс-валидации.
5. Проверить качество лучшей модели на тестовой выборке.

### В ходе проекта были выполнены следующие шаги:
- Первичный анализ данных:
    - Выполнена предобработка количественных и категориальных признаков.
    - Выявлены и обработаны выбросы и пропущенные значения.
- Обработка и объединение данных:
    - Выполнено объединение данных из разных источников по уникальному идентификатору клиента.
    - Проведен корреляционный анализ признаков.
- Обучение моделей:
    - Обучены модели GradientBoostingClassifier, RandomForestClassifier и LGBMClassifier с подбором гиперпараметров.
    - Модель GradientBoostingClassifier показала наилучший результат по метрике AUC-ROC 0.9016 на тестовой выборке.

### Вывод:
- Проделанный анализ данных и использование машинного обучения позволили достичь необходимой точности прогноза оттока клиентов.
- Разработанная модель может быть использована оператором для предоставления целевых предложений и снижения оттока клиентов.

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)

# EN: Customer Churn Prediction for Telecom Operator "TeleDom"

### This project was created as part of the Yandex Practicum: Data Science course

The project aims to develop a model that predicts whether a subscriber will terminate their contract. This will help the telecom operator "TeleDom" offer special conditions to retain customers.

## Key features implemented in the project:
- Exploratory data analysis and preprocessing
- Correlation analysis between features
- Use of machine learning for model building (GradientBoostingClassifier, RandomForestClassifier, LGBMClassifier)
- Implementation of a pipeline for data preprocessing (handling missing values, normalization, and feature encoding)
- Hyperparameter tuning with RandomizedSearchCV
- Evaluation of model quality based on AUC-ROC and Accuracy metrics

## Libraries used:
- gc, os, re
- numpy, pandas
- matplotlib, seaborn
- scipy, phik, shap
- sklearn
- lightgbm

## Project objectives:

### Main objective:
Train a model to predict customer churn with an AUC-ROC metric of at least 0.85.

### The project tasks include:
1. Load and inspect data from various sources.
2. Perform exploratory data analysis and combine them into a single dataframe.
3. Preprocess the data and prepare features for modeling.
4. Train several machine learning models and select the best one based on cross-validation results.
5. Test the performance of the best model on the test set.

### The following steps were completed in the project:
- Initial data analysis:
    - Conducted preprocessing of quantitative and categorical features.
    - Identified and handled outliers and missing values.
- Data processing and integration:
    - Combined data from different sources using a unique customer identifier.
    - Conducted a correlation analysis of features.
- Model training:
    - Trained GradientBoostingClassifier, RandomForestClassifier, and LGBMClassifier with hyperparameter tuning.
    - The GradientBoostingClassifier model showed the best result with an AUC-ROC of 0.9016 on the test set.

### Conclusion:
- The performed data analysis and use of machine learning allowed achieving the required accuracy for customer churn prediction.
- The developed model can be used by the operator to provide targeted offers and reduce customer churn.


## Author:

- Tarasova Uliana
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)
