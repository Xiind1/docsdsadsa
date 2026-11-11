# Failed to load. Please restart the app.

1. Откройте командную строку администратора \
   (Чтобы открыть от имени администратора: откройте поиск, введите "CMD", щелкните правой кнопкой мыши "Командная строка" и выберите "Запуск от имени администратора") \
   и выполните эту команду:

```
taskkill /F /IM RobloxPlayerBeta.exe 2>nul & reg add "HKLM\SOFTWARE\Seliware" /v "Version" /t REG_SZ /d "0" /f & if exist "%appdata%\Seliware" rmdir /s /q "%appdata%\Seliware"
```

2. Перезапустите Seliware и нажмите "Load"
