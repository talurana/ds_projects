# RU: Проект анализа данных для "ЭкоФерма": Модели прогнозирования удоя и вкуса молока

### Данный проект создан в рамках курса Яндекс Практикум: Data Science

Проект направлен на анализ и моделирование данных для фермы "ЭкоФерма", с целью прогнозирования удоя молока и его вкуса у коров.

## Используемые библиотеки:
- pandas
- seaborn
- matplotlib
- numpy
- scipy
- sklearn
- phik

## Задачи проекта:

### Основная задача:
Анализ и прогнозирование удоя молока и его вкуса у коров фермы "ЭкоФерма".

### В рамках проекта необходимо сделать:
- Удаление дубликатов и предобработка данных.
- Проведение исследовательского анализа данных (EDA) с визуализацией.
- Обучение и оценка моделей линейной и логистической регрессии.
- Формулировка рекомендаций по улучшению моделей и подхода к кормлению.

## Основные этапы проекта:
### В ходе проекта были выполнены следующие шаги:

1. Первичный анализ данных:
   - Произведено удаление полных и неявных дубликатов.
   - Проведён анализ количественных и категориальных переменных, построены столбчатые и круговые диаграммы.

2. Обработка данных:
   - Устранение выбросов для переменных и анализ распределения.
   - Расчёт корреляций и выявление мультиколлинеарности.

3. Анализ сезонности и тренда:
   - Обнаружена нелинейная связь для ряда признаков и проведена их трансформация.
   - Выданы рекомендации по изменению подхода к кормлению с учётом увеличения показателей содержания в рационе.

4. Обучение моделей:
   - Обучены три модели линейной регрессии. Для лучшей модели:
     - MSE: 35316
     - MAE: 144.64
     - RMSE: 187.93
     - R²: 0.83
   - Обучена модель логистической регрессии для прогноза вкуса молока.

5. Классификация и оценка:
   - Для модели логистической регрессии проведён анализ и подбор порога классификации (0.7), чтобы минимизировать ошибки первого рода.
   - Проверка результатов и формулирование рекомендаций.

### Результаты и выводы:
- Для фермеров были найдены две коровы, соответствующие критериям вкусного молока.
- Модели достигли удовлетворительных метрик и предложены рекомендации по улучшению.

## Автор:

- Тарасова Ульяна  
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana)

# EN: Data Analysis Project for "EcoFarm": Milk Yield and Flavor Prediction Models

### This project was created as part of the Yandex Practicum: Data Science course.

The project is focused on data analysis and modeling for the "EcoFarm" to predict the milk yield and flavor quality of cows.

## Libraries Used:
- pandas
- seaborn
- matplotlib
- numpy
- scipy
- sklearn
- phik


## Project Objectives:

### Main Objective:
Analyze and predict the milk yield and flavor quality of cows at "EcoFarm".

### Tasks to be Accomplished:
- Remove duplicates and preprocess data.
- Conduct exploratory data analysis (EDA) with visualization.
- Train and evaluate linear and logistic regression models.
- Formulate recommendations for model improvement and feeding approach adjustments.

## Key Project Steps:
### The following steps were performed during the project:

1. Initial Data Analysis:
   - Removed full and implicit duplicates.
   - Analyzed quantitative and categorical variables using bar and pie charts.

2. Data Processing:
   - Identified and treated outliers, analyzed distributions.
   - Calculated correlations and detected multicollinearity.

3. Seasonality and Trend Analysis:
   - Detected nonlinear relationships in several features and performed transformations.
   - Provided recommendations to adjust the feeding approach based on nutrient content.

4. Model Training:
   - Trained three linear regression models. For the best model:
     - MSE: 35316
     - MAE: 144.64
     - RMSE: 187.93
     - R²: 0.83
   - Trained a logistic regression model to predict milk flavor.

5. Classification and Evaluation:
   - Analyzed and set a classification threshold (0.7) for the logistic regression model to minimize Type I errors.
   - Conducted result verification and formulated recommendations.

### Results and Conclusions:
- Two cows meeting the criteria for flavorful milk were identified for the farmers.
- The models achieved satisfactory metrics, and recommendations for improvement were provided.

## Author:

- Ulyana Tarasova  
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana) 

