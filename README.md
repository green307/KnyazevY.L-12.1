# Домашнее задание к занятию 12.1. «Базы данных»

Легенда
Заказчик передал вам файл в формате Excel, в котором сформирован отчёт.

На основе этого отчёта нужно выполнить следующие задания.

Задание 1
Опишите не менее семи таблиц, из которых состоит база данных:

какие данные хранятся в этих таблицах;
какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.
Приведите решение к следующему виду:

Сотрудники (

идентификатор, первичный ключ, serial,
фамилия varchar(50),
...
идентификатор структурного подразделения, внешний ключ, integer).


Ответ:

Какие данные хранятся в этих таблицах :

1 фио - фамилия имя и отчество сотрудника

2 ОКЛАД - заработная плата сотрудника

3 должность - Занимаемая должность сотрудника

4 Тип подразделения - отдел в котором работает сотрудник

5 Дата - дата найма сотрудника

6 Адрес - местонахождение филиала

7 Проэкт - наименование проэкта для конкретного сотрудника.




Какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.

1 фио - строковый (varchar)

2 ОКЛАД - числовой (decimal/numeric)

3 должность - строковый (varchar)

4 Тип подразделения - строковый (varchar)

5 Дата - дата и время (tinyint)

6 Адрес - местонахождение филиала (varchar)

7 Проэкт - строковый (varchar)




решение к следующему виду:




Staff (

Staff_id primary_key,

FName VARCHAR(50) ,

LName VARCHAR(50) ,

Patronymic varchar(50),

Divisions_id varchar(50),

Structura_id varchar(50),

Date_off_id datetime,

Position_id varchar(50),

Salary_id numeric,

Address_id VARCHAR(50),

Project_id VARCHAR(50),

)

Salary (

Salary_id primary_key

Pay numeric

)

Position (

Position_id primary_key

Spethion_type

)

Divisions (

Divisions_id primary_key

Department varchar(50)

Unit Group varchar(50)

Unit Group_type

Department_type

)

Structura (

Structura_id primary_key

Group varchar(50)

Structura_type

Structura_title

)

Date_off_Employee )

Date_off_id primary_key

Date datetime

(

Branch address (

Address_id primary_key

Edge VARCHAR(50)

City VARCHAR(50)

Street VARCHAR(50)

House VARCHAR(50)

)

Project (

Project_id primary_key

Project_type

)
