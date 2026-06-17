# Monitoring Stack test для правки потом под структуру домашнего задания 

Стек мониторинга на базе Prometheus, Node Exporter и Grafana.

## Состав

- Prometheus
- Node Exporter
- Grafana

## Запуск

```bash
docker compose up -d
```

## Проверка

Grafana:

http://<SERVER_IP>:3000

Prometheus:

http://<SERVER_IP>:9090

Node Exporter:

http://<SERVER_IP>:9100/metrics

## Авторизация Grafana

Логин:

admin

Пароль:

admin

## Dashboard

В репозитории присутствует экспортированный Dashboard:

dashboard/node-exporter-dashboard.json

## Alerting

Настроены алерты:

- High CPU Usage
- High Load Average
- Low Free Memory
- Low Disk Space

Уведомления отправляются в Telegram.
