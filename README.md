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
