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

