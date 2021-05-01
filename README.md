# graphQL_movies_app
## https://eloquent-haibt-76a4e0.netlify.app/
## Стак: GraphQL, React, Material-UI, Apollo Client, Mongoose

Приложение для просмотра режиссеров и их фильмов.
Идея такая: сделана БД на cloud.mongodb.com, в ней две коллекции документов:
1. Movies, для фильмов
2. Directors, для режиссеров
Документы в Directors связаны с документами из Movies как "один ко многим".

Бэкенд написан на GraphQL, схемы запросов лежат в `server\schema`.
Модели документов для Mongoose лежат в `server\models`.
"Общение" сервера с клиентом происходит с помощью Apollo Client. 
Все запросы и мутации лежат в папках с компонентами, попадают в компонент через HOC-и.
На проекте реализован CRUD:
- Режиссеры и фильмы добавляются (POST)
- Они редактируются (UPDATE)
- Они удаляются (DELETE)
- Они запрашиваются в список (GET)
- Плюс есть поиск по имеющимся элементам

Фронт выложен на Netlify
Бек выложен на Heroku
...это не очень логично, но хотелось поработать с Netlify :)

Информация о режиссерах и фильмах честно украдена с Вики.
Оценки выставлены от балды и не отображают реальности.
