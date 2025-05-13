docker-compose up -d

# Скачать модель
docker exec -it ollama ollama pull llama2
# Запустить инференс
docker exec -it ollama ollama run llama2 "Привет! Как дела?"
# Удалить модель
docker exec -it ollama ollama rm llama2

# Вывести список моделей
docker exec -it ollama ollama ls