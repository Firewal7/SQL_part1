# Домашнее задание к занятию 12.3 "Реляционные базы данных: SQL. Часть 1"
# Софьин Роман

## ЗАДАЧА 1

``` sql
SELECT DISTINCT district
FROM address
WHERE district LIKE "K%a" AND district NOT LIKE "% %";
```

![Задача 1](https://raw.githubusercontent.com/Firewal7/SQL1/main/1.1.png)

## ЗАДАЧА 2

``` sql
SELECT * FROM payment
WHERE (payment_date BETWEEN "2005-06-15 00:00:00" AND "2005-06-18 23:59:59") AND (amount > 10.00);
```

![Задача 2](https://raw.githubusercontent.com/Firewal7/SQL1/main/2.2.png)

## ЗАДАЧА 3

``` sql
SELECT * FROM rental
ORDER BY rental_date DESC
LIMIT 5;
```

![Задача 3](https://raw.githubusercontent.com/Firewal7/SQL_part1/main/3.3.png)

## ЗАДАЧА 4

``` sql
SELECT LOWER(REPLACE(name, 'LL', 'pp')) AS customer
FROM customer_list
WHERE (name LIKE 'Kelly%' OR name LIKE 'Willie%') AND (notes LIKE 'active');
```

![Задача 4](https://raw.githubusercontent.com/Firewal7/SQL1/main/4.4.png)