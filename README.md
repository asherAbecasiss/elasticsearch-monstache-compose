

run 
```
  docker-compose up
```


mongo config 


```
docker exec to mongo ~$ > mongo
MongoDB shell version: 2.6.9
connecting to: test
> rs.initiate()
> cfg = rs.conf()
> cfg.members[0].host = "mongodb:27017"
> rs.reconfig(cfg)
> rs.status();

```



