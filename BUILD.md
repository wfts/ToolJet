## build
```shell
openssl rand -hex 64
```
```
TOOLJET_HOST=http://localhost:8082
LOCKBOX_MASTER_KEY=13c9b8364ae71f714774c82498ba328813069e48d80029bb29f49d0ada5a8e40
SECRET_KEY_BASE=ea85064ed42ad02cfc022e66d8bccf452e3fa1142421cbd7a13592d91a2cbb866d6001060b73a98a65be57e65524357d445efae00a218461088a706decd62dcb
NODE_ENV=development

PG_HOST=postgres
PG_PORT=5432
PG_USER=postgres
PG_PASS=postgres
PG_DB=tooljet_development
ORM_LOGGING=all
```

```shell
docker-compose build
docker-compose run --rm plugins npm run build:plugins
docker-compose up -d
docker-compose exec server npm run db:seed
```

```
email: dev@tooljet.io
password: password
```
