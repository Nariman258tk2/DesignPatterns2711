# DesignPatterns2711
Lab1
ДЗ- 1) Применить к иерархии File System паттерн Singleton. 2) Применить к иерархии 2 любой паттерн фабрик (или все сразу)

Lab2
Дополнить класс ConnectionPoolGrowLimit из проекта patterns_demo следующим функциональном:
1) Сделать pool с "восстановлением размера". Т.е. pool растет до определенного лимита (например с 10ти исходных ресурсов до 20ти). 
Но при снижении нагрузки (т.е. при возврате в pool более чем 70% соединений) удаляет лишние добавленные ресурсы (т.е. уменьшает свой размер с 20ти обратно до 10ти)
2) Добавить запрет использования ресурса из pool-а по ссылке, после того как он был возвращен в pool.

Lab3
Дополнить иерархию Composite следующей логикой:
1) Каждый MenuItem может состоять из комбинации других MenuItem и/или продуктов
2) Каждый продукт имеет каллорийность
3) Добавить логику расчета каллорийности всего меню

Lab4
Добавить в пакете proxy.homework новый прокси со следующей функциональностью:
1) Фильтрация ответа UserRepo метода getAll() с пользователями только старше 18 лет
2) Фильтрация параметров метода changeUsers с пользователями с ролью не "admin@"

Lab5
Имитировать работу SpringFilterChain с использованием паттерна "Цепочка обязанностей". Описание работы по ссылке- https://docs.spring.io/spring-security/site/docs/3.0.x/reference/security-filter-chain.html в п.7.3.

Lab6
В иерархию banking из примеров паттерна Command добавить следующую функциональность
1) Добавить операцию перевода счета в другую валюту
2) Реализовать корректную отмену данной операции

Lab7
В иерархию statecommandupgr добавить следующий функционал:
1) Добавить отмену операций с возвратом в нужное состояние.
2) Добавить операцию добавления контента в документ. Доступно только в состоянии New.

Lab8
В иерархии memento добавить следующий функционал:
1) Добавить в TextEditor понятие курсора. Курсор устанавливается в конкретную позицию текста- оттуда теперь происходит вставка/удаление текста
2) Добавить операцию redo, которая отменяет операцию undo
3) Дополнительно- объединить этот паттерн с паттерном команда. Ответить для себя- применим ли в этом кейсе паттерн "Состояние"
