# Отчет по Курсовой Работе

University: [ITMO University](https://itmo.ru/ru/)\
Faculty: FTMI\
Course: [introduction-in-web-tech](https://itmo-ict-faculty.github.io/introduction-in-web-tech)\
Year: 2025/2026\
Group: U4225\
Author: Laptev Anatoly Aleksandrovich\
Lab: Курсовая работа\
Date of create: 12.10.2025\
Date of finished: 13.10.2025

0. Задеплоеный вариант можно посмотреть тут:
https://septemberer.github.io/devops-lab-laptev/

1. Устанавливаем Material for MkDocs\

> pip install mkdocs mkdocs-material
![img.png](img.png)

2. Пулим образ\

> docker pull squidfunk/mkdocs-material
![img_1.png](img_1.png)

3. Создаем пустой проект\

> docker run --rm -it -v %cd%:/docs squidfunk/mkdocs-material new .
![img_2.png](img_2.png)

4. Запустим заготовку\

> docker run --rm -it -p 8000:8000 -v %cd%:/docs squidfunk/mkdocs-material
![img_3.png](img_3.png)
![img_4.png](img_4.png)

5. Наполним своей информацией\
   ![img_5.png](img_5.png)
6. Смотрим что получилось

> docker run --rm -it -p 8000:8000 -v %cd%:/docs squidfunk/mkdocs-material

- Главная страница\
  ![img_6.png](img_6.png)
- Странички на вкладке\
  ![img_7.png](img_7.png)
  ![img_8.png](img_8.png)
  ![img_9.png](img_9.png)
- Другая вкладка\
  ![img_10.png](img_10.png)
- Темная тема\
  ![img_11.png](img_11.png)
- Копирайт и ссылка на Гитхаб\
  ![img_12.png](img_12.png)
- Еще ссылка на Гитхаб\
  ![img_13.png](img_13.png)
- Фича поиска\
  ![img_14.png](img_14.png)

#

------------------------------