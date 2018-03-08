## get all keys 
 > KEYS
## remove all keys
 > FLUSHALL
## hash table operation
Hash table likes an object, it can be set multiple values in one key.
For example, a person named zhangsan, we can set his age, gender and so on.
 > HSET zhangsan age 30 gender mail
 > HGET zhangsan age 

## queue
 Redis can be used like simple message queue
 > RPUSH mylist 'one'
 > RPUSH mylist 'two'
 > RPOP mylist
