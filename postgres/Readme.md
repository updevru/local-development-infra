# PostgresSQL

Запуск базы данных PostgresSQL.

## Запуск

Создайте `.env` файл в корне:

```
POSTGRES_USER=admin
POSTGRES_PASSWORD=adminpassword
```

```bash
docker compose up -d
```

## Сервисы

| Сервис      | Адреса         |
|-------------|----------------|
| PostgresSQL | localhost:5432 |