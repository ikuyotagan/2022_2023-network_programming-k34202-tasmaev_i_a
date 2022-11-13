University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)

Year: 2022/2023

Group: K34202

Author: Tasmaev Igor Tasmaev

Lab: Lab2

Date of create: 13.11.2022

Date of finished: 

#### Цель работы:
С помощью Ansible настроить несколько сетевых устройств и собрать информацию о них. Правильно собрать файл Inventory.

#### Ход работы:
Установлен второй CHR на своем yandex cloud. Обновлен до версии 7.5. Настроен Wireshark клиент на втором CHR, установлено соединение с впн сервером Wireshark. 

<img width="436" alt="image" src="https://user-images.githubusercontent.com/63468028/201539803-c95a3c7d-89d7-4ee6-b781-63a54732a204.png">

Используя Ansible, создан новый юзер, а также настроен NTP клиент сразу на 2-х CHR:
<img width="520" alt="image" src="https://user-images.githubusercontent.com/63468028/201540136-fab8ca06-0cf4-49b9-9899-914d152ae280.png">

Поскольку плеи уже были запущены ранее, часть неидемпотентных команд возвращают ошибки.
<img width="833" alt="image" src="https://user-images.githubusercontent.com/63468028/201540689-89037c1f-0d84-4dba-8f59-5dc075afa724.png">

Настроен OSPF на двух CHR. Информация о соединении между соседями выведена в файлы json формата.
<img width="650" alt="image" src="https://user-images.githubusercontent.com/63468028/201541194-4c2989af-91f9-4d29-8323-2da250cc55de.png">

<img width="810" alt="image" src="https://user-images.githubusercontent.com/63468028/201541405-415089b0-7086-4db2-8ed2-47ab5178372f.png">

<img width="1792" alt="image" src="https://user-images.githubusercontent.com/63468028/201542582-6e2cd4ba-1018-47ba-a2e8-dcbe8bead735.png">


Собраны данные по OSPF топологии и полный конфиг устройства.
<img width="676" alt="image" src="https://user-images.githubusercontent.com/63468028/201545661-d0fe54df-7f45-46e6-a3fc-adff40679c5d.png">

<img width="1792" alt="image" src="https://user-images.githubusercontent.com/63468028/201545631-f02c8c73-7ec5-429c-9d0b-a48a844e4562.png">

Выполнена проверка связности устройств

<img width="548" alt="image" src="https://user-images.githubusercontent.com/63468028/201545737-8591446f-7f9e-4567-9c2d-5b73e9b65ccb.png">
<img width="575" alt="image" src="https://user-images.githubusercontent.com/63468028/201545763-f82bcdc1-f010-4071-aa3a-239a6f7ff3dc.png">

![Диаграмма без названия drawio](https://user-images.githubusercontent.com/63468028/201546331-75ef79fa-f7b5-4851-9852-c5077a0c57a4.svg)

Вывод:
В ходе выполнения лабораторной работы был создан еще один CHR. После чего удаленно были проведена настройка CHR с помощью Ansible, установленного на удаленной ВМ, находящейся в Yandex Cloud.
