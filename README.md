# Лабораторная работа №7
## Цель работы
* Ознакомиться с работой многоконтейнерного приложения на базе docker-compose.
### Создайте файл .gitignore в корне проекта и добавьте в него строки:
![1ю](https://github.com/Iulia1511/containers06/assets/159126852/5f6a80ef-4dc1-4cdc-9026-44eb7a742998)
### Создайте в директории containers06 файл nginx/default.conf со следующим содержимым:
![2ю](https://github.com/Iulia1511/containers06/assets/159126852/02bb4bff-450c-4d48-b682-ac2943db26b9)
### Создайте в директории containers06 файл docker-compose.yml со следующим содержимым:
![3ю](https://github.com/Iulia1511/containers06/assets/159126852/032ab947-4678-4391-8825-ed1925cc21b3)
### Создайте файл mysql.env в корне проекта и добавьте в него строки:
![4ю](https://github.com/Iulia1511/containers06/assets/159126852/f6c7e01c-2a84-42e3-878b-5a27662f1771)
### Cозданные папки:

![image](https://github.com/Iulia1511/containers06/assets/159126852/a9914dd9-5ad9-4fb5-a827-d04c2971527f)

### Запустите контейнеры командой: docker-compose up -d
![5ю](https://github.com/Iulia1511/containers06/assets/159126852/d26f9145-1a8a-45e2-b0f3-915507310129)
### Открылся мой сайт php
![6ю](https://github.com/Iulia1511/containers06/assets/159126852/9a17a85c-438c-4fa6-9b46-8fb964a026af)
## Ответы на вопросы:
* 1.В данном случае, сначала запускается контейнер базы данных (database), затем контейнеры backend и frontend.
* 2.Данные базы данных хранятся в томе Docker, который называется db_data, как указано в файле docker-compose.yml. Этот том привязан к директории /var/lib/mysql в контейнере базы данных.
* 3.Контейнеры проекта называются frontend, backend и database
* 4.Вам необходимо добавить еще один файл app.env с переменной окружения APP_VERSION для сервисов backend и frontend. Как это сделать?
![8ю](https://github.com/Iulia1511/containers06/assets/159126852/596971d6-08ce-4927-ab54-f583c68fe99c)
![9ю](https://github.com/Iulia1511/containers06/assets/159126852/ee138c25-fb29-4eda-ba6f-c2e002af8f05)
# Вывод
* Я ознакомилась с работой многоконтейнерного приложения на базе docker-compose.
