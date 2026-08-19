Установим инстанс PostgreSQL:
<img width="2671" height="749" alt="image" src="https://github.com/user-attachments/assets/1ebd28eb-27ab-4941-b030-ef90fdf4086c" />
Создадим базу данных для тестирования:
<img width="1453" height="187" alt="image" src="https://github.com/user-attachments/assets/6112ef02-dfa8-42d6-8ce8-931c635ca55e" />
Скачаем pgbench и сделаем тестирование:
<img width="2401" height="1260" alt="image" src="https://github.com/user-attachments/assets/58273e47-5a1d-49c5-a3a0-100c63ee5403" />
Опитимизируем настройки(опираясь на лекцию):
Настраиваем transparent_hugepage:
<img width="2414" height="656" alt="image" src="https://github.com/user-attachments/assets/17d8d1ca-4c6a-4508-a750-8c3f5084e4f1" />
Настраиваем swappiness:
<img width="1074" height="358" alt="image" src="https://github.com/user-attachments/assets/1fdac4e9-11a9-46f8-ad65-cdf561621232" />
Настраиваем postgresql.conf:
<img width="1311" height="1207" alt="image" src="https://github.com/user-attachments/assets/e4ad33be-285d-44e3-aff3-149e98cad835" />
Перезагружаем конфигурации:
<img width="833" height="348" alt="image" src="https://github.com/user-attachments/assets/09ba81cc-498d-4b94-94e3-6b98803e3113" />

Попробуем еще раз проверить через pgbench:
<img width="1141" height="710" alt="image" src="https://github.com/user-attachments/assets/feef8549-bad3-4101-b4d2-7d736f8d29bc" />
Теперь обратимся на специализированный сайт и попробуем настроить согласно их рекомендациям:
<img width="2852" height="1450" alt="image" src="https://github.com/user-attachments/assets/14e9bc7e-a9f9-4dfa-bf56-aa972abacb4d" />
Настроим согласно рекомендациям:
<img width="1203" height="1095" alt="image" src="https://github.com/user-attachments/assets/078959f3-9c19-4558-a094-3ed0d54c3b5a" />
Проверим еще раз через pgbench:
<img width="1242" height="854" alt="image" src="https://github.com/user-attachments/assets/d8a5418e-01a3-4573-96a6-3221578c13e7" />
Делаем вывод, 3 прогон самый лучший. 
