# RU: Репозиторий проектов в области Data Science: Оценка рыночной стоимости автомобилей

### Данный проект создан в рамках курса Яндекс Практикум: DataScience

Проект направлен на создание модели, позволяющей определить рыночную стоимость автомобилей, используя исторические данные о технических характеристиках, комплектациях и ценах. Проект выполнен в формате Jupyter Notebook (.ipynb).

## Основной функционал, реализованный в проекте:
- Предобработка данных: обработка пропусков, аномалий и дубликатов
- Модели: DecisionTreeRegressor, LGBMRegressor, KNeighborsRegressor, Ridge

## Используемые библиотеки:
- seaborn
- pandas
- matplotlib
- numpy
- os
- math
- sklearn
- lightgbm

## Задачи проекта:

### Основная задача:
Создание модели для оценки рыночной стоимости автомобилей.

### Требования к модели:
Значение метрики RMSE на тестовой выборке должно быть меньше 2500.

### В рамках проекта необходимо сделать:
1. Загрузить данные из файла и выполнить их предобработку.
2. Обучить различные модели, включая LightGBM и хотя бы одну модель, не использующую бустинг.
3. Проанализировать время обучения, предсказания и качество моделей.
4. Выбрать лучшую модель в соответствии с критериями заказчика и проверить её качество на тестовой выборке.

### В ходе проекта были выполнены следующие шаги:
- Анализ и предобработка данных:
    - Удалены данные с нулевой ценой и некорректными значениями мощности двигателя.
    - Пропущенные значения категориальных данных заполнены на основе частоты или отмечены как NotFilled.
    - Признак ремонта заполнен значением no.
    - Столбцы типа datetime заменены на разницу в днях относительно текущей даты.
    - Удалены дубликаты и неиспользуемые признаки: PostalCode, LastSeen, NumberOfPictures, DateCreated.
    - Построена матрица корреляции, показавшая сильную корреляцию между price, Power и RegistrationYear.
- Обучение моделей:
    - Гиперпараметры для моделей DecisionTreeRegressor, LGBMRegressor, KNeighborsRegressor, Ridge были подобраны с использованием RandomizedSearchCV.
    - Для категориальных признаков применялся OrdinalEncoder, для количественных — StandardScaler, RobustScaler, MinMaxScaler.
    - Наилучший результат показал LGBMRegressor с параметрами max_depth=6, n_estimators=500, random_state=5, learning_rate=0.1, RMSE составил 1798.
- Тестирование модели:
    - На тестовых данных получен результат RMSE 1800, удовлетворяющий требованиям проекта.

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)

# EN: Data Science Projects Repository: Estimating Car Market Value

### This project was created as part of the Yandex Practicum: Data Science course.

The project aims to develop a model that estimates the market value of cars using historical data on technical specifications, configurations, and prices. The project is implemented in Jupyter Notebook (.ipynb) format.

## Main functionality implemented in the project:
- Data preprocessing: handling missing values, anomalies, and duplicates
- Models: DecisionTreeRegressor, LGBMRegressor, KNeighborsRegressor, Ridge

## Libraries used:
- seaborn
- pandas
- matplotlib
- numpy
- os
- math
- sklearn
- lightgbm

## Project Objectives:

### Main Objective:
Create a model to estimate the market value of cars.

### Model Requirements:
The RMSE metric on the test set should be less than 2500.

### Tasks Required for the Project:
1. Load and preprocess data from the file.
2. Train different models, including LightGBM and at least one non-boosting model.
3. Analyze the training time, prediction speed, and quality of models.
4. Select the best model based on customer criteria and test its quality on the test set.

### Steps performed during the project:
- Data Analysis and Preprocessing:
    - Removed data with zero price and incorrect engine power values.
    - Filled missing values in categorical data based on frequency or marked them as NotFilled.
    - Filled the repair indicator with the value 'no'.
    - Replaced datetime columns with the difference in days relative to the current date.
    - Removed duplicates and unused features: PostalCode, LastSeen, NumberOfPictures, DateCreated.
    - Built a correlation matrix showing a strong correlation between price, Power, and RegistrationYear.
- Model Training:
    - Tuned hyperparameters for models DecisionTreeRegressor, LGBMRegressor, KNeighborsRegressor, Ridge using RandomizedSearchCV.
    - Used OrdinalEncoder for categorical features and StandardScaler, RobustScaler, MinMaxScaler for quantitative ones.
    - Best results achieved with LGBMRegressor with parameters max_depth=6, n_estimators=500, random_state=5, learning_rate=0.1, RMSE of 1798.
- Model Testing:
    - Achieved an RMSE of 1800 on test data, meeting the project's requirements.

## Author:

- Ulyana Tarasova
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana)
