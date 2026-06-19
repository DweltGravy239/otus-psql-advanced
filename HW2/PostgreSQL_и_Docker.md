Создайте инстанс с Ubuntu 20.04 в Яндекс.Облаке или аналогах.
<img width="2794" height="1127" alt="image" src="https://github.com/user-attachments/assets/aae065ef-1639-4a04-ac31-0d0a9d0e88ab" />
Данную работу выполнял на виртуальной машине. 

Установите Docker Engine.
<img width="1344" height="405" alt="image" src="https://github.com/user-attachments/assets/1a1c896b-3b40-46da-af76-fdd12848e21c" />
Докер уже был установлен на виртуальной 

Создайте каталог /var/lib/postgres для хранения данных.
<img width="1165" height="134" alt="image" src="https://github.com/user-attachments/assets/25430711-87fd-48bc-b0d9-55ca1b931def" />

Разверните контейнер с PostgreSQL 14, смонтировав в него /var/lib/postgres.
<img width="1775" height="975" alt="image" src="https://github.com/user-attachments/assets/d34ab4a5-0de6-4f51-a173-06a3108e7a1f" />
Развернуть необходимые контейнеры я решил через docker compose.
<img width="2863" height="642" alt="image" src="https://github.com/user-attachments/assets/7f6938ee-190e-4af5-a707-6bcfffaa1956" />
Разверните контейнер с клиентом PostgreSQL.
<img width="2869" height="218" alt="image" src="https://github.com/user-attachments/assets/6510dd87-568c-48ac-b1d7-7eda43a37aea" />
Подключитесь из контейнера с клиентом к контейнеру с сервером и создайте таблицу с данными о перевозках.
<img width="2871" height="455" alt="image" src="https://github.com/user-attachments/assets/f830b172-48fa-4899-92bc-54e68921b364" />
<img width="2013" height="882" alt="image" src="https://github.com/user-attachments/assets/7e75eeeb-f6c6-4f29-8f1f-2f05055745f7" />
<img width="863" height="613" alt="image" src="https://github.com/user-attachments/assets/3925539e-2705-433a-b678-8b57bf64fe13" />
Подключитесь к контейнеру с сервером с ноутбука или компьютера.
<img width="2847" height="955" alt="image" src="https://github.com/user-attachments/assets/78b2d877-79fd-40f5-999c-1012715eb49e" />
Удалите контейнер с сервером и создайте его заново.
<img width="1509" height="1036" alt="image" src="https://github.com/user-attachments/assets/78e643a8-35de-4058-9f69-c5f9d7d4fdc3" />
<img width="2867" height="1090" alt="image" src="https://github.com/user-attachments/assets/1c9324f3-3ecd-4219-82fb-eaa980269469" />
Проверьте, что данные остались на месте.
<img width="2844" height="1337" alt="image" src="https://github.com/user-attachments/assets/6447e12f-e097-43f6-b0f2-e99f8d0a527a" />

