# Docker for [todo-mvc](https://github.com/tekerrr/todo-mvc)
## Порядок установки
Клонировать данный репозиторий
    
    git clone https://github.com/tekerrr/docker-for-todo-mvc.git

Клонировать репозиторий [todo-mvc](https://github.com/tekerrr/todo-mvc)

    cd docker-for-todo-mvc/www/
    git clone https://github.com/tekerrr/todo-mvc.git
    
Загрузить зависимости с помощью composer

    cd todo-mvc/    
    composer install

Запустить docker

    cd ../../
    docker-compose up -d

Мигрировать БД

    docker-compose exec php bash
    php todo-mvc/database/migrate.php
    exit
    
Добавить редирект в host

    127.0.0.1 todo-mvc.local
    
Запустить проект по ссылке

    http://todo-mvc.local:42080/
