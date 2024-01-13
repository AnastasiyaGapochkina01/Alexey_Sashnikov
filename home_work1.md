1) В домашнем каталоге создать каталог inform_фамилия (фамилия латиницей).
2) Перейти в каталог inform_фамилия создать в нем каталог lab1
3) Внутри каталога lab1 создать каталог catalog1, файл file1, каталог catalog2. Перейти в каталог catalog2.
4) Внутри каталога catalog2 создать файлы file3 и file4, каталог catalog3
5) Внутри каталога catalog3 создать файл file5, жесткую ссылку на файл file1
6) Создать в каталоге lab1 символическую ссылку s_link на файл file5
7) Вывести полученную структуру каталогов командой tree
8) В каталоге lab1 создать директорию files
9) Перейти в каталог files, создать в нем 10 файлов file1.txt, file2.txt, file3.txt ... file10.txt (идеальное решение в одну команду)
10) Скопировать всю директорию files в files2
11) Удалить файлы file2.txt, file3.txt и file5.txt в директории files2
12) Скопировать файлы file2.txt, file3.txt и file5.txt из директории files в директорию files2
13) Переименовать ВСЕ файлы в директории files2 из file(1,2,3...).txt в text_file_(1,2,3...).txt
14) Удалить директорию files
15) Переименовать директорию files2 в text_files
16) Удалить директорию text_files
17) В директории lab1 создать пустой файл output
18) Перенаправить вывод команды tree -a ~/inform_фамилия в файл output
19) По умолчанию ls сортирует вывод по алфавиту. Отсортировать вывод команды ls по
- размеру файла
- по времени модификации файла и перенаправить в файл output (ДОПИСАТЬ в него, а не ПЕРЕзаписать)
20) Посмотреть первые шесть записей любого лога из /var/log
21) Посмотреть последние двадцать записей любого лога из /var/log
22) С помощью cat, grep и cut вывести id (3 поле в строке) пользователя www-data (если такого пользователя нет, то выбрать любого существующего пользователя и выполнить задание для него)
23) С помощью grep вывести и пронумеровать все строки из /etc/passwd, где встречается строка /bin/bash
24) Из файла /proc/meminfo выести всю информацию о HugePages (там скорее всего будет всё по нулям, это норма)
25) Из файла /proc/stat высести информацию про softirq
26) Вывести участников группы cdrom (файл /etc/group) пример, группа floppy, участник anestesia
27) Выпонить команду ```ip -o a``` и получить ip машины (нужно получить только ip), то есть
вывод команды такой
```
anestesia@anestesia:~$ ip -o a
1: lo    inet 127.0.0.1/8 scope host lo\       valid_lft forever preferred_lft forever
1: lo    inet6 ::1/128 scope host noprefixroute \       valid_lft forever preferred_lft forever
2: wlo1    inet 192.168.0.70/24 brd 192.168.0.255 scope global dynamic noprefixroute wlo1\       valid_lft 6207sec preferred_lft 6207sec
2: wlo1    inet6 fe80::a5b:d6ff:fe18:e8e0/64 scope link noprefixroute \       valid_lft forever preferred_lft forever
anestesia@anestesia:~$
```
из него надо выкусить 192.168.0.70
