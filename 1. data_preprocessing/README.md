# Исследование надежности заемщиков

### Этот проект выполнен в рамках курса Яндекс Практикум: DataScience

## Основной функционал, реализованный в проекте:
- Предобработка данных: заполнение пропусков, обработка аномалий и дубликатов
- Категоризация доходов и целей кредита
- Анализ зависимости возврата кредита от различных факторов

## Используемые библиотеки:
- pandas

## Задачи проекта:

### Основная задача:
Анализ факторов, влияющих на возврат кредита в срок.

### В рамках проекта необходимо было сделать:
1. Загрузить данные и провести их предобработку.
2. Исследовать зависимости между возвратом кредита и различными факторами, такими как:
   - Количество детей
   - Семейное положение
   - Уровень дохода
   - Цели кредита
3. Написать общий вывод и рекомендации.

### В ходе проекта были выполнены следующие шаги:
- Предобработка данных:
  - Заполнение пропусков в столбцах days_employed и total_income медианными значениями.
  - Обработка аномалий: удаление строк с некорректными значениями количества детей и отрицательным стажем.
  - Приведение данных об образовании к единому виду для устранения дубликатов.
  - Категоризация данных по уровню дохода и целям кредита.
  
- Анализ данных:
  - Выявлена зависимость между количеством детей и возвратом кредита: доля должников увеличивается с увеличением числа детей.
  - Анализ влияния семейного положения показал, что неженатые и в разводе с большей вероятностью имеют задолженности.
  - Наиболее надежной группой по уровню дохода являются клиенты с доходом от 200001 до 1000000.
  - Выявлены цели кредита, наиболее связанные с возвратом в срок.

- Рекомендации:
  - Наиболее надежные клиенты: состоящие в браке, без детей, с доходом в указанном диапазоне, берущие кредит для проведения свадьбы или операций с недвижимостью.


## Автор:

- Тарасова Ульяна
- telegram: [talurana](https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: [talurana](https://github.com/talurana)

# Borrower Reliability Research

### This project was completed as part of the Yandex Practicum Data Science course

## Main Features Implemented in the Project:
- Data preprocessing: filling in missing values, handling anomalies and duplicates
- Income and loan purpose categorization
- Analysis of credit repayment dependencies on various factors

## Libraries Used:
- pandas

## Project Objectives:

### Main Objective:
Analyze factors affecting the timely repayment of loans.

### Project Steps:
1. Load data and preprocess it.
2. Investigate dependencies between loan repayment and factors such as:
   - Number of children
   - Marital status
   - Income level
   - Loan purposes
3. Write a summary and recommendations.

### Steps Completed During the Project:
- Data Preprocessing:
  - Filled missing values in days_employed and total_income columns with median values.
  - Handled anomalies by removing rows with incorrect values for number of children and negative work experience.
  - Standardized education data to eliminate duplicates.
  - Categorized data by income level and loan purposes.
  
- Data Analysis:
  - Identified dependence between number of children and credit repayment: the proportion of defaulters increases with the number of children.
  - Marital status analysis showed that unmarried and divorced individuals are more likely to have debts.
  - The most reliable income group consists of clients with income ranging from 200,001 to 1 million.
  - Identified loan purposes most associated with timely repayment.

- Recommendations:
  - Most reliable clients: married, without children, with income in the specified range, taking loans for weddings or real estate transactions.

## Author:

- Uliana Tarasova
- telegram: talurana (https://t.me/talurana)
- email: tarasova.ulya@gmail.com
- github: talurana (https://github.com/talurana)
