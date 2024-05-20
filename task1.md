127.0.0.1:6379> set index index_precalculated_content

OK

127.0.0.1:6379> get index

"index_precalculated_content"

127.0.0.1:6379> exists index

(integer) 1

127.0.0.1:6379> ttl index

(integer) -1

127.0.0.1:6379> 