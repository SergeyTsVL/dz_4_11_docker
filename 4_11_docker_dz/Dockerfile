# Используем официальный образ Nginx
FROM nginx:alpine

# Копируем HTML файл в нужную директорию
COPY index.html /usr/share/nginx/html/index.html

# Копируем конфигурацию Nginx
COPY default.conf /etc/nginx/conf.d/default.conf

RUN apk update && apk add --no-cache curl

# Открываем порт 80
EXPOSE 80 