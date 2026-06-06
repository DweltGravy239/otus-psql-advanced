1. Создадим виртуальные машины
<img width="2880" height="746" alt="image" src="https://github.com/user-attachments/assets/e1ae3662-120f-4257-af99-83e213adb430" />
2. Настроим SSH-доступ
<img width="1002" height="144" alt="image" src="https://github.com/user-attachments/assets/9301dc9d-a733-4ae4-9864-6946f836944b" />
P.S. Ранее доступ уже был пробит, поэтому показываю часть ключ
3. Установить PostgreSQL
<img width="1236" height="296" alt="image" src="https://github.com/user-attachments/assets/5f566d12-4f62-447d-b148-d22bc7d0213b" />
4. Открыть 2 сессии, войти в пользователя postgres и подключиться к PostgreSQL
<img width="2876" height="794" alt="image" src="https://github.com/user-attachments/assets/f2edf21e-5bb7-466f-92fe-d0bb2d7f7d2b" />
5. Выключаем autocommit
<img width="1424" height="442" alt="image" src="https://github.com/user-attachments/assets/754b3def-8618-4156-93bf-843221a6ff5b" />
7. Создает в первой сессии таблицы "Перевозки" и добавляем туда нужные данные
<img width="1424" height="442" alt="image" src="https://github.com/user-attachments/assets/5b18eefa-b90a-435f-9bdb-e6e2b9bb56bf" />
8. Проверяем текущий уровень изоляции
<img width="962" height="290" alt="image" src="https://github.com/user-attachments/assets/0525b413-8ae5-4e3b-a1f8-bcbaa65e8e89" />
9. Начнем транзацию в двух сессиях
<img width="2666" height="1510" alt="image" src="https://github.com/user-attachments/assets/15a3923a-8636-4b5d-86b0-24929d55add4" />
10. Добавим новую строчку и выполним селект по данной таблице
<img width="2392" height="1022" alt="image" src="https://github.com/user-attachments/assets/46a5c03b-0774-46a5-8244-50c708567da2" />
Мы не увидим обновленную строчку, так как уровень изоляции "Read commited", это значит, что при незавершенной транзакции мы видим только ту инфорамацию, которая была до ее начала.
11. Завершим транзакцию
<img width="2872" height="1432" alt="image" src="https://github.com/user-attachments/assets/c295a42f-438b-4731-ae08-1edff68035f6" />
Как мы видим, после завершения транзакции мы видим изменения в таблице.
12. Поменяем уровень транзакций в двух сессиях
<img width="2630" height="158" alt="image" src="https://github.com/user-attachments/assets/d61cc0bc-c1d8-4c3e-9202-7f830d485b4d" />
13. В первой сессии добавляем новую запись и проверяем таблицу
<img width="2306" height="358" alt="image" src="https://github.com/user-attachments/assets/78a4261a-0224-43dc-8bcf-333b83a32e50" />
Таблица при выводе не изменилась, так как мы повысили уровень изоляции, то есть на него стали действовать более строгие правила, учитывая прошлый уровень
14. Завершаем первую транзакцию
<img width="2298" height="328" alt="image" src="https://github.com/user-attachments/assets/c636fe32-d80c-478a-8408-077aa5b06771" />
Мы не видим изменений, так как уровень изоляции "Repeatable read" ставит условие, что транзакция до своего закрытия видит только те данные, которые были у нее в начале
15. Завершаем вторую транзакцию
<img width="2252" height="504" alt="image" src="https://github.com/user-attachments/assets/af6293ff-2f94-4585-b026-433b6c5cdea8" />
Данное действие подтверждает слова выше, теперь мы видим изменения в таблице, тем самым убеждаемся в работоспособности уровней транзакций.


