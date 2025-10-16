# Инфраструктура локальной разработки

Описание инфраструктуры.

## Сервисы

Конфигурация сервисов находится в папке `services`.

| Сервис         | Описание                                       | Test                                        |
|----------------|------------------------------------------------|---------------------------------------------|
| Grafana        | Просмотр логов                                 | http://localhost:3000 (admin/admin)         |
| OTEL коллектор | Телеметрия приложения (трейсы, логи и метрики) | http://localhost:4317 http://localhost:4318 |
| PostgresSQL    | База данных для приложений                     | localhost:5432                              |


## Запуск

Создайте сеть:

```bash
docker network create --attachable local-infra
```

Создайте `.env` файл в корне:

```
POSTGRES_USER=admin
POSTGRES_PASSWORD=adminpassword
```

Запустите:

```bash
docker compose up -d
```