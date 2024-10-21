# RU: Репозиторий проектов в области Data Science: Анализ объявлений о продаже квартир

### Данный проект создан в рамках курса Яндекс Практикум: DataScience

Курс предоставил данные для анализа. Проект состоит из одного файла: Jupyter Notebook (.ipynb) версии.

## Используемые библиотеки:
- seaborn
- matplotlib
- pandas

## Задачи проекта

1. **Предобработка данных**:
   - Заполнить пропуски, зафиксировать причины.
   - Проверить типы данных и устранить дубликаты.

2. **Добавление столбцов**:
   - Рассчитать цену за м², день недели, месяц, год, тип этажа и расстояние до центра.

3. **Анализ данных**:
   - Построить гистограммы и обработать аномалии.
   - Описать наблюдения.

4. **Анализ продаж**:
   - Изучить время продажи, построить гистограмму, рассчитать среднее и медиану.

5. **Факторы стоимости**:
   - Исследовать зависимость цены от параметров и визуализировать.
   - Рассчитать среднюю цену м² в 10 населённых пунктах.
   - Для СПб построить график средней стоимости по расстоянию от центра.

### В ходе проекта были выполнены следующие шаги:
- Предобработка данных:
  - Проведено заполнение пропусков значениями, удаление дубликатов и создание новых столбцов, включая уникальные имена для населённых пунктов, уровень квартиры относительно здания, цену за квадратный метр и расстояние до центра города в километрах.
- Анализ корреляции:
  - Выполнен анализ зависимости цены квартиры от различных признаков, таких как общая площадь, жилая площадь, площадь кухни, количество комнат, тип этажа (первый, последний или другой) и дата размещения (день недели, месяц, год). Наиболее сильная зависимость была выявлена для общей и жилой площади, площади кухни — в порядке убывания силы. Также обнаружена более слабая зависимость цены от количества комнат.
- Влияние расстояния до центра:
  - Анализ показал, что цена квартир в Санкт-Петербурге монотонно уменьшается с увеличением расстояния от центра в пределах определённого диапазона.
- Независимость признаков:
  - Не была найдена значительная зависимость между уровнем этажа и количеством дней размещения объявления, что позволяет предположить их независимость.
- Анализ средней цены за квадратный метр:
  - Выполнено задание по вычислению средней цены одного квадратного метра в 10 населённых пунктах с наибольшим числом объявлений. Результаты показали, что самые дорогие населённые пункты — это Пушкин и Санкт-Петербург, а также Кудрово и Парголово; самые бюджетные — Гатчина и Всеволожск.
- Оценка продолжительности продаж квартир:
  - В среднем для продажи квартиры требуется около ста дней. Большинство квартир продаётся в диапазоне 40-230 дней; минимальный срок продажи составляет один день. Продажа менее 40 дней считается быстрой, тогда как срок более 230 дней указывает на долгую продажу. Объявления, находящиеся на продаже более 450 дней, составляют 10% от общего числа.

### В ходе проекта были выполнены следующие шаги:
В была проведена работа с данными, включающая в себя:
   - Заполнение пропусков данных медианным значением в столбцах `days_employed`, `total_income`, отвечающие за общий трудовой стаж в днях и ежемесячный доход соответственно
   - Поиск и удаление аномалий в данных - удаление строк, в которых в столбце `children` указано отрицательное количество детей и аномально большое: 20. Для аномалий в виде отрицательного стажа работы в столбце `days_employed` была произведена замена на положительные значения
   - Для `education` — уровень образования клиента было произведено приведение к единообразному представлению данных, которые являются неявными дубликатами и могут повлиять на дальшнейший анализ
   - Чтобы произвести оценку зависимостей дохода от задолжностей было проведено категоризирование данных на пять категорий в зависимости от уровня дохода
   - Для дальнейшего анализа и единообразности данных было произведено категоризирование данных `purpose` — цель получения кредита

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)

# ENG: DataScience project repository: Taxi Order Predictions

### This project was created as part of the Yandex Practicum course.

The course provided data for analysis and model training. The repository consists of two files: an HTML version of the project file and a Jupyter Notebook (.ipynb) version.

## Important features used in this project:
- Seasonal Decomposition: Residual, Seasonal, Trend
- Models: Ridge, Lasso, DecisionTreeRegressor, LGBMRegressor, RandomForestRegressor

## Used libraries in project:
- seaborn
- numpy
- matplotlib
- pandas
- statsmodels
- sklearn
- lightgbm

## Tasks:

### **Main task:** 
Create a model that can predict the number of cabs in the next hour.

### Model Requirement:
The value of the **RMSE** metric on the test sample should not exceed 48.

### Project Methodology:
1. Load the data and resample it one hour interval at a time.
2. Analyze the data.
3. Train different models with different hyperparameters. Make a test sample of size 10% of the original data.
4. Validate the data on the test sample and draw conclusions.

### The following steps were accomplished during the project:
- Primary data analysis:
    - Analyzed omissions and duplicates: absent
    - Replaced the index with the `datetime` column, sorted the index in ascending order, and resampled the data with the time period replaced with 1 hour. For the analysis, the data from March to August 2018 inclusive
- Seasonality and trend analysis:
    - Seasonality, trend and residuals were plotted. Seasonality during the day was analyzed and hypothesized the cause of increased demand. The seasonality in the data is 1 day
    - A dataframe with additional features - time lags - was created for forecasting. The best RMSE results on the number of lags = 24.
    - The data was split and prepared for model training
    - The general trend of the data is an increase in the number of orders with each month - the trend function is increasing. This may be due to both increased airport traffic - more planes, and long family vacations - it is much more convenient to call a cab than to ask someone to pick up from the airport.
- Model Training:
    - The models selected for consideration were LGBMRegressor, RandomForestRegressor, Ridge, Lasso, and DecisionTreeRegressor
    - The models for testing were selected based on the RMSE parameter on cross validation as well as model training time. LGBMRegressor was selected for further testing
- Model Testing:
    - Prediction visualization plots and RMSE calculation on the test data were plotted for the final decision. The best model was selected as LGBMRegressor based on its results on the training data as well as training time
    - The result of the final selected model satisfies the selection conditions < 48

## Author:

- Tarasova Uliana
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)
