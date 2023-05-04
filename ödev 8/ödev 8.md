# Ödev 8

## Sorular

1. test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
2. Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

-----
## Cevaplar
1. Soru
``` sql
CREATE TABLE employee (
	id SERIAL PRIMARY KEY,
	name VARCHAR (50) NOT NULL,
	birthday DATE NOT NULL,
	email VARCHAR (100) 
);
```
2. Soru
``` sql
insert into employee (name, birthday, email) values ('Godart', '2011-07-26', 'gdodge0@topsy.com');
insert into employee (name, birthday, email) values ('Meade', '1986-04-28', 'mcoton1@google.cn');
insert into employee (name, birthday, email) values ('Leoline', '1955-11-02', 'lburchatt2@amazon.com');
insert into employee (name, birthday, email) values ('Radcliffe', '2012-01-09', 'rgallichan3@columbia.edu');
insert into employee (name, birthday, email) values ('Ozzie', '1992-11-14', 'opeat4@w3.org');
insert into employee (name, birthday, email) values ('Filip', '1966-08-13', 'fcowperthwaite5@moonfruit.com');
insert into employee (name, birthday, email) values ('Horace', '1978-10-18', 'hhadlington6@yandex.ru');
insert into employee (name, birthday, email) values ('Zorah', '2007-05-09', 'zgowanson7@ftc.gov');
insert into employee (name, birthday, email) values ('Alikee', '1968-06-01', 'adaniau8@ibm.com');
insert into employee (name, birthday, email) values ('Rudy', '1981-07-06', 'rwind9@rediff.com');
insert into employee (name, birthday, email) values ('Witty', '2005-06-25', 'wsnowlinga@cbc.ca');
insert into employee (name, birthday, email) values ('Sherwynd', '2004-02-13', 'slimerb@sciencedaily.com');
insert into employee (name, birthday, email) values ('Arabela', '1992-03-13', 'awahnerc@nps.gov');
insert into employee (name, birthday, email) values ('Dusty', '1971-03-17', 'dwardhaughd@amazon.co.uk');
insert into employee (name, birthday, email) values ('Hubert', '2018-04-14', 'hhaineye@wiley.com');
insert into employee (name, birthday, email) values ('Kaine', '1968-11-15', 'krattf@ebay.co.uk');
insert into employee (name, birthday, email) values ('Ignace', '1968-05-20', 'ileythleyg@arstechnica.com');
insert into employee (name, birthday, email) values ('Byrann', '1960-05-15', 'bfiddemanh@rambler.ru');
insert into employee (name, birthday, email) values ('Ingemar', '2006-03-12', 'itrytsmani@icio.us');
insert into employee (name, birthday, email) values ('Sidonnie', '1978-05-29', 'ssteinhammerj@si.edu');
insert into employee (name, birthday, email) values ('Marlena', '2014-07-15', 'mgoldhawkk@unicef.org');
insert into employee (name, birthday, email) values ('Iseabal', '1968-07-21', 'imercyl@blogs.com');
insert into employee (name, birthday, email) values ('Petronella', '1993-08-01', 'pwhatem@reddit.com');
insert into employee (name, birthday, email) values ('Trista', '1973-07-11', 'thirschn@dion.ne.jp');
insert into employee (name, birthday, email) values ('Alisha', '1975-02-27', 'aduckerino@wp.com');
insert into employee (name, birthday, email) values ('Angela', '2019-10-13', 'abuggp@godaddy.com');
insert into employee (name, birthday, email) values ('Griz', '1951-09-23', 'gkuzmaq@reference.com');
insert into employee (name, birthday, email) values ('Darbie', '2001-11-15', 'dberriganr@bloomberg.com');
insert into employee (name, birthday, email) values ('Henrieta', '2007-05-17', 'hgayles@g.co');
insert into employee (name, birthday, email) values ('Kathlin', '1955-05-14', 'kcapnerhurstt@virginia.edu');
insert into employee (name, birthday, email) values ('Ellissa', '1962-04-04', 'evolksu@buzzfeed.com');
insert into employee (name, birthday, email) values ('Brigitta', '1961-08-05', 'bcrawfordv@umn.edu');
insert into employee (name, birthday, email) values ('Kasey', '2000-08-01', 'kchauveyw@mapy.cz');
insert into employee (name, birthday, email) values ('Mitchell', '2000-03-21', 'mceresax@networksolutions.com');
insert into employee (name, birthday, email) values ('Kendell', '2006-02-23', 'kweekleyy@uiuc.edu');
insert into employee (name, birthday, email) values ('Hastie', '1978-07-08', 'hburrowsz@mediafire.com');
insert into employee (name, birthday, email) values ('Kort', '2015-09-24', 'knorthwood10@qq.com');
insert into employee (name, birthday, email) values ('Carine', '1965-11-15', 'cvandevlies11@multiply.com');
insert into employee (name, birthday, email) values ('Aidan', '1965-08-22', 'abezzant12@furl.net');
insert into employee (name, birthday, email) values ('Emelyne', '2002-03-29', 'emorrell13@reuters.com');
insert into employee (name, birthday, email) values ('Elsinore', '1964-06-08', 'ewillmont14@buzzfeed.com');
insert into employee (name, birthday, email) values ('Ada', '2014-04-23', 'agrzelczyk15@jimdo.com');
insert into employee (name, birthday, email) values ('Nealson', '2009-12-09', 'nkells16@mozilla.com');
insert into employee (name, birthday, email) values ('Luelle', '2000-10-04', 'lfleeming17@biblegateway.com');
insert into employee (name, birthday, email) values ('Estrellita', '2016-03-11', 'efewtrell18@house.gov');
insert into employee (name, birthday, email) values ('Ansley', '1991-09-09', 'afassman19@patch.com');
insert into employee (name, birthday, email) values ('Ardenia', '1968-06-15', 'ajoret1a@edublogs.org');
insert into employee (name, birthday, email) values ('Manolo', '1952-01-27', 'mbarwack1b@bandcamp.com');
insert into employee (name, birthday, email) values ('Ilene', '1958-09-14', 'igertz1c@paypal.com');
insert into employee (name, birthday, email) values ('Libbey', '1980-04-27', 'lattenbarrow1d@eventbrite.com');
```

3. Soru
``` SQL
UPDATE employee
SET email = 'random.0323@gmail.com',
	birthday = '1999-11-22'
WHERE name = 'Filip'
RETURNING * ;
``` 
``` sql
UPDATE employee
SET name = 'Ahmet',
	birthday = '1989-09-21'
WHERE email = 'rwind9@rediff.com'
RETURNING * ;
```
``` sql
UPDATE employee
SET name = 'Thomas',
	email = 'random123@gmail.com'
WHERE birthday = '1992-03-13'
RETURNING * ;
```

4. Soru

``` sql
DELETE FROM employee
WHERE name LIKE 'A%'
RETURNING * ;
``` 
``` sql 
DELETE FROM employee
WHERE email ='opeat4@w3.org'
RETURNING * ;
``` 
``` sql 
DELETE FROM employee
WHERE birthday ='1971-03-17'
RETURNING * ;
``` 

``` sql 
DELETE FROM employee
WHERE name ='Thomas'
RETURNING * ;
``` 
``` sql 
DELETE FROM employee
WHERE name  LIKE '%z'
RETURNING * ;
``` 