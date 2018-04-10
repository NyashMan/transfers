**cd**
-
root@git:/etc/gitlab# cd

**pwd**
-
root@git:~# pwd
/root

**ls**
-
root@git:~# ls -lha
итого 36K
drwx------  5 root root 4,0K фев 23 23:57 .
drwxr-xr-x 22 root root 4,0K фев 23 00:28 ..
-rw-------  1 root root   39 фев 23 00:29 .bash_history
-rw-r--r--  1 root root  570 янв 31  2010 .bashrc
drwx------  3 root root 4,0K фев 23 01:55 .cache
drwx------  3 root root 4,0K фев 23 01:55 .config
drwx------  3 root root 4,0K фев 23 01:55 .local
-rw-r--r--  1 root root  148 авг 17  2015 .profile
-rw-r--r--  1 root root   72 фев 23 23:57 .selected_editor

**cd to /usr/src/**
-
root@git:~# cd /usr/src/
**mkdir**
-
root@git:/usr/src# mkdir -p transfers/
**rmdir**
-
root@git:/usr/src# rmdir transfers/

root@git:/usr/src# cd transfers/

root@git:/usr/src/transfers# ls

root@git:/usr/src/transfers#

**touch**
-
root@git:/usr/src/transfers# touch test1.txt

root@git:/usr/src/transfers# ls

test1.txt

**rm**
-
root@git:/usr/src/transfers# rm test1.txt 

root@git:/usr/src/transfers# ls

root@git:/usr/src/transfers# touch 1 2 3 4

root@git:/usr/src/transfers# ls

1  2  3  4

root@git:/usr/src/transfers# cd ../
**rm -rf**
-
root@git:/usr/src# rm -rf transfers/

root@git:/usr/src# ls -lha

итого 8,0K

drwxr-xr-x  2 root root 4,0K фев 24 00:40 .

drwxr-xr-x 10 root root 4,0K фев 23 00:25 ..

root@git:/usr/src# echo "file 1" >> file.1

root@git:/usr/src# echo "file 2" >> file.2

**mv**
-
root@git:/usr/src# mv file.2 file.4.mv

root@git:/usr/src# ls

file.1	file.4.mv

**cat**
-
root@git:/usr/src# cat file.1

file 1

root@git:/usr/src# cat file.4.mv 

file 2
**cp**
-
root@git:/usr/src# cp file.4.mv file.44

root@git:/usr/src# ls -lha

итого 20K

drwxr-xr-x  2 root root 4,0K фев 24 00:42 .

drwxr-xr-x 10 root root 4,0K фев 23 00:25 ..

-rw-r--r--  1 root root    7 фев 24 00:41 file.1

-rw-r--r--  1 root root    7 фев 24 00:42 file.44

-rw-r--r--  1 root root    7 фев 24 00:41 file.4.mv

root@git:/usr/src# cat file.44 

file 2

**apt-get update**
-
root@git:/usr/src# apt-get update

Пол:1 http://security.debian.org/debian-security stretch/updates InRelease [63,0 kB]

Игн:2 http://deb.debian.org/debian stretch InRelease                                                        

Пол:3 http://deb.debian.org/debian stretch-updates InRelease [91,0 kB]                                      

Сущ:4 http://deb.debian.org/debian stretch Release                                                       

Пол:5 http://security.debian.org/debian-security stretch/updates/main Sources [121 kB]                                    

Пол:6 http://security.debian.org/debian-security stretch/updates/main amd64 Packages [329 kB]                                                   

Пол:7 http://security.debian.org/debian-security stretch/updates/main Translation-en [145 kB]                                                   

Сущ:9 http://nginx.org/packages/mainline/debian stretch InRelease                                                           

Сущ:10 https://packages.gitlab.com/gitlab/gitlab-ce/debian stretch InRelease

Получено 749 kБ за 1с (528 kБ/c)

Чтение списков пакетов… Готово

**apt-get upgrade**
-
root@git:/usr/src# apt-get upgrade

Чтение списков пакетов… Готово

Построение дерева зависимостей       

Чтение информации о состоянии… Готово

Расчёт обновлений… Готово

обновлено 0, установлено 0 новых пакетов, для удаления отмечено 0 пакетов, и 0 пакетов не обновлено.

**apt-get install**
-
root@git:/usr/src# apt-get install **p7zip-full**

Чтение списков пакетов… Готово

Построение дерева зависимостей       

Чтение информации о состоянии… Готово

Будут установлены следующие дополнительные пакеты:
  **p7zip**

Предлагаемые пакеты:
  **p7zip-rar**

НОВЫЕ пакеты, которые будут установлены:
  **p7zip p7zip-full**

обновлено 0, установлено 2 новых пакетов, для удаления отмечено 0 пакетов, и 0 пакетов не обновлено.

Необходимо скачать **1 479 kБ** архивов.

После данной операции, объём занятого дискового пространства возрастёт на 5 469 kB.

Хотите продолжить? [Д/н] 

Пол:1 http://security.debian.org/debian-security stretch/updates/main amd64 p7zip amd64 16.02+dfsg-3+deb9u1 [364 kB]

Пол:2 http://security.debian.org/debian-security stretch/updates/main amd64 p7zip-full amd64 16.02+dfsg-3+deb9u1 [1 115 kB]

Получено 1 479 kБ за 0с (6 566 kБ/c)    

Выбор ранее не выбранного пакета p7zip.
(Чтение базы данных … на данный момент установлено 135074 файла и каталога.)

Подготовка к распаковке …/p7zip_16.02+dfsg-3+deb9u1_amd64.deb …

Распаковывается p7zip (16.02+dfsg-3+deb9u1) …

Выбор ранее не выбранного пакета p7zip-full.

Подготовка к распаковке …/p7zip-full_16.02+dfsg-3+deb9u1_amd64.deb …

Распаковывается p7zip-full (16.02+dfsg-3+deb9u1) …

Настраивается пакет p7zip (16.02+dfsg-3+deb9u1) …

Обрабатываются триггеры для man-db (2.7.6.1-2) …

Настраивается пакет p7zip-full (16.02+dfsg-3+deb9u1) …

**apt-get remove**
-
root@git:/usr/src# apt-get remove nginx

Чтение списков пакетов… Готово

Построение дерева зависимостей       

Чтение информации о состоянии… Готово

Пакеты, которые будут УДАЛЕНЫ:

**nginx**

обновлено 0, установлено 0 новых пакетов, для удаления отмечено 1 пакетов, и 0 пакетов не обновлено.

После данной операции, объём занятого дискового пространства уменьшится на 2 871 kB.

Хотите продолжить? [Д/н] 

(Чтение базы данных … на данный момент установлено 135172 файла и каталога.)
Удаляется nginx (1.13.9-1~stretch) …

Обрабатываются триггеры для man-db (2.7.6.1-2) …

root@git:/usr/src# **apt-get install htop  iftop nload iotop**

Чтение списков пакетов… Готово

Построение дерева зависимостей       

Чтение информации о состоянии… Готово

Предлагаемые пакеты:
  strace

НОВЫЕ пакеты, которые будут установлены:
  htop iftop iotop nload

обновлено 0, установлено 4 новых пакетов, для удаления отмечено 0 пакетов, и 0 пакетов не обновлено.
Необходимо скачать 214 kБ архивов.

После данной операции, объём занятого дискового пространства возрастёт на 574 kB.

Пол:1 http://deb.debian.org/debian stretch/main amd64 htop amd64 2.0.2-1 [88,2 kB]

Пол:2 http://deb.debian.org/debian stretch/main amd64 iftop amd64 1.0~pre4-4 [41,4 kB]

Пол:3 http://deb.debian.org/debian stretch/main amd64 iotop amd64 0.6-2 [30,4 kB]

Пол:4 http://deb.debian.org/debian stretch/main amd64 nload amd64 0.7.4-1+b2 [54,0 kB]

Получено 214 kБ за 0с (3 622 kБ/c)         

Выбор ранее не выбранного пакета htop.
(Чтение базы данных … на данный момент установлено 135154 файла и каталога.)

Подготовка к распаковке …/htop_2.0.2-1_amd64.deb …
Распаковывается htop (2.0.2-1) …

Выбор ранее не выбранного пакета iftop.
Подготовка к распаковке …/iftop_1.0~pre4-4_amd64.deb …
Распаковывается iftop (1.0~pre4-4) …

Выбор ранее не выбранного пакета iotop.
Подготовка к распаковке …/archives/iotop_0.6-2_amd64.deb …
Распаковывается iotop (0.6-2) …

Выбор ранее не выбранного пакета nload.
Подготовка к распаковке …/nload_0.7.4-1+b2_amd64.deb …
Распаковывается nload (0.7.4-1+b2) …
Настраивается пакет nload (0.7.4-1+b2) …

Обрабатываются триггеры для mime-support (3.60) …

Настраивается пакет iftop (1.0~pre4-4) …

Настраивается пакет iotop (0.6-2) …

Обрабатываются триггеры для man-db (2.7.6.1-2) …

Настраивается пакет htop (2.0.2-1) …

**man**
-
root@git:/usr/src# **man mv >> /tmp/man.mv**

**swap and mem info**
-
root@git:/usr/src# **free -h**

**              total        used        free      shared  buff/cache   available**

**Mem:           3,9G        2,4G        186M         64M        1,2G        1,0G**

**Swap:          4,0G         12K        4,0G**

root@git:/usr/src# 
** space info**
-
root@git:/usr/src# **df -h**

Файловая система Размер Использовано  Дост Использовано% Cмонтировано в

udev               2,0G            0  2,0G            0% /dev

tmpfs              396M         5,4M  391M            2% /run

/dev/sda1           28G         3,3G   23G           13% /

tmpfs              2,0G         4,0K  2,0G            1% /dev/shm

tmpfs              5,0M            0  5,0M            0% /run/lock

tmpfs              2,0G            0  2,0G            0% /sys/fs/cgroup

tmpfs              396M            0  396M            0% /run/user/0

tmpfs              396M            0  396M            0% /run/user/1000

**ping**
-
root@git:/usr/src# **ping -c 5 ya.ru**

PING ya.ru (87.250.250.242) 56(84) bytes of data.

64 bytes from ya.ru (87.250.250.242): icmp_seq=1 ttl=49 time=38.7 ms

64 bytes from ya.ru (87.250.250.242): icmp_seq=2 ttl=49 time=38.8 ms

64 bytes from ya.ru (87.250.250.242): icmp_seq=3 ttl=49 time=38.6 ms

64 bytes from ya.ru (87.250.250.242): icmp_seq=4 ttl=49 time=39.1 ms

64 bytes from ya.ru (87.250.250.242): icmp_seq=5 ttl=49 time=38.9 ms

--- ya.ru ping statistics ---

*5 packets transmitted, 5 received, 0% packet loss, time 4005ms*

*rtt min/avg/max/mdev = 38.676/38.854/39.118/0.266 ms*

**kernel loaded modules**
-

root@git:/usr/src# lsmod | more

Module                  Size  Used by

cfg80211              589824  0

nfnetlink_queue        24576  0

nfnetlink_log          20480  0

nfnetlink              16384  2 nfnetlink_log,nfnetlink_queue

bluetooth             552960  0

rfkill                 24576  3 bluetooth,cfg80211

bochs_drm              20480  1

hid_generic            16384  0

ttm                    98304  1 bochs_drm

drm_kms_helper        155648  1 bochs_drm

sg                     32768  0

shpchp                 36864  0

virtio_balloon         16384  0

drm                   360448  4 bochs_drm,ttm,drm_kms_helper

pcspkr                 16384  0

joydev                 20480  0

evdev                  24576  1

serio_raw              16384  0

button                 16384  0

usbhid                 53248  0

hid                   122880  2 hid_generic,usbhid

ip_tables              24576  0

x_tables               36864  1 ip_tables

autofs4                40960  2

ext4                  585728  1

crc16                  16384  2 bluetooth,ext4

*...........................................*
**show network settings**
-
root@git:/usr/src# **ifconfig -a**

*ens18*: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500

        inet 192.168.1.120  netmask 255.255.255.0  broadcast 192.168.1.255

        inet6 fe80::9cb1:5aff:fe5e:ec0  prefixlen 64  scopeid 0x20<link>

        ether 9e:b1:5a:5e:0e:c0  txqueuelen 1000  (Ethernet)

        RX packets 125139  bytes 585992432 (558.8 MiB)

        RX errors 0  dropped 0  overruns 0  frame 0

        TX packets 68256  bytes 7971949 (7.6 MiB)

        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

*lo*: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536

        inet 127.0.0.1  netmask 255.0.0.0

        inet6 ::1  prefixlen 128  scopeid 0x10<host>

        loop  txqueuelen 1  (Local Loopback)

        RX packets 30014  bytes 26384710 (25.1 MiB)

        RX errors 0  dropped 0  overruns 0  frame 0

        TX packets 30014  bytes 26384710 (25.1 MiB)

        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

