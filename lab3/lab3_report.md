# Отчет по лабораторной №3

University: [ITMO University](https://itmo.ru/ru/)\
Faculty: FTMI\
Course: [introduction-in-web-tech](https://itmo-ict-faculty.github.io/introduction-in-web-tech)\
Year: 2025/2026\
Group: U4225\
Author: Laptev Anatoly Aleksandrovich\
Lab: Lab3\
Date of create: 05.10.2025\
Date of finished: 

1) Создание конфигурации Prometheus:
* Создать папку prometheus для конфигурации
* Создать файл prometheus/prometheus.yml
![img.png](img.png)
2) Запуск Node Exporter:
* Запустить контейнер Node Exporter для сбора системных метрик:
![img_1.png](img_1.png)
* Проверить работу: curl http://localhost:9100/metrics
![img_2.png](img_2.png)
3) Запуск Prometheus:
* Создать том для данных Prometheus:
![img_3.png](img_3.png)
* Запустить контейнер Prometheus:
![img_5.png](img_5.png)
* Проверить работу: открыть http://localhost:9090 в браузере
![img_11.png](img_11.png)
4) Запуск Grafana:
* Создать том для данных Grafana:
![img_6.png](img_6.png)
* Запустить контейнер Grafana:
![img_7.png](img_7.png)
* Проверить работу: открыть http://localhost:3000 в браузере (логин: admin, пароль: admin)
![img_8.png](img_8.png)
5) Настройка Grafana:
* Войти в Grafana (admin/admin)
* Добавить источник данных Prometheus
![img_9.png](img_9.png)
* Создать дашборд:
![img_12.png](img_12.png)
5.1) На самом деле если до этого момента все делать по методичке то ничего не работает, потому что
все эти сервисы находятся в разных контейнерах и не могут связываться друг с другом. 
* Для решения этого понадобилось создать сетевую связанность 
![img_13.png](img_13.png)
6) Тестирование системы:
* Проверить все контейнеры: docker ps
![img_14.png](img_14.png)
* Открыть Prometheus и убедиться, что метрики собираются
![img_15.png](img_15.png)
* Открыть Grafana и проверить отображение графиков
![img_16.png](img_16.png)
* Создать несколько графиков для разных метрик (CPU, память, диск)
![img_17.png](img_17.png)