# Catworks ID

Доступ к сервисам Catworks управляется ID сервисом, хранящим данные о пользователях и их 
правах доступа. Взаимодействие осуществляется по следующей схеме:
![Схема взаимодействия](res/id_seq.svg)

Области доступа (scopes) ограничивают доступ к определенным функциям и данным.

ID сервис:

- Хранит информацию о пользователях, в т.ч. и доступные им области доступа;
- Предоставляет пользователю авторизовать токен с необходимыми областями доступа;
- Позволяет проверить действительность токена.

## Области доступа по умолчанию

- id.self

## Перечень областей доступа

### ID сервис

| Ключ      | Описание                                |
|-----------|-----------------------------------------|
| id.all    | Любые действия в рамках сервиса         |
| id.list   | Чтение любых существующих пользователей |
| id.invite | Приглашение пользователей               |
| id.self   | Любые действия с самим собой            |
