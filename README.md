
# Лабораторная работа 4.

Для начала я написал в Dockerfile следующий код
```
FROM ubuntu:latest

RUN apt-get update && apt-get install -y libaa-bin && apt-get install -y iputils-ping
```

Затем создал образ с помощью команды
```
docker build -t aafire1 .
```

Создал два контейнера с помощью команды 
```
docker run -it aafire1
```

Запустил в интерактивном режиме aafire
![image](https://github.com/user-attachments/assets/b3b9ee41-7e55-42b1-884a-06a13f201067)

Организовал соединение между контейнерами
![image](https://github.com/user-attachments/assets/0603e690-7b63-4d0d-a887-4d3230741e0e)
