# Please synchronize your time!

1. Откройте командную строку администратора \
   (Чтобы открыть от имени администратора: откройте поиск, введите "CMD", щелкните правой кнопкой мыши "Командная строка" и выберите "Запуск от имени администратора") \
   и выполните эту команду:

```
sc config w32time start= auto & net start w32time & w32tm /config /manualpeerlist:time.google.com /syncfromflags:manual /update & w32tm /resync /rediscover
```

2. Перезапустите Seliware и нажмите "Load"
