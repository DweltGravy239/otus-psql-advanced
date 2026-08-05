Построение кластера Patroni 
Создадим 3 виртульных машины etcd и patroni:
<img width="872" height="712" alt="image" src="https://github.com/user-attachments/assets/336e469e-1322-4f55-8c92-2c0f57c023c6" />
Развернем кворум etcd (действия будут показаны только для 1 машинки, но они будут дублироваться на остальные):
Устанавливаем etcd:
<img width="2762" height="794" alt="image" src="https://github.com/user-attachments/assets/f2b4fda2-b67a-4c08-a04c-c337b7d0896c" />
Произведем базовые настройки для первой ноды:
<img width="1404" height="570" alt="image" src="https://github.com/user-attachments/assets/603280ef-9c21-499e-994d-c02061dfb787" />
Запустим etcd:
<img width="2526" height="940" alt="image" src="https://github.com/user-attachments/assets/3e976e87-fe7b-466b-bcad-ce95bfacd1c9" />
Проверим его работоспособность:
<img width="2474" height="1010" alt="image" src="https://github.com/user-attachments/assets/e5e15a76-d92d-4d89-a923-ab24d3c2ac3a" />
Настроим конфиг для первой ноды:
<img width="1391" height="567" alt="image" src="https://github.com/user-attachments/assets/042e051d-d384-4cd8-a043-6706a9612448" />
Создадим кворум:
<img width="1912" height="357" alt="image" src="https://github.com/user-attachments/assets/8d8ba0b4-7796-45ce-91e1-a3a46ba67572" />
Теперь приступим к настройке patroni
Установим postgresql:
<img width="2700" height="858" alt="image" src="https://github.com/user-attachments/assets/8453f02d-c7b7-4199-a55b-041d08e8306f" />
Произведем базовые настройки(создадим пользователя для репликации, отредактируем доступные подключения и прослушиваемые адреса):
<img width="1731" height="229" alt="image" src="https://github.com/user-attachments/assets/1a718afa-afd1-4c98-bfdd-4a40a21996f1" />
<img width="1606" height="522" alt="image" src="https://github.com/user-attachments/assets/7a347b59-65b4-4ab4-934f-7cacb6e7f36d" />
<img width="1801" height="916" alt="image" src="https://github.com/user-attachments/assets/3c2a9950-ea6f-4059-bc03-ce76e8eaedad" />
<img width="1354" height="150" alt="image" src="https://github.com/user-attachments/assets/ef5b6aa5-d7e6-4705-977b-2bb64af6d487" />
Настроим patroni:
Установим patroni:
<img width="2582" height="906" alt="image" src="https://github.com/user-attachments/assets/85fca132-8a5a-4ca4-8172-d5e24dd07dd2" />
<img width="2280" height="732" alt="image" src="https://github.com/user-attachments/assets/80409962-5eb9-4a50-8b9a-3580cbba91ed" />
Настраиваем patroni:
<img width="686" height="1292" alt="image" src="https://github.com/user-attachments/assets/ef791509-b696-4112-a0e6-0d531b496dc5" />
Настраиваем patroni как сервис:
<img width="1892" height="538" alt="image" src="https://github.com/user-attachments/assets/f334d5fd-5302-4153-8cff-49884e9b1f37" />
Запустим patroni и проверим его:
<img width="2880" height="1302" alt="image" src="https://github.com/user-attachments/assets/efa255da-420a-45d5-b4d3-c551c7434b96" />
Создаем кластер patroni:
<img width="1650" height="448" alt="image" src="https://github.com/user-attachments/assets/7bdd5dae-e8aa-4c9f-9b9d-a084b28568a4" />
Устанавливаем и настраиваем HaProxy:


