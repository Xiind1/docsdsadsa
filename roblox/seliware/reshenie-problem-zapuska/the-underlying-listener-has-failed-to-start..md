# The underlying listener has failed to start.

1. Откройте командную строку администратора \
   (Чтобы открыть от имени администратора: откройте поиск, введите "CMD", щелкните правой кнопкой мыши "Командная строка" и выберите "Запуск от имени администратора") \
   и выполните эту команду:

```
powershell -Command "Get-NetTCPConnection -LocalPort 3000 -LocalAddress 127.0.0.1 -State Listen | ForEach-Object { Stop-Process -Id $_.OwningProcess -Force }"
```

2. Перезапустите Seliware и нажмите "Load"
