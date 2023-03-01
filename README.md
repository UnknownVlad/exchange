# Биржа

### Описание задания
Требовалось разработать **RESTfull API service** — биржу для проведения торгов криптовалютами.

Из дополнительных заданий было выполнено подключение к базе данных `PostgreSQL` для хранения данных о балансе пользовательских кошельков и истории операций.

### Описание работы приложения
Приложение написано с помощью `Spring` контейнеров. Базовые запросы принимаются в формате `json` и в этом же формате сервис возвращает данные. Классы с именем **DAO** играют роль sql-запросника. 

### REST-запросы, реализованные в приложении
Для удобства **REST-запросы** отправлялись в приложении **Postman**
* Регистрация нового пользователя.  


    POST запрос  
![img.png](img.png)  

      Ответ
![img_1.png](img_1.png)  


    Запрос с уже существующим пользователем
![img_2.png](img_2.png)

      Ответ
![img_3.png](img_3.png)

* Просмотр баланса своего кошелька.


    GET запрос  
![img_4.png](img_4.png)!

      Ответ
![img_5.png](img_5.png)

* Пополнение кошелька.
    

    POST запрос  
![img_6.png](img_6.png)

    Ответ
![img_7.png](img_7.png)

* Посмотреть общую сумму на всех пользовательских счетах для указанной валюты (от имени админа).


    GET запрос   
![img_8.png](img_8.png)
    
    Ответ
![img_9.png](img_9.png)

* Посмотреть общую сумму на всех пользовательских счетах для указанной валюты (от имени пользователя).


    GET запрос     
![img_10.png](img_10.png)
    
    Ответ
![img_11.png](img_11.png)

* Вывод денег с биржи.


    POST запрос  
![img_12.png](img_12.png)
    
    Ответ
![img_13.png](img_13.png)

* Просмотр актуальных курсов валют (данный запрос будет доступен и пользователю и администратору).


    GET запрос  
![img_14.png](img_14.png)

    Ответ
![img_15.png](img_15.png)

* Изменить курс валют.


    POST запрос  
![img_16.png](img_16.png)
    
    Ответ
![img_17.png](img_17.png)
