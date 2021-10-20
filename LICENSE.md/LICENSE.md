Найдите номер модели, скорость и размер жесткого диска ПК, имеющих 12x или 24x CD и цену менее 600 дол.
SELECT model,speed, hd FROM pc WHERE (cd='12x'AND price<600) OR (cd='24x' AND price<600)

Для каждого производителя, выпускающего ПК-блокноты c объёмом жесткого диска не менее 10 Гбайт, найти скорости таких ПК-блокнотов. Вывод: производитель, скорость.
SELECT DISTINCT maker, speed FROM product JOIN  laptop ON product.model=laptop.model 
WHERE hd>= 10
