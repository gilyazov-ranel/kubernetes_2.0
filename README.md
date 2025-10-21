### Задание 1. Создать сетевую политику или несколько политик для обеспечения доступа

1. Создать deployment'ы приложений frontend, backend и cache и соответсвующие сервисы.
2. В качестве образа использовать network-multitool.
3. Разместить поды в namespace App.
4. Создать политики, чтобы обеспечить доступ frontend -> backend -> cache. Другие виды подключений должны быть запрещены.
5. Продемонстрировать, что трафик разрешён и запрещён.
### Ответ
Применяем deployment'ы и политики
<img width="1185" height="463" alt="image" src="https://github.com/user-attachments/assets/1346d068-876d-4f4e-aab0-d9b59d6207a4" />
Проверяем поды, сервисы, сетевые политики
<img width="1472" height="397" alt="image" src="https://github.com/user-attachments/assets/30217170-5eef-4a76-89c4-8d46992d1661" />
#### Тестируем
Frontend → Backend
<img width="1477" height="256" alt="image" src="https://github.com/user-attachments/assets/b4527c0e-67a6-4931-9919-ba74ac7bb3e4" />
Backend → Cache
<img width="1475" height="269" alt="image" src="https://github.com/user-attachments/assets/90750f1c-ad3d-4f2b-ad2b-b56a15111189" />
Frontend → Cache
<img width="1453" height="191" alt="image" src="https://github.com/user-attachments/assets/070dcb21-3a49-4e5e-92e9-38746d274495" />
Backend → Frontend
<img width="1472" height="177" alt="image" src="https://github.com/user-attachments/assets/54096ab3-dd33-46db-bfb6-734ebc866d1a" />
Cache → Backend
<img width="1464" height="203" alt="image" src="https://github.com/user-attachments/assets/041cbeff-90e3-4b5d-ae88-8b90dff85c19" />
Внешние подключения
<img width="1450" height="114" alt="image" src="https://github.com/user-attachments/assets/6a32c36c-9f26-46fb-9a31-362dc73438fb" />
Проверка DNS
<img width="1353" height="298" alt="image" src="https://github.com/user-attachments/assets/1e42cf1f-6bb4-4620-b18d-c6b871f85404" />
