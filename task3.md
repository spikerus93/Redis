Задание 3

Цель практической работы:
Научиться работать с механизмом Pub/Sub в Redis.

Напишите две команды для СУБД Redis:

Подпишитесь на все события, опубликованные на каналах, начинающихся с events.
127.0.0.1:6379> psubscribe events*

Reading messages... (press Ctrl-C to quit)

1) "psubscribe"

2) "events*"

3) (integer) 1

1) "pmessage"

2) "events*"

3) "events101"

4) "Hello there."

_____________________

Опубликуйте сообщение на канале events101 с текстом: 
“Hello there”.

127.0.0.1:6379> publish events101 "Hello there."

(integer) 1

127.0.0.1:6379> 


