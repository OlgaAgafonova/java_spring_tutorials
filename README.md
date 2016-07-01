# Уроки с сайта http://spring-projects.ru

## Папка ``building RESTful web service``
Создан сервис, который принимает HTTP GET запросы на: 

``http://localhost:8080/greeting``

а ответом будет JSON строка вида: 

``{"id":1,"content":"Hello, World!"}``

Можно модифицировать сообщение ответа, если добавить к строке запроса параметр name:

``http://localhost:8080/greeting?name=User``

Значение параметра ``name`` заменяет значение по умолчанию ``"World"`` и отображается в ответе:

``{"id":1,"content":"Hello, User!"}``

## Папка ``consuming a RESTful web service``

Создано приложение, которое использует Spring RestTemplate для получения случайной фразы из Spring Boot:

``http://gturnquist-quoters.cfapps.io/api/random``

### Заметки
- ``@JsonIgnoreProperties`` - показывает, что любые поля, не связанные с полями класса, должны быть проигнорированы.

