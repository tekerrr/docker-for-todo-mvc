# Docker for [todo-mvc](https://github.com/tekerrr/todo-mvc)
## Порядок установки
Склонировать данный репозиторий
    
    git clone https://github.com/tekerrr/docker-for-todo-mvc.git

Перейти в директорию "docker-for-todo-mvc/www" и склонировать резоторий [todo-mvc](https://github.com/tekerrr/todo-mvc)

    cd docker-for-todo-mvc/www
    
    git clone https://github.com/tekerrr/todo-mvc.git
    
Перейти в директорию "todo-mvc" и загрузить зависомости с помощью composer

    cd todo-mvc
    
    composer install

...

...

...

Запустить docker

    docker-compose up
    
Запусть проект по ссылке

    todo-mvc:42080/
