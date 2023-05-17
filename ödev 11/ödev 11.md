# Ödev 11

## Sorular

Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1. actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
2. actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
3. actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
4. İlk 3 sorguyu tekrar eden veriler için de yapalım.

## Cevaplar

1. Soru
``` sql
(
select first_name from actor
)
union
(
select first_name from customer
);
```
2. Soru
``` sql
(
select first_name from actor
)
intersect
(
select first_name from customer
);
```
 3. Soru
 ``` sql
(
select first_name from actor
)
except
(
select first_name from customer
);
```
 4. Soru
``` sql
(
select first_name from actor
)
union all
(
select first_name from customer
);
```










