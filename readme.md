# Docker for [todo-mvc](https://github.com/tekerrr/todo-mvc)
## Порядок установки
Клонировать данный репозиторий
    
    git clone https://github.com/tekerrr/docker-for-todo-mvc.git

Клонировать репозиторий [todo-mvc](https://github.com/tekerrr/todo-mvc)

    cd docker-for-todo-mvc/www    
    git clone https://github.com/tekerrr/todo-mvc.git
    
Загрузить зависимости с помощью composer

    cd todo-mvc    
    composer install

...

...

...

Запустить docker

    docker-compose up

Мигрировать БД

    docker-compose exec php bash
    php todo-mvc/database/migrate.php
    exit
    
Запустить проект по ссылке

    todo-mvc:42080/
