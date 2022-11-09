University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)

Year: 2022/2023

Group: K34202

Author: Tasmaev Igor Aleksandrovich

Lab: Lab1

Date of create: 20.10.2022

Date of finished: 

#### Цель: 
развернуть виртуальную машину на базе платформы Яндекс Облако с установленной системой контроля конфигураций Ansible и установка CHR в VirtualBox
#### Ход работы: 
1. Создана виртуальная машина на Яндекс Облаке. На виртуальную машину установлены python3 и Ansible.  
<img width="1042" alt="Screen Shot 2022-10-25 at 21 10 08" src="https://user-images.githubusercontent.com/63468028/200915186-0d526d12-7a7e-4c47-bc5e-237a0098cc92.png">

2. Создана виртуальная машина CHR на Яндекс Облаке.
Так как прав на отключение фаервола на моем устройстве у меня нет, а фаервол блочит все входящие icmp пакеты, было решено использовать в качестве Яндекс Облако как сервис виртуализации.
<img width="559" alt="Screen Shot 2022-10-25 at 21 11 46" src="https://user-images.githubusercontent.com/63468028/200915384-c71c2538-f272-42d4-b5df-4a1c961ee43f.png">

3. Так как Яндекс Облако предоставляет в готовых образах только 6 версию CHR, а я уже настроился использовать wireguard, версию пришлось обновить до 7.
<img width="174" alt="Screen Shot 2022-10-25 at 21 16 55" src="https://user-images.githubusercontent.com/63468028/200915473-0e545db2-07b6-4e96-9292-f2c0539466ba.png">

4. Установлен Wireguard. Сгенерированы приватные и публичные ключи сервера и клиента. Выполнена настройка конфигурации сервера.
<img width="444" alt="Screen Shot 2022-10-25 at 21 22 30" src="https://user-images.githubusercontent.com/63468028/200915578-394a9822-6eac-4717-94c7-8fe765f44d7f.png">

5. Выполнена настройка Wireguard клиента на CHR машине
<img width="458" alt="Screen Shot 2022-10-25 at 21 24 17" src="https://user-images.githubusercontent.com/63468028/200915662-e18545ef-b88f-4f9c-9ba3-cd341bc2e54c.png">
<img width="413" alt="Screen Shot 2022-10-25 at 21 24 54" src="https://user-images.githubusercontent.com/63468028/200915770-45d5fdaa-fdef-4006-92e3-fa3b3cb09466.png">

6. Интерфейсу присвоен IP адрес
<img width="425" alt="Screen Shot 2022-10-25 at 21 25 45" src="https://user-images.githubusercontent.com/63468028/200915823-91a00842-0f03-4301-a133-e2e064230414.png">

7. Запустил сервер и проверил соединение
<img width="438" alt="Screen Shot 2022-10-25 at 21 28 55" src="https://user-images.githubusercontent.com/63468028/200916085-b1153ba5-8a64-4524-93ea-fd86aeda66e8.png">
<img width="541" alt="Screen Shot 2022-10-25 at 21 30 53" src="https://user-images.githubusercontent.com/63468028/200916093-8d5af729-9cb5-4925-8716-5d9edf15de4b.png">

#### Вывод:

В ходе выполнения лабораторной работы были созданы две виртуальные машины, одна на Ubuntu другая на CHR Router Os. После чего между ними был создан VPN туннель с использованием Wireguard. Протестирована работа туннеля.

