### ISIS_Lab2
Создать приложение1 на любом языке программирования, сделать Docker образ приложения, запустить приложение

### Инструкция
Склонировать репозиторий
```
git clone https://github.com/shadowHD-bit/ISIS_LAB2.git
```
Создать образ
```
docker build . -t nodejs-docker
```
Запустить образ
```
docker run -p 80:8080 -d nodejs-docker
```
Перейти на локальную страницу
```
localhost:80
```