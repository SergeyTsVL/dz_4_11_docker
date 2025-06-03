Порядок выдачи команд по очереди

Заходим в командную строку Ubuntu

git clone <Адрес репозитория на гитхабе>                       - Копируем репозиторий

docker build -f ./Dockerfile -t go-api:latest .                - создаем образ контенера

docker ps

docker ps -a

docker images

docker run --name go-api-demo -d go-api                        - Запускаем контейнер по образу
                                            
docker exec -it <ID контейнера> sh -c "cd /usr/share/nginx/html && curl http://localhost/index.html"