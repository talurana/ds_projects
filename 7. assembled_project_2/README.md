# RU: Репозиторий проектов в области Data Science: Анализ и прогноз удовлетворённости и оттока сотрудников для компании «Работа с заботой»

### Данный проект создан в рамках задания, направленного на предсказание удовлетворённости работой сотрудников и их склонности уходить из компании.

## Основной функционал, реализованный в проекте:
- Анализ данных и подготовка признаков
- Обучение моделей для предсказания уровня удовлетворённости и увольнений
- Интерпретация и оценка моделей

## Используемые библиотеки:
- pandas
- seaborn
- matplotlib
- numpy
- scipy
- shap
- phik
- sklearn

## Используемые модели и технологии:
- Модели машинного обучения: 
  - Для предсказания удовлетворённости: Lasso, DecisionTreeRegressor, Ridge
  - Для предсказания увольнений: LogisticRegression, SVC, KNeighborsClassifier, DecisionTreeClassifier
- Пайплайн для предобработки данных:
  - Кодирование признаков с использованием OrdinalEncoder и OneHotEncoder
  - Масштабирование данных с MinMaxScaler, StandardScaler, и RobustScaler
  - Подбор гиперпараметров с использованием GridSearchCV и RandomizedSearchCV

## Задачи проекта:

### Основная задача:
1. Предсказать уровень удовлетворенности сотрудника работой.
2. Предсказать вероятность увольнения сотрудника из компании.

### Требование к модели:
1. Для предсказания удовлетворённости: SMAPE ≤ 15 на тестовой выборке.
2. Для предсказания увольнений: ROC-AUC ≥ 0.91 на тестовой выборке.

### В рамках проекта необходимо сделать:
1. Загрузить и проанализировать данные.
2. Обработать и подготовить признаки для моделирования.
3. Обучить различные модели и интерпретировать результаты.
4. Сделать выводы о лучших моделях и предложить рекомендации для бизнеса.

### В ходе проекта были выполнены следующие шаги:
- Проведён первичный и исследовательский анализ данных:
    - Оценка количественных и категориальных признаков.
    - Проведение корреляционного анализа и выявление мультиколлинеарности.
    - Удаление дубликатов в данных и принятие решения об их оставлении в тестовой выборке.
- Обработка данных:
    - Создание пайплайна для предобработки данных с использованием различных методов кодирования и масштабирования.
- Обучение и тестирование моделей:
    - Использование моделей: Lasso, DecisionTreeRegressor для уровней удовлетворённости, и LogisticRegression, SVC, среди прочих, для увольнений.
    - Подбор гиперпараметров с помощью GridSearchCV и RandomizedSearchCV.
    - Оценка моделей по метрикам SMAPE и ROC-AUC.

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)


# EN: Data Science Project Repository: Employee Satisfaction and Attrition Analysis and Forecasting for "Careful Work" Company

### This project was created as part of an assignment aimed at predicting employee job satisfaction and their propensity to leave the company.

## Key Features Implemented in the Project:
- Data analysis and feature preparation
- Model training for predicting satisfaction levels and employee attrition
- Interpretation and evaluation of models

## Libraries Used:
- pandas
- seaborn
- matplotlib
- numpy
- scipy
- shap
- phik
- sklearn

## Models and Technologies Used:
- Machine Learning Models:
  - For satisfaction prediction: Lasso, DecisionTreeRegressor, Ridge
  - For attrition prediction: LogisticRegression, SVC, KNeighborsClassifier, DecisionTreeClassifier
- Data Preprocessing Pipeline:
  - Encoding features using OrdinalEncoder and OneHotEncoder
  - Data scaling using MinMaxScaler, StandardScaler, and RobustScaler
  - Hyperparameter tuning with GridSearchCV and RandomizedSearchCV

## Project Goals:

### Main Objectives:
1. Predict the level of employee job satisfaction.
2. Predict the likelihood of employee attrition from the company.

### Model Requirements:
1. For satisfaction prediction: SMAPE ≤ 15 on the test dataset.
2. For attrition prediction: ROC-AUC ≥ 0.91 on the test dataset.

### Project Steps:
1. Load and analyze the data.
2. Process and prepare features for modeling.
3. Train various models and interpret results.
4. Make conclusions about the best models and provide business recommendations.

### Steps Completed During the Project:
- Conducted initial and exploratory data analysis:
  - Evaluation of quantitative and categorical features.
  - Correlation analysis and detection of multicollinearity.
  - Deduplication in data and decision to retain duplicates in the test dataset.
- Data Processing:
  - Built a pipeline for preprocessing data with different encoding and scaling methods.
- Model Training and Testing:
  - Used models: Lasso, DecisionTreeRegressor for satisfaction levels, and LogisticRegression, SVC, among others, for attrition.
  - Hyperparameter tuning with GridSearchCV and RandomizedSearchCV.
  - Model evaluation based on SMAPE and ROC-AUC metrics.

## Author:

- Ulyana Tarasova
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana)
