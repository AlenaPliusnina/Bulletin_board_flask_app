# Bulletin board / Доска объявлений

     Flask, MongoDB, Redis, Docker
     
Описание:
     
     Bulletin board - это Flask приложение, представляющее собой доску объявлений. Для хранения данных использована 
     NoSQL база данных MongoDB, а также реализовано кэширование объявлений при помощи Redis.


Разворачиваем проект локально:

1. Скачайте репозиторий

2. Перейдите в деректорию с ним и в терминале/командной строке запустите:

       docker-compose build

3. Приложение будет запущено по адресу: http://0.0.0.0:5000/

Описание функционала:

1. по пути '/' - отображаются все размещенные объявления, если их нет выводится соответствующее сообщение

   ![There are not posts](/screenshots/screenshot_1.png)
   ![All posts](/screenshots/screenshot_2.png)

 2. В меню есть поле для поиска определенного объявления по его ID:
   
   ![Search field](/screenshots/screenshot_3.png)
   ![Get post by id](/screenshots/screenshot_4.png)
 
 3. по пути '/add_post' отображается форма для создания нового объявления, где поля title, message, author являются обязательными для заполнения.
 
   ![Get post by id](/screenshots/screenshot_5.png)
 
 4. На главной странице у каждого объявления есть также:
 
    - ссылки для добавления комментариев (Leave comment) и (Add tag) тегов к нему
    
    ![Leave comment](/screenshots/screenshot_6.png)
    ![Add tag](/screenshots/screenshot_7.png)
 
    - статистика для данного объявления: сколько у него тегов и комментариев
