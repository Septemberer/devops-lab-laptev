# Отчет по лабораторной №1

University: [ITMO University](https://itmo.ru/ru/)\
Faculty: FTMI\
Course: [introduction-in-web-tech](https://itmo-ict-faculty.github.io/introduction-in-web-tech)\
Year: 2025/2026\
Group: U4225\
Author: Laptev Anatoly Aleksandrovich\
Lab: Lab1\
Date of create: 29.09.2025\
Date of finished: 29.09.2025

1) docker --version\
![img.png](img.png)
2) docker run hello-world
![img_1.png](img_1.png)
3) docker images, docker ps, docker ps -a
![img_2.png](img_2.png)
![img_3.png](img_3.png)
![img_4.png](img_4.png)
4) docker pull ubuntu:latest
![img_5.png](img_5.png)
5) docker run -it ubuntu bash
![img_6.png](img_6.png)
6) apt update && apt install -y curl
![img_7.png](img_7.png)
7) curl --version
![img_8.png](img_8.png)
8) exit\
![img_9.png](img_9.png)
9) docker run -d -p 8080:80 --name web-server nginx:alpine
![img_10.png](img_10.png)
10) http://localhost:8080
![img_11.png](img_11.png)
11) docker logs web-server
![img_12.png](img_12.png)
12) docker exec -it web-server sh
![img_13.png](img_13.png)
13) docker ps | docker ps -a | docker stop web-server
![img_14.png](img_14.png)
14) docker start web-server
![img_15.png](img_15.png)
15) docker rm web-server | docker rmi nginx:alpine
![img_16.png](img_16.png)
16) docker volume create my-volume
![img_17.png](img_17.png)
17) docker run -d -v my-volume:/data --name volume-test ubuntu
![img_18.png](img_18.png)
18) docker exec -it volume-test bash
![img_19.png](img_19.png)
19) Создать файл в томе: echo "Hello from volume" > /data/test.txt
![img_20.png](img_20.png)