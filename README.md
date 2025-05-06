# Шпаргалка:
`
CREATE TABLE - Создать таблицу
`
`
DROP TABLE - Удалить таблицу
`
`
TRUNCATE TABLE table_name - Удалить все данные из таблицы
`
`
INSERT INTO - Вставить данные
`
`
SELECT * FROM - Вывести все записи
`
`
UPDATE - Обновить данные
`
`
DELETE FROM - Удалить данные
`
`
SHOW DATABASES - Показать все базы данных
`
`
CREATE DATABASE - Создать базу данных
`
`
DROP DATABASE dbname - Удалить базу данных
`
`
ALTER TABLE - Изменение типа столбца
`

# Лабораторная работа №1
1) Выберите из таблицы orders все заказы.

![Image](https://i.imgur.com/QFxDKpE.png)
2) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in:

![Image](https://i.imgur.com/ZkSqJGZ.png)

3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".
![Image](https://i.imgur.com/B6Jnwhy.png)

4) Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа:
![Image](https://i.imgur.com/gArGNhP.png)



# Лабораторная работа №2

1) Выберите из таблицы orders 3 самых дешевых заказа за всё время. Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывайте.
![Image](https://i.imgur.com/VPBQRZX.png)

2) Выберите из таблицы orders 2 самых дорогих заказов за всё время. Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывайте.
![Image](https://i.imgur.com/JANF2dA.png)

3) Добавьте в таблицу orders данные о новом заказе стоимостью 8000 рублей. В заказе 4 товара (products).
![Image](https://i.imgur.com/zl3eItz.png)
![Image](https://i.imgur.com/fRJvPRi.png)

5) Добавьте в таблицу products новый товар — «VR-очки», стоимостью 70000 рублей в количестве (count) 2 штук.
![Image](https://i.imgur.com/0zXjhuA.png)
![Image](https://i.imgur.com/QSVUM99.png)
7) В таблицу products внесли данные с ошибкой, вместо "PS5" в наименовании написали IMAC. Исправьте ошибку.
![Image](https://i.imgur.com/T3nqVaM.png)
![Image](https://i.imgur.com/3HCxd6a.png)



# Лабораторная работа №3
Создайте таблицу users с полем id типа INT и двумя текстовыми полями, которые будут хранить имя (first_name) и фамилию (last_name). Длина имени и фамилии не превышает 50 символов. Добавьте в таблицу трех пользователей: Дмитрия Иванова, Анатолия Белого и Дениса Давыдова.

CREATE TABLE users (id INT, first_name VARCHAR (50), last_name VARCHAR (50)); INSERT INTO users (id, first_name, last_name) VALUE (1, 'Дмитрий', 'Иванов'), (2, 'Анатолий', 'Белый'), (3, 'Денис', 'Давыдов'); image image
![418252857-5b7036e5-d0e6-4971-b655-904454b47ec0](https://github.com/user-attachments/assets/a72136e4-cfa0-46a0-8cc5-5def7d39ebfe)


