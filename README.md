# -ODEV3-SQL
dvdrental sorgu senaryolarının çözümleri
Sorgu 1- country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.
Çözüm 1- SELECT country FROM country
WHERE country LIKE 'A%a';
<img width="455" alt="Ekran Resmi 2023-03-01 18 37 48" src="https://user-images.githubusercontent.com/116847744/222187819-646e6e24-9d74-4dcd-a9e4-4f37d8326b48.png">

Sorgu 2- country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
Çözüm 2- SELECT country FROM country
WHERE country LIKE '%_____n';
<img width="468" alt="Ekran Resmi 2023-03-01 18 40 17" src="https://user-images.githubusercontent.com/116847744/222188517-cd0c81c5-9ed9-4389-8df3-2305cc0e1af0.png">

Sorgu 3- film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
Çözüm 3-SELECT title FROM film
WHERE title ILIKE ('%t%t%t%t');
<img width="469" alt="Ekran Resmi 2023-03-01 18 45 24" src="https://user-images.githubusercontent.com/116847744/222189922-69edf49b-c568-418d-900d-3fc0e387d724.png">

Sorgu 4-film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.
Çözüm 4-SELECT * FROM film
WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;
<img width="731" alt="Ekran Resmi 2023-03-01 18 50 52" src="https://user-images.githubusercontent.com/116847744/222191319-e4ee15c5-8599-4309-891f-d3eba3814706.png">
