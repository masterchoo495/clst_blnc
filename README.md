# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки»

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

### Решение

Запуск двух simple python серверов на моей виртуальной машине на разных портах
![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/001.png)  

![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/002.png)  

Демонстрация направления запросов на разные серверы при обращении к HAProxy  
![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/003.png)

[haproxy.cfg](https://github.com/masterchoo495/clst_blnc/blob/main/haproxy.cfg)


### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

### Решение

Запуск двух simple python серверов на моей виртуальной машине на разных портах  
![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/004.png)  

![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/005.png)  

![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/006.png)  

Демонстрация направления запросов на разные серверы при обращении к HAProxy    
![alt text](https://github.com/masterchoo495/clst_blnc/blob/main/007.png)  

[haproxy2.cfg](https://github.com/masterchoo495/clst_blnc/blob/main/haproxy2.cfg)  

---

------
