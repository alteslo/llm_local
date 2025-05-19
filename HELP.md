# Docker
## Поднять контейнер
`docker compose up -d`
## Остановить и удалить контейнер
`docker compose down`
## Запустить контейнер
`docker compose start`
## Остановить контейнер
`docker compose stop`

docker compose -f docker-compose.base.yml up -d
docker compose -f docker-compose.base.yml -f docker-compose.ui.yml up -d
docker compose -f docker-compose.base.yml -f docker-compose.ui.yml -f docker-compose.metrics.yml up -d
## Перезапустить контейнер
docker compose restart ollama



## Зайти в контейнер
docker exec -it ollama /bin/bash

# Ollama
## Скачать модель
`docker exec -it ollama ollama pull llama2`
## Запустить интерактивный режим
`docker exec -it ollama ollama run llama2 "Привет! Как дела?"`
## Удалить модель
`docker exec -it ollama ollama rm llama2`
## Вывести список моделей
`docker exec -it ollama ollama ls`
## Вывести список процессов
`docker exec -it ollama ollama ps`