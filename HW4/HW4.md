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


