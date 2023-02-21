# ODEV-6

**film** tablosunda bulunan **rental_rate** sütunundaki değerlerin ortalaması nedir?

```sql
select AVG (Rental_rate) from film ;
```

**film** tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?

```sql
select COUNT(*) from film where title LIKE 'C%';
```

**film** tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?

```sql
select MAX(length) from film
where  rental_rate = 0.99
```

**film** tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?

```sql
select COUNT(DISTINCT(replacement_cost)) from film
where length > 150
```
