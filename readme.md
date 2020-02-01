# Docker for [todo-mvc](https://github.com/tekerrr/todo-mvc)
## Порядок установки
Склонировать данный репозиторий
    
    git clone https://github.com/tekerrr/docker-for-todo-mvc.git

Склонировать репозиторий [todo-mvc](https://github.com/tekerrr/todo-mvc)

    cd docker-for-todo-mvc/www    
    git clone https://github.com/tekerrr/todo-mvc.git
    
Загрузить зависомости с помощью composer

    cd todo-mvc    
    composer install

...

...

...

Мигрировать БД

    docker-compose exec php bash
    php todo-mvc/database/migrate.php
    exit

Запустить docker

    docker-compose up
    
Запусть проект по ссылке

    todo-mvc:42080/
