# Домашнее задание к занятию "`Система мониторинга Zabbix. Часть 2`" - `Стрекозов Владимир`

### Задание 1
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z1.PNG)
### Задание 2-3
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z2-3.PNG)
### Задание 4
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z4%20dashboard.PNG)
## Дополнительные задания (со звездочкой*)
### Задание 5
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z5%20map.PNG)
### Задание 6
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z6.PNG)
### код скрипта
```python
import sys
import os
import re
if (sys.argv[1] == '1'):
        result="Strekozov Vladimir Aleksandrovich"
        print(result)
elif (sys.argv[1] == '2'):
        result=os.popen("date").read()
        print(result)
else:
        print(f"unknown input: {sys.argv[1]}")
```
### Задание 7
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z7.PNG)
### код скрипта
```python
import sys
import os
import re
if (sys.argv[1] == '1'):
        result="Strekozov Vladimir Aleksandrovich"
        print(result)
elif (sys.argv[1] == '2'):
        result=os.popen("date").read()
        print(result)
elif (sys.argv[1] == '-ping'):
        result=os.popen("ping -c 1 " + sys.argv[2]).read()
        result=re.findall(r"time=(.*) ms", result)
        print(result[0])
elif (sys.argv[1] == '-simple_print'):
        print(sys.argv[2])
else:
        print(f"unknown input: {sys.argv[1]}")
```
### Задание 8
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z8_actions.PNG)
![alt text](https://github.com/Svalker1989/hw-03/blob/main/Z8_discovery.PNG)

