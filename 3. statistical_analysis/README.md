# RU: Репозиторий проектов в области Data Science: Исследование данных сервиса аренды самокатов GoFast

### Данный проект создан в рамках курса Яндекс Практикум: Data Science

Проект направлен на анализ поведения пользователей сервиса аренды самокатов GoFast и проверку гипотез с целью повышения эффективности бизнеса. Данные для анализа предоставляются в виде трёх CSV-файлов.

## Основной функционал, реализованный в проекте:
- Анализ пользовательского поведения и их поездок
- Проверка статистических гипотез
- Расчет выручки и анализ доходности подписок
- Обработка данных, включая предобработку и проверку на дубликаты

## Используемые библиотеки:
- pandas
- seaborn
- numpy
- matplotlib
- scipy
- statsmodels

## Задачи проекта:

### Основная задача:
Анализ данных с целью выявления инсайтов о поведении пользователей и проверки гипотез, которые могут поспособствовать развитию компании.

### Необходимо:
1. Загрузить данные и выполнить их предварительную обработку.
2. Провести исследовательский анализ данных, включая визуализацию.
3. Объединить данные о пользователях, поездках и подписках в единый датафрейм.
4. Рассчитать месячную выручку и проверить различные гипотезы.

### В ходе проекта были выполнены следующие шаги:
- Предварительный анализ данных:
  - Поиск и обработка пропусков и дубликатов. В таблице поездок удален 31 дубликат (2% от общего числа поездок).
  
- Исследовательский анализ данных:
  - Определено распределение пользователей по городам: наиболее популярным городом оказался Пятигорск, наименее — Москва.
  - Проанализировано соотношение пользователей с различными типами подписок и возрастная структура клиентов.
  - Рассмотрены длины и длительности поездок, подтверждена нормальная форма распределений.

- Агрегация данных и проверка гипотез:
  - Создана таблица агрегированных данных с добавленной информацией о подписках и выручке.
  - Проверены три основные гипотезы о времени поездок, среднем расстоянии, и выручке подписчиков; подтверждено, что пользователи с подпиской более выгодны.
  - Подготовлены рекомендации для маркетинговой стратегии и улучшений в хранении данных.

## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)

# EN: Data Science Project Repository: Analysis of the GoFast Scooter Rental Service

### This project was created as part of the Yandex Practicum: Data Science course

The project aims to analyze the behavior of users of the GoFast scooter rental service and test hypotheses to improve business efficiency. The data for analysis is provided in three CSV files.

## Key functionalities implemented in the project:
- Analysis of user behavior and their trips
- Testing statistical hypotheses
- Calculation of revenue and analysis of subscription profitability
- Data processing, including preprocessing and checking for duplicates

## Libraries used:
- pandas
- seaborn
- numpy
- matplotlib
- scipy
- statsmodels

## Project objectives:

### Main objective:
To analyze data with the goal of gaining insights into user behavior and testing hypotheses that can contribute to company growth.

### Tasks:
1. Load the data and perform preliminary processing.
2. Conduct an exploratory data analysis, including visualization.
3. Merge user, trip, and subscription data into a single dataframe.
4. Calculate monthly revenue and test various hypotheses.

### The following steps were completed in the project:
- Preliminary data analysis:
  - Search for and handle missing values and duplicates. Removed 31 duplicates from the rides table (2% of total ride entries).
  
- Exploratory data analysis:
  - Determined the distribution of users across cities: Pyatigorsk was the most popular city, while Moscow had the least users.
  - Analyzed the ratio of users with different subscription types and the age structure of clients.
  - Examined trip lengths and durations, confirming a normal distribution shape.

- Data aggregation and hypothesis testing:
  - Created a table of aggregated data, including information on subscriptions and revenues.
  - Tested three main hypotheses regarding trip time, average distance, and subscriber revenue; confirmed that subscribed users are more profitable.
  - Developed recommendations for marketing strategy and improvements in data storage.

## Author:

- Uliana Tarasova
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana)