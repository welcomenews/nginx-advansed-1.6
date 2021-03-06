# nginx-advansed-1.6

```
Задача
Цель домашнего задания
В этом модуле мы рассмотрели особенности YAML-языка, узнали, что такое балансировка и балансировщики нагрузки и как с помощью cherry-pick можно легко перемещать отдельные коммиты в Git. 

Вам предстоит закрепить полученные знания, самостоятельно написать YAML-файл и настроить обратный прокси-сервер.

Что входит в задание
* Переписать JSON-файл на YAML.
* Настроить обратный прокси-сервер на базе nginx.

Задание 1. Переписать JSON-файл на YAML

Что нужно сделать
В прикреплённых материалах найдите файл в формате JSON (to_yaml.json). Перепишите файл в YAML-формат.
В прикреплённых материалах найдите файл в формате YAML (builds.yaml). В файле описана сборка трёх docker-образов. Оптимизируйте описание, используя переменные YAML.

Задание 2. Настроить обратный прокси-сервер на базе nginx

Что нужно сделать
К вам приходят разработчики и просят настроить сервер, который будет перенаправлять запросы на их внутренний сервер на базе Gunicorn, который находится на адресе 127.0.0.1:8888. При этом разработчики просят сделать ещё несколько манипуляций:

* путь /static/ должен вести к папке /opt/venv/site/static;
* для всех запросов, кроме /static/*, нужно добавить header с ключом CST_HEADER и значением с названием текущего сервера;
* все запросы, начинающиеся с пути /admin/, должны быть переадресованы на корень сайта, и только те запросы, в которых присутствует header с ключом X_CST_TOKEN, должны вести по запрошенному пути.
```
