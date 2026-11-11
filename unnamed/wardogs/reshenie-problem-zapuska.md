---
icon: triangle-exclamation
---

# Решение проблем запуска

<figure><img src="../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

***

#### Мгновенный краш при запуске игры <a href="#instant-crash-on-game-launch" id="instant-crash-on-game-launch"></a>

1. Установите последние драйверы для видеокарты: **NVIDIA** · **AMD**
2. Откройте **«Система» → «Видео» → «Графика»** и отключите следующие параметры:
   * Аппаратное ускорение планирования задач на графическом процессоре
   * Переменная частота обновления
   * Оптимизация для игр в оконном режиме
3. Запустите **командную строку от имени администратора** и вставьте следующую команду:

```
reg add "HKLM\SOFTWARE\Microsoft\Windows\Dwm" /v OverlayTestMode /t REG_DWORD /d 5 /f
```

4. Отключите **виртуализацию** в настройках BIOS.
5. Перезагрузите компьютер.
6. Попробуйте сделать инъекцию еще раз.

***

#### Driver Error 1, 2

Для устранения этих ошибок инициализации драйверов необходимо отключить конфликтующие функции безопасности и античиты:

* Отключить **HVCI** (проверку целостности памяти).
* Отключите **список заблокированных уязвимых драйверов Microsoft** .
* Отключите **Windows Defender** с помощью dControl (Defender Control).
* Удалите **Riot Vanguard** и **FACEIT AC** .

***

#### Can't Handle Driver

Если во время запуска возникла следующая ошибка:

* Перейдите в настройки безопасности Windows и установите для всех параметров **защиты от эксплойтов значение «По умолчанию»** .

***

#### Нет меню после нажатия F2

1. Нажмите клавишу **F2** и посмотрите, какое сообщение появится в загрузчике.
   * Если отображается сообщение об ошибке `"Initialize Complete"`, перейдите к следующему шагу.
   * Если вы видите сообщение об ошибке, пожалуйста, свяжитесь с продавцом.
2. Отключите **все** фоновые наложения от других программ (таких как NVIDIA GeForce Experience, Discord, AMD Adrenalin и т. д.).
3. Подключитесь к **VPN** и попробуйте снова.

***

#### BSOD после нажатия F2

Если после нажатия клавиши F2 ваш компьютер зависает с «синим экраном смерти», вам необходимо отключить KPTI.

Запустите **командную строку от имени администратора** и вставьте следующие команды по очереди:

```
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverride /t REG_DWORD /d 3 /f
```

```
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverrideMask /t REG_DWORD /d 3 /f
```

_После внесения этих изменений в реестр перезагрузите компьютер, прежде чем снова пытаться выполнить запуск._
