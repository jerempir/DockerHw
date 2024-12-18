# Проект с двумя контейнерами: SQLite и клиент

## Запуск контейнеров

1. Собрать и запустить контейнеры:
   ```bash
   docker-compose up --build

2. Второй контейнер (app_entry) должен показать данные из SQLite:
   Database rows:
   (1, 'Alice', 'alice@example.com')
   (2, 'Bob', 'bob@example.com')
   Можно запустить команду docker logs app_entry в другом терминале

3. Остановка контейнеров:
docker-compose down

4. Повторный запуск не удаляет данные в БД:
docker-compose up