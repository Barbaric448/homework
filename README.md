# Лабораторная работа
Данная лабораторная работа основываеся на работе с планировщиком задач `cron`
# Пример
Допустим, нам нужно сделать так, чтобы некоторая команда выполнялась бесконечно с каким-то промежутком. Тогда в терминале мы напишем:
```
crontb -e
```
А затем:
```
* * * * * echo "hello world!"
```
Комада будет выполняться кажду минуту.
При открытии системного журнала..
```
cat /var/log/syslog
```
видим это:
![image](https://github.com/user-attachments/assets/a0b4838d-ff59-429f-922e-21cbec899558)
Значит, все работает как надо.
# Задания
**1.** Используя cron, автоматизировать выполнение скрипта для проверки свободного места на диске и записи полученных данных в `disk_usage.log` каждые 5 минут.

**2.** Автоматизируйте скрипт, проверяющий доступность какого-либо сервера каждые полчаса (кроме выходных). Запись логов в `server_ping.log`.

# Источники
1. [Источник, где можно найти все](https://www.google.com/)
   
