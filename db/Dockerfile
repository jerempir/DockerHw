# db/Dockerfile
FROM python:3.9-slim

WORKDIR /data

# Установка SQLite
RUN apt-get update && apt-get install -y sqlite3 && rm -rf /var/lib/apt/lists/*

# Создание БД
COPY init.sql /data/init.sql
RUN sqlite3 mydb.sqlite < init.sql

# Установка точки входа
CMD ["sqlite3", "mydb.sqlite"]
