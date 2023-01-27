## ODEV- 3

**country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.**

```sql
select country from country where country LIKE 'A%a'
```

**country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.**

```sql
select country from country where country LIKE '_____%n'
```

**film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.**

```sql
select title from film where title ILIKE '____%%T%'
```

**film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.**

```sql
select * from film where title LIKE 'C%' and length >= 90 and rental_rate IN (2.99)
```


