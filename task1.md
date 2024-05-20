Задание 1

Цель практической работы:
Научиться выполнять простые запросы в Redis.

Напишите последовательность команд для Redis:

Создайте ключ index со значением “index precalculated content”.
127.0.0.1:6379> set index index_precalculated_content ex 60

OK

Проверьте, есть ли ключ index в БД.
127.0.0.1:6379> exists index

(integer) 1

OK

Узнайте, сколько ещё времени будет существовать ключ index.
127.0.0.1:6379> ttl index

(integer) 56

127.0.0.1:6379> ttl index

(integer) 52

127.0.0.1:6379> ttl index

(integer) 50

127.0.0.1:6379> ttl index

(integer) 47

Отмените запланированное удаление ключа index.
127.0.0.1:6379> persist index

(integer) 1

Узнайте, сколько ещё времени будет существовать ключ index.
127.0.0.1:6379> ttl index

(integer) -1

127.0.0.1:6379> 

