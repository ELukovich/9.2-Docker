## Сборка образа

docker build . --tag smarthome:0.1

## Запуск контейнера

docker run --name my-smarthome -d -p 8000:8000 smarthome:0.1