# OpenTelemetry

Набор сервисов для организации наблюдаемости вашего проекта.

- запускаются Loki, Mimir, Tempo, Grafana и Otel collector
- создаются datasource в Grafana

## Запуск

```bash
docker compose up -d
```

## Сервисы

| Сервис         | Адреса                                      |
|----------------|---------------------------------------------|
| Grafana        | http://localhost:3000 (admin/admin)         |
| Otel collector | http://localhost:4317 http://localhost:4318 |