select d.first_name, d.rate  //что выбираем (поля вывода)
from driver d    //сама БД
where d.first_name //где и с какими условиями искать в БД запрос
<> // не равно (!= аналог JS)
=============================
select * (это выбор всех полей) или c.id_car, c.model, c.number, c.odo, c.id_driver
from car c
where c.odo > 100000
order by 1 // sortirovka по возрастанию по первому элементу
order by car.odo (по названию поля)
order by c.odo desc (обратная сортировка по убыв)
=============================
