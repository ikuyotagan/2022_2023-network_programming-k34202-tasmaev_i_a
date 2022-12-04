University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)

Year: 2022/2023

Group: K34202

Author: Tasmaev Igor Tasmaev

Lab: Lab2

Date of create: 04.12.2022

Date of finished: 

#### Цель работы:
С помощью Ansible и Netbox собрать всю возможную информацию об устройствах и сохранить их в отдельном файле.

#### Ход работы:
Поднят нетбокс на новой виртуальной машине.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 18.06.49.png">

В нетбоксе заполнена основная информация о двух роутерах.

При помощи сценария ansible выгружена информация о роутерах.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 19.12.02.png">

<img alt="image" src="screens/Screen Shot 2022-12-04 at 19.11.38.png">

При помощи другого сценария изменено имя роутера и задан новый IP адрес.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 20.09.33.png">

<img alt="image" src="screens/Screen Shot 2022-12-04 at 20.09.13.png">

Серийные номера роутеров занесены в netbox.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 20.23.26.png">

<img alt="image" src="screens/Screen Shot 2022-12-04 at 20.23.08.png">

![Диаграмма без названия drawio (1)](https://user-images.githubusercontent.com/63468028/205507868-d1b9ab0e-dd78-4a7f-9a83-0635d8b9c3cf.svg)

#### Вывод:

В ходе выполнения лабораторной работы была создана еще одна виртуальная машина с netbox. После чего были проведены настройки обоих CHR, а также настройка Netbox с помощью информации взятой из CHR.
