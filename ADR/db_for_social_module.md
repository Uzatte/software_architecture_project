### Выбор базы данных для социального модуля

**Статус:**
Предложено

**Контекст:**

Необходимо выбрать тип базы данных для социального модуля

**Решение:**
Использовать документоориентированную базу данных

**Последствия:**

Сущности пользователя, групп, сообщений и т.д. слишком разнородные, где каждый объект может иметь разные наборы атрибутов. Использование реляционной БД может стать проблематичной и приведет к очень сильной связанности через внешние ключи.
В документоориентированной БД каждую сущность можно хранить в виде JSON файла, что делает ее гибкой и удобной