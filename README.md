# Домашнее задание к занятию "`«SQL. Часть 1»`" - `Бызгаев Александр`

---

### Задание 1

Получите уникальные названия районов из таблицы с адресами, которые начинаются на “K” и заканчиваются на “a” и не содержат пробелов.

### Решение:

```
select district as from address
where district like 'K%a' and district not like '% %';
```

![image](https://github.com/Byzgaev-I/SQL.Part-1/blob/main/1.png)


---

### Задание 2

Получите из таблицы платежей за прокат фильмов информацию по платежам, которые выполнялись в промежуток с 15 июня 2005 года по 18 июня 2005 года включительно и стоимость которых превышает 10.00.

### Решение:

```
select * from payment
where date(payment_date) >= '2005-06-15' and date(payment_date) <= '2005-06-18' and amount > 10.00
order by payment_date asc;
```

![image](https://github.com/Byzgaev-I/SQL.Part-1/blob/main/2.png)
