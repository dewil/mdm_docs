# Настройка VPN
version 2022-04-24
## Описание

Подключив VPN соединение вы попадаете в локальную сеть предприятия.

Для доступа к внутренним ресурсам необходимо вручную ввести протокол и адрес нужного ресурса, например http://10.0.0.1/

Если ваша локальная сеть, до подключения к VPN тоже начинается на 10.\*, а не на 192.168.\*, то возможны сложности с доступом к локальной сети предприятия. В этом случае обратитесь за консультацией к системному администратору.

## Настройка WinXP
![](img/vpn/Pasted%20image%2020220424120155.png)

![](img/vpn/Pasted%20image%2020220424121521.png)

![](img/vpn/Pasted%20image%2020220424122314.png)

![](img/vpn/Pasted%20image%2020220424122328.png)

![](img/vpn/Pasted%20image%2020220424122338.png)

![](img/vpn/Pasted%20image%2020220424122347.png)

![](img/vpn/Pasted%20image%2020220424122357.png)

![](img/vpn/Pasted%20image%2020220424122413.png)

![](img/vpn/Pasted%20image%2020220424122423.png)

После этого окна, в Trey должна появиться иконка и подсказка, что соединение установлено.

Добавление маршрута, если у вас ip 192.168.222.6

Вызвать cmd и там набрать команду:

```
route add 10.0.0.0 mask 255.0.0.0 192.168.222.6
```

## Настройка Win10
![](img/vpn/Pasted%20image%2020220424123116.png)

![](img/vpn/Pasted%20image%2020220424123127.png)


>  С 29.03.2020 можно использовать два протокола: PPTP или L2TP

Лучше первый, если с ним проблема, попробуйте второй.

![](img/vpn/Pasted%20image%2020220424123243.png)

![](img/vpn/Pasted%20image%2020220424123257.png)

![](img/vpn/Pasted%20image%2020220424123307.png)

Для проверки соединения можно в командной строке набрать например,
```
ping 10.0.0.61
```