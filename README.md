# DockerWithPythonFlask

https://docs.docker.com/language/python/

```
docker run --rm -d -v mysql:/var/lib/mysql \
  -v mysql_config:/etc/mysql -p 3306:3306 \
  --network mysqlnet \
  --name mysqldb \
  -e MYSQL_ROOT_PASSWORD=p@ssw0rd1 \
  mysql
```

``` 
docker-compose -f docker-compose.dev.yml up --build
```

```
curl http://localhost:8000/initdb
curl http://localhost:8000/widgets
```
