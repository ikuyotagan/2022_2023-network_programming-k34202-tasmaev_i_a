University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Network programming](https://github.com/itmo-ict-faculty/network-programming)

Year: 2022/2023

Group: K34202

Author: Tasmaev Igor Tasmaev

Lab: Lab4

Date of create: 04.12.2022

Date of finished: 

#### Цель работы
Изучить синтаксис языка программирования P4 и выполнить 2 задания обучающих задания от Open network foundation для ознакомления на практике с P4.

#### Ход работы

С помощью Vagrant создана ВМ P4 Tutorial Release 2022-12-04.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.17.49.png">
Выполнена превичная конфигурация сети "Basic Forwarding" с помощью Makefile, а также проверена связь хостов через Ping.Связь отсутствует.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.29.22.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.31.08.png">
Отредактирован файл basic.p4 для правильной кофигурации сети.
Добавлен парсинг ethernet и ipv4 headers.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.36.54.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.38.16.png">
Добавлена валидация хэдеров.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.40.04.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.41.09.png">
Добавлена логика форвардинга ipv4 пакетов.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.41.51.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.42.19.png">
Добавлен депарсинг ethernet и ipv4 headers.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.43.14.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.43.40.png">
Заново сконфигурирована сеть с помошью Makefile и исправленного basic.p4, проверена связь хостов через ping и pingall.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.44.50.png">
Отредактирован файл basic_tunnel.p4 для правильной кофигурации сети "Basic Tunneling".
Добавлен парсинг хэдеров myTunnel.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.51.37.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.59.47.png">
Добавлена логика форвардинга myTunnel пакетов, таблица myTunnel_exact для связи логики пересылки и header dst_id и валидация хэдеров myTunnel.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.52.35.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.53.46.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.55.05.png">
Добавлен депарсинг хэдеров myTunnel.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.55.59.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 22.56.19.png">

Сконфигурирована сеть с помошью Makefile и исправленного basic_tunnel.p4, проверена связь хостов через ping и pingall.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.01.49.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.02.04.png">
Проверена работа сети через программы receive.py и send.py хостов, а также работа туннелирования, используя параметр dst_id.
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.17.52.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.19.10.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.20.01.png">
<img alt="image" src="screens/Screen Shot 2022-12-04 at 23.20.26.png">
Схемы сетей:

<img alt="image" src="https://github.com/p4lang/tutorials/blob/master/exercises/basic/pod-topo/pod-topo.png">

<img alt="image" src="https://github.com/p4lang/tutorials/blob/master/exercises/basic_tunnel/topo.png">

#### Вывод:
В ходе выполнения лабораторной работы была создана виртуальная машина для работы с P4. Был изучен синтаксис языка программирования P4 и выполнены 2 обучающих задания от для ознакомления с P4 на практике.