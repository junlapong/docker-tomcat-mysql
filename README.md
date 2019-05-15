# Docker Tomcat MySQL

## Docker Compose

```
# start
docker-compose up -d

# view logs
docker-compose logs

# stop
docker-compose down
```

## Tomcat
 - http://localhost:9080/example-webapp/

## MySQL

```
docker exec -it docker-tomcat-mysql_db_1 /bin/bash
mysql -u root -p

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| example_db         |
| information_schema |
| ...                |
+--------------------+
```

### MySQL data
 - map volumes to local directory `./db/data`
