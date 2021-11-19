**19.11.2021**

```
cp .env.dist .env
docker-compose -f ./docker-compose.yml up -d
```
либо
```
docker-compose -f ./docker-compose.yml --env-file ./.env.dist up -d
```

Контейнер слушает порт 8080. Получить версию php можно вот так
```
curl -I http://127.0.0.1:8080/phpinfo.php | grep X-Powered-By
```

