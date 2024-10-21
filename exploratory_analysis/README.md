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

# EN: Data Science Project Repository: Apartment Sale Advertisements Analysis

### This project was created as part of the Yandex Practicum: DataScience course.

The course provided the data for analysis. The project consists of a single file: a Jupyter Notebook (.ipynb) version.

## Libraries Used:
- seaborn
- matplotlib
- pandas

## Project Objectives

1. Data Preprocessing:
   - Fill missing values and identify reasons.
   - Check data types and eliminate duplicates.

2. Adding Columns:
   - Calculate price per square meter, weekday, month, year, floor type, and distance to the city center.

3. Data Analysis:
   - Plot histograms and handle anomalies.
   - Describe the observations.

4. Sales Analysis:
   - Examine sale times, plot histogram, calculate mean and median.

5. Price Factors:
   - Investigate the dependence of price on parameters and visualize it.
   - Calculate the average price per square meter in 10 localities.
   - For St. Petersburg, plot a graph of average cost based on distance from the center.

### The project involved the following steps:
- Data Preprocessing:
  - Filled in missing values, removed duplicates, and created new columns, including unique names for localities, apartment level in relation to the building, price per square meter, and distance to the city center in kilometers.
- Correlation Analysis:
  - Analyzed the dependence of apartment price on various features such as total area, living area, kitchen area, number of rooms, floor type (first, last, or other), and date of listing (weekday, month, year). The strongest correlation was found for total and living area, and kitchen area, in decreasing order of strength. A weaker correlation was also found between price and the number of rooms.
- Impact of Distance to Center:
  - Analysis showed that the price of apartments in St. Petersburg monotonically decreases with the increasing distance from the center within a certain range.
- Independence of Features:
  - No significant dependence was found between the floor level and the number of days a listing is on the market, suggesting their independence.
- Analysis of Average Price per Square Meter:
  - Calculated the average price per square meter in the 10 localities with the most listings. Results showed that the most expensive localities are Pushkin and St. Petersburg, as well as Kudrovo and Pargolovo; the most budget-friendly are Gatchina and Vsevolozhsk.
- Evaluation of Apartment Sale Duration:
  - On average, it takes about a hundred days to sell an apartment. Most apartments sell within 40-230 days; the minimum sale period is one day. A sale period of less than 40 days is considered fast, while a period of more than 230 days indicates a long sale period. Listings on the market for more than 450 days account for 10% of the total.

### The following steps were performed during the project:
Data handling included:
   - Filling in missing data with median values in the columns days_employed and total_income, which account for total work experience in days and monthly income, respectively.
   - Identifying and removing anomalies in the data - removing rows where the children column indicates a negative number of children or an abnormally large number: 20. For anomalies like negative work experience in the days_employed column, the values were replaced with positive ones.
   - For education — unifying the data representation for the client's education level to eliminate implicit duplicates that could affect further analysis.
   - To assess the dependencies of income on debts, data was categorized into five categories based on income level.
   - For further analysis and data consistency, the purpose — the loan purpose — was categorized.

## Author:

- Tarasova Uliana
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)
