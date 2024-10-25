# RU: Репозиторий проектов в области Data Science: Определение локации для скважины

### Данный проект создан в рамках курса Яндекс Практикум: DataScience

Проект разработан для определения оптимальной локации бурения новой скважины на основе анализа геологоразведочных данных. В проекте используется Jupyter Notebook (.ipynb).

## Основной функционал, реализованный в проекте:
- Анализ данных и их предобработка
- Построение графиков распределения и матриц корреляции для признаков
- Модели: LinearRegression, Lasso, Ridge, ElasticNet
- Оценка рисков и расчет прибыли с помощью Bootstrap

## Используемые библиотеки:
- os
- seaborn
- pandas
- matplotlib
- numpy
- sklearn

## Задачи проекта:

### Основная задача:
Создание модели, которая поможет определить регион, где добыча принесёт наибольшую прибыль.

### В рамках проекта необходимо сделать:
1. Загрузить и подготовить данные.
2. Обучить и протестировать модели для каждого региона.
3. Провести оценку прибыльности и рисков с помощью техники Bootstrap.
4. Определить оптимальный регион для бурения.

### В ходе проекта были выполнены следующие шаги:
- Первичный анализ данных:
    - Проведена очистка данных от дубликатов.
    - Построены графики распределения для количественных признаков в каждом регионе.
    - Построены матрицы корреляции.
- Обучение моделей:
    - Реализован пайплайн для обучения моделей LinearRegression, Lasso, Ridge, ElasticNet.
    - Подбор лучших параметров для каждой модели в разных регионах.
- Анализ результатов:
    - Рассчитаны прибыль и риски для каждого региона.
    - Применена техника Bootstrap для оценки доверительных интервалов и рисков убытков.
- Итоговый вывод:
    - На основании оценки прибыли и рисков был выбран оптимальный регион для бурения.

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)


# EN: Data Science Project Repository: Well Location Selection

### This project was created as part of the Yandex Practicum: Data Science course.

The project is designed to determine the optimal location for drilling a new well based on geological exploration data analysis. The project utilizes a Jupyter Notebook (.ipynb).

## Main features implemented in the project:
- Data analysis and preprocessing
- Construction of distribution graphs and correlation matrices for features
- Models: LinearRegression, Lasso, Ridge, ElasticNet
- Risk assessment and profit calculation using Bootstrap

## Libraries used:
- os
- seaborn
- pandas
- matplotlib
- numpy
- sklearn

## Project Objectives:

### Main Objective:
Create a model to help determine the region where extraction will yield the highest profit.

### Steps to accomplish within the project:
1. Load and prepare the data.
2. Train and test models for each region.
3. Assess profitability and risks using Bootstrap.
4. Identify the optimal region for drilling.

### Steps performed during the project:
- Initial data analysis:
    - Removed duplicate data.
    - Constructed distribution graphs for quantitative features in each region.
    - Built correlation matrices.
- Model training:
    - Implemented a pipeline for training LinearRegression, Lasso, Ridge, ElasticNet models.
    - Parameter tuning for each model in different regions.
- Results analysis:
    - Calculated profit and risks for each region.
    - Applied Bootstrap to estimate confidence intervals and risk of loss.
- Final conclusion:
    - Based on profit and risk assessment, the optimal region for drilling was selected.

## Author:

- Ulyana Tarasova
- Telegram: talurana (https://t.me/talurana)
- Email: tarasova.ulya@gmail.com
- GitHub: talurana (https://github.com/talurana)