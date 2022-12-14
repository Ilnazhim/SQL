# SQL

INSERT INTO 
  my_books
VALUES 
 (17, 'Евгений Онегин',1,'Александр Пушкин','1832-01-01',736,330,4.7); 
 
 UPDATE books 
 SET rating = 4.9 
 WHERE author='Лев Толстой'
 
 DELETE FROM
    название_таблицы
WHERE 
    условие; -- определяем условие, по которому будем отбирать строки 
    
    SELECT -- перечисляют только те поля, которые нужны
    TABLE_1.поле_1 AS поле_1,
    TABLE_1.поле_2 AS поле_2,
    ...
    TABLE_2.поле_n AS поле_n
FROM
    TABLE_1
INNER JOIN TABLE_2 ON TABLE_2.поле_1 = TABLE_1.поле_2; 


SELECT 
    TABLE_1.поле_1 AS поле_1,
    TABLE_1.поле_2 AS поле_2,
    ...
    TABLE_2.поле_n AS поле_n
FROM
    TABLE_1
LEFT JOIN TABLE_2 ON TABLE_2.поле = TABLE_1.поле; 

SELECT 
    TABLE_1.поле_1 AS поле_1,
    TABLE_1.поле_2 AS поле_2,
    ...
    TABLE_2.поле_n AS поле_n
FROM
    TABLE_1
RIGHT JOIN TABLE_2 ON TABLE_1.поле = TABLE_2.поле; 


SELECT 
    * 
FROM 
    books
WHERE 
    author LIKE '%Толст__'; 

API

API (Application Programming Interface — программный интерфейс приложения) — 
интерфейс, который помогает приложениям взаимодействовать.
