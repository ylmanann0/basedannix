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


# Лабораторная работа №4
Создайте таблицу users для хранения информации о пользователях сайта. В таблице должны быть следующие поля:

id – идентификатор, целое положительное; email – адрес электронной почты, строка не более 100 символов; date_joined – дата регистрации (достаточно хранить дату, без времени) last_activity – дата и время последней активности (с точностью до секунд).

CREATE TABLE users( id INT UNSIGNED, email VARCHAR(100), date_joined DATE, last_activity DATETIME );

INSERT INTO users (id, email, date_joined, last_activity) VALUES (1, "user1@domain.com", "2014-12-12", "2016-04-08 12:34:54"), (2, "user2@domain.com", "2014-12-12", "2017-02-13 11:46:53"), (3, "user3@domain.com", "2014-12-13", "2017-04-04 05:12:07");
![423033796-5511b6d7-a988-4542-9490-31dd257329f3-1](https://github.com/user-attachments/assets/1230c3a2-11d6-44ca-972a-037fc94f9de5)
Создайте таблицу calendar для хранения календаря посетителей. В таблице должны быть следующие поля:

id – идентификатор записи в календаре, целое положительное; user_id – идентификатор пользователя, целое положительное; doctor_id – идентификатор доктора, целое положительное; visit_date – дата и время визита (точность до секунд).

Create table calendar ( id int unsigned, user_id int unsigned, doctor_id int unsigned, visit_date datetime); Insert into calendar (id, user_id, doctor_id, visit_date) Values (1, 1914 , 1, '2017-04-08 12:00:00'), (2, 12, 1, '2017-04-08 12:30:00'), (3, 4641, 2, '2017-04-09 09:00:00'), (4, 784, 1,'2017-04-08 13:00:00'), (5, 15, 2,'2017-04-09 10:00:00');

![423034725-aae46175-0619-4a99-9022-97a5e8d3ce19](https://github.com/user-attachments/assets/1d94657e-8951-4e33-a5ac-7c2765f4c131)
Создайте таблицу users , в которой будут следующие поля:

id — идентификатор, целые положительные числа. first_name— имя, строки до 50 символов. last_name — фамилия, строки до 60 символов. bio — биография, текст до 65000 символов.

create table users ( id int (10) unsigned, first_name varchar (50), last_name varchar (60), bio text ); INSERT INTO users (id, first_name, last_name, bio) VALUES (1,'Антон','Кулик','С отличием окончил 39 лицей.'), (2,'Сергей','Давыдов',''), (3,'Дмитрий','Соколов','Профессиональный программист.')

![423037453-9cff2921-70f6-44ef-af74-d45be801ed56](https://github.com/user-attachments/assets/b0a26db3-6846-49af-9c7a-b95663392116)

# Лабораторная работа №5
Выберите из таблицы orders 4 самых дорогих заказов за всё время. Данные нужно отсортировать в порядке убывания цены. Отмененные заказы не учитывайте.
SELECT * FROM orders WHERE STATUS IN ('new', 'in_progress', 'delivery') ORDER BY SUM DESC LIMIT 4;

![428267381-9e1c14d7-0fd8-45a7-bde8-a02b498fc76c](https://github.com/user-attachments/assets/d11b554d-3625-45f9-ad33-9fa678da5799)
Выберите из таблицы products название и цены четырех самых дешевых товаров, которые есть на складе.
SELECT NAME, price from products WHERE COUNT>0 LIMIT 4;

![428267463-997449e6-383a-4ce6-b821-77aff3f0c3cd](https://github.com/user-attachments/assets/ef6ba9cf-04eb-44fe-8cd0-30495903de31)
Выберите из таблицы orders три последних заказа (по дате date) стоимостью от 3200 рублей и выше. Данные отсортируйте по дате в обратном порядке.
SELECT * FROM orders WHERE SUM>=3200 ORDER BY DATE DESC LIMIT 3;

![428267803-d0ec4f7b-ea11-4197-b5be-0628c77731de](https://github.com/user-attachments/assets/ed740261-e157-4343-bb99-4616304e6229)
Создайте данную таблицу:
CREATE TABLE products (id INT, NAME VARCHAR (50), COUNT INT, price INT); INSERT INTO products (id, NAME, COUNT, price) VALUE (1, 'Стиральная машина', 5, 10000), (2, 'Холодильник', 0, 10000), (3, 'Микроволновка', 3, 4000), (4, 'Пылесос', 2, 4500), (5, 'Вентилятор', 0, 700), (6, 'Телевизор', 7, 31740), (7, 'Тостер', 2, 2500), (8, 'Принтер', 4, 3000), (9, 'Активные колонки', 1, 2900), (10, 'Ноутбук', 4, 36990), (11, 'Посудомоечная машина', 0, 17800), (12, 'Видеорегистратор', 23, 4000), (13, 'Смартфон', 8, 12300), (14, 'Флешка', 4, 1400), (15, 'Блендер', 0, 5500), (16, 'Газовая плита', 5, 11900), (17, 'Клавиатура', 3, 1800);

![428269950-c82c180f-f94c-467b-8d67-745f8bb23030](https://github.com/user-attachments/assets/65f1baf0-68be-4031-8b39-cc71da4a895a)
Из этой таблицы сделать выборку на основе задания: Сайт выводит товары по 5 штук. Выберите из таблицы products товары, которые пользователи увидят на 3 странице каталога при сортировке в порядке возрастания цены (price).
SELECT * FROM products ORDER BY price LIMIT 5 OFFSET 10;

![428270355-dba2d832-abc0-44a8-bf81-ab45de48ffb4](https://github.com/user-attachments/assets/38cdafda-a17a-487e-a2c5-58160add0527)


# Лабораторная работа №6
1)Создайте таблицу orders для хранения списка заказов:

id — идентификатор, целое положительное. user_id — идентификатор пользователя, который оформил заказ. Целое положительное, NULL запрещен. amount — стоимость заказа. Целое положительное число не более 1 млн. NULL запрещен, по умолчанию 0. created — дата и время создания заказа. NULL запрещен. state — статус заказа. Выбор из new, cancelled, in_progress, delivered, completed. Можно выбрать только один вариант. NULL запрещен. По умолчанию должен стоять new. Добавьте 3 записи так, чтобы получалась таблица ниже:

CREATE table orders (id INT UNSIGNED, user_id INT UNSIGNED NOT null, amount mediumint unsigned NOT NULL DEFAULT 0, created DATETIME NOT NULL, state ENUM ('NEW', 'cancelled', 'in_progress', 'delivered', 'completed') NOT NULL DEFAULT 'new'); INSERT INTO orders (id, user_id, amount, created, state) VALUES (1, 56, 5400, '2018-02-01 17:46:59', DEFAULT), (2, 90, 249, '2018-02-01 19:13:04', DEFAULT), (3, 78, 2200, '2018-02-01 22:43:09', DEFAULT);
![433009414-bce17f59-c4f3-486e-a565-f2df2c4f9579](https://github.com/user-attachments/assets/b8c1a016-5565-4981-9d0e-8250a152bb43)

2)Создайте таблицу users для хранения списка пользователей сайта:

id — идентификатор, целое положительное. first_name — имя, строка до 20 символов. NULL запрещен. last_name — фамилия, строка до 20 символов. NULL запрещен. patronymic — отчество, строка до 20 символов. NULL запрещен, по умолчанию пустая строка. is_active — отметка об активности пользователя. Логическое поле, по умолчанию TRUE. is_superuser — отметка администратора. Логическое поле, по умолчанию FALSE. Добавьте 3 записи так, чтобы получалась таблица ниже:

CREATE table users (id INT UNSIGNED, first_name VARCHAR(20) NOT NULL, last_name VARCHAR(20) NOT NULL, patronymic VARCHAR(20) NOT NULL DEFAULT '', is_active BOOLEAN DEFAULT TRUE, is_superuser BOOLEAN DEFAULT FALSE); INSERT INTO users (id, first_name, last_name, patronymic, is_active, is_superuser) VALUES (1, 'Дмитрий', 'Иванов', DEFAULT, DEFAULT, DEFAULT), (2, 'Анатолий', 'Белый', 'Сергеевич', DEFAULT, TRUE), (3, 'Андрей', 'Крючков', DEFAULT, FALSE, DEFAULT); SELECT * FROM users;

![433012470-78fa6624-3e2a-479f-b1f0-e79deaf5f1ba](https://github.com/user-attachments/assets/ede5c3d8-e747-4bc1-91d0-4f29b6d111bd)
3)Создайте таблицу products для хранения товаров в интернет магазине:

id — идентификатор, целое положительное. category_id — категория, целое положительное. Может принимать NULL. По умолчанию NULL. name — название, строка до 100 символов. NULL запрещен. count — количество, целое положительное до 255. NULL запрещен, по умолчанию 0. price — цена типа DECIMAL с 10 знаками, 2 из которых выделены для копеек. NULL запрещен, по умолчанию 0.00. Добавьте 3 записи так, чтобы получалась таблица ниже:

CREATE table products (id INT UNSIGNED, category_id INT DEFAULT NULL, name VARCHAR(100) NOT null, count TINYINT unsigned NOT NULL DEFAULT 0, price DECIMAL (10, 2) NOT NULL DEFAULT 0.00); INSERT INTO products (id, category_id, name, count, price) VALUES (1, 1, 'Кружка', 5, 45.90), (2, 17, 'Фломастеры', DEFAULT, 78.00), (3, NULL, 'Сникерс', 12, 50.80);

![433012117-dd8701ec-b515-410a-921f-ebe51530f83f](https://github.com/user-attachments/assets/d5555792-a820-4119-bb30-8f84ed6217f1)
