# ödev 9

### Sorular
Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1. city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
2. customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
3. customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.

### Cevaplar

1. Soru
``` sql
select city, country from city
left join country on country.country_id = city.country_id;
```
2. Soru
``` sql
select payment_id, first_name, last_name from customer
right join payment on payment.customer_id = customer.customer_id; 
```
3. Soru
``` sql
select rental_id, first_name, last_name from customer
full join rental on rental.customer_id = customer.customer_id; 
```