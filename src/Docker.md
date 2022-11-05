## Part 1. Готовый докер

##### Взять официальный докер образ с **nginx** и выкачать его при помощи `docker pull`

![simple_docker](./img/1_1.png)nginx pull

##### Проверить наличие докер образа через docker images

![simple_docker](./img/1_2.png)docker images

##### Запустить докер образ через docker run -d [image_id|repository]

![simple_docker](./img/1_3.png)docker run

##### Проверить, что образ запустился через docker ps

![simple_docker](./img/1_4.png)docker ps

##### Посмотреть информацию о контейнере через docker inspect [container_id|container_name]
![simple_docker](./img/1_5.png)container size
![simple_docker](./img/1_6.png)ports
![simple_docker](./img/1_7.png)container ip


##### Остановить докер образ через docker stop

![simple_docker](./img/1_8.png)docker stop

##### Проверить, что образ остановился через docker ps

![simple_docker](./img/1_9.png)docker ps


##### Запустить докер с замапленными портами 80 и 443 на локальную машину через команду run

![simple_docker](./img/1_10.png)docker run mapping

##### Проверить, что в браузере по адресу localhost:80 доступна стартовая страница nginx

![simple_docker](./img/1_11.png)browser

##### Перезапустить докер контейнер через docker restart [container_id|container_name]s

![simple_docker](./img/1_12.png)docker restart

##### Проверить любым способом, что контейнер запустился

![simple_docker](./img/1_13.png)docker ps

## Part 2. Операции с контейнером

##### Прочитать конфигурационный файл nginx.conf внутри докер контейнера через команду exec
![simple_docker](./img/2_1.png)nginx conf

##### Создать на локальной машине файл nginx.conf
![simple_docker](./img/2_2.png)new nginx conf

##### Настроить в нем по пути /status отдачу страницы статуса сервера nginx
![simple_docker](./img/2_3.png)/status

##### Скопировать созданный файл nginx.conf внутрь докер образа через команду docker cp
![simple_docker](./img/2_4.png)docker cp

##### Перезапустить nginx внутри докер образа через команду exec
![simple_docker](./img/2_5.png)restart nginx

##### Проверить, что по адресу localhost:80/status отдается страничка со статусом сервера nginx
![simple_docker](./img/2_6.png)/status

##### Экспортировать контейнер в файл container.tar через команду export

![simple_docker](./img/2_7.png)container.tar

##### Остановить контейнер
![simple_docker](./img/2_8.png)stop

##### Удалить образ через docker rmi [image_id|repository], не удаляя перед этим контейнеры
![simple_docker](./img/2_9.png)rmi force

##### Удалить остановленный контейнер
![simple_docker](./img/2_10.png)delete container

##### Импортировать контейнер обратно через команду import
![simple_docker](./img/2_11.png)import

##### Запустить импортированный контейнер
![simple_docker](./img/2_12.png)run container

##### Проверить, что по адресу localhost:80/status отдается страничка со статусом сервера nginx
![simple_docker](./img/2_13.png)status

## Part 3. Мини веб-сервер


