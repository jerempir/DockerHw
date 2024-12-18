# app/Dockerfile
FROM python:3.9-slim

WORKDIR /app

# Устанавливаем зависимости
RUN pip install requests

COPY main.py /app/main.py

CMD ["python", "main.py"]
