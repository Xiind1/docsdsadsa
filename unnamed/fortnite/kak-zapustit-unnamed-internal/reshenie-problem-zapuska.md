---
icon: triangle-exclamation
---

# Решение проблем запуска

<figure><img src="../../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

***

#### Мгновенный краш при запуске игры <a href="#instant-crash-on-game-launch" id="instant-crash-on-game-launch"></a>

1. Установите последние драйверы для видеокарты: [NVIDIA](https://www.nvidia.com/Download/index.aspx) · [AMD](https://www.amd.com/en/support)
2. Откройте `System → Display → Graphics`и отключите:
   * **Аппаратное ускорение планирования задач на графическом процессоре**
   * **Переменная частота обновления**
   * **Оптимизация для игр в оконном режиме**
3. Запустите **командную строку от имени администратора** и вставьте следующую команду:

```
reg add "HKLM\SOFTWARE\Microsoft\Windows\Dwm" /v OverlayTestMode /t REG_DWORD /d 5 /f
```

4. **Перезагрузите компьютер.**
5. Попробуйте сделать инъекцию еще раз.

***

#### Мгновенный синий экран смерти после инъекции <a href="#instant-bsod-on-injecting" id="instant-bsod-on-injecting"></a>

1. Запустите **командную строку от имени администратора** и вставьте следующую команду:

```
reg add "HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management" /v FeatureSettingsOverrideMask /t REG_DWORD /d 3 /f
```

2. **Перезагрузите компьютер.**
