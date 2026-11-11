---
icon: circle-chevron-right
---

# Как заупстить Xernel

<figure><img src="../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

***

## **1. Подготовка системы к запуску продукта**&#x20;

### **1.1 Отключение Безопасности Windows**

* Перейдите в параметры системы (вы можете нажать комбинацию WIN + I)
* Откройте **Безопасность Windows**
* Отключите параметр **"Защита в реальном времени" и остальные параметры защиты**

<figure><img src="../../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

#### **Окончательно отключите Безопасность Windows с помощью dControl**

* **Google Drive** - [ссылка для загрузки](https://drive.google.com/file/d/19G3C5Gg1KDr1W05jhwwB6xeMx8PG_IrU/view?usp=sharing) (пароль 1234)
* **Yandex Disk** - [ссылка для загрузки](https://disk.yandex.ru/d/pLPzChHbwskWNQ) (пароль 1234)
* **Mega** - [ссылка для загрузки](https://mega.nz/file/Vr9EUSKB#Sn0bze9l49paasaCZqYPkAodQwo5avSpUWVzo5f4x38)

<figure><img src="../../.gitbook/assets/image (141).png" alt=""><figcaption><p><strong>Нажмите "</strong><mark style="color:red;"><strong>Отключить Защитник Windows</strong></mark><strong>"</strong> </p></figcaption></figure>

#### Отключите системные защиты <a href="#kwkehrhcotqi" id="kwkehrhcotqi"></a>

1. Откройте Пуск, введите `cmd` и выберите **Запуск от имени администратора**.
2. Выполните команды по очереди

```
reg add "HKLM\SYSTEM\CurrentControlSet\Control\DeviceGuard\Scenarios\HypervisorEnforcedCodeIntegrity" /v Enabled /t REG_DWORD /d 0 /f
reg add "HKLM\SYSTEM\CurrentControlSet\Control\CI\Config" /v VulnerableDriverBlocklistEnable /t REG_DWORD /d 0 /f
reg add "HKLM\SYSTEM\CurrentControlSet\Control\DeviceGuard" /v EnableVirtualizationBasedSecurity /t REG_DWORD /d 0 /f
```

### **1.2** Удаление конфликтующего программного обеспечения

Следующие программы необходимо **полностью удалить**, а не просто закрыть:

* **Античиты FACEIT, Vanguard**
* Любой сторонний антивирус (Avast, Kaspersky, McAfee, ESET, Bitdefender и т. д.)

{% hint style="danger" %}
Если установлен FACEIT AC или сторонний антивирус, загрузчик **не будет работать** независимо от других настроек.
{% endhint %}

<h4 align="center">Перезагрузите ПК после подготовки системы.</h4>

***

## 2. Установка оверлея для отображения Xernel

{% hint style="info" %}
Работа проекта "**Xernel**" основана на продуктах, типа "**External**", в связи с чем проект использует оверлей Вашей видеокарты для отображения продукта в самой игре.
{% endhint %}

#### Включите один из поддерживаемых оверлеев.

### NVIDIA <a href="#aymjkeqtphng" id="aymjkeqtphng"></a>

1. Откройте **NVIDIA App**.
2. В **Настройках** включите **Оверлей NVIDIA**.
3. Нажмите **Alt + Z** и проверьте, что оверлей открывается.

### AMD <a href="#bqwlxyeyoabn" id="bqwlxyeyoabn"></a>

1. Откройте **AMD Radeon Software**.
2. Откройте настройки и включите **Внутриигровой оверлей**.

## 3.Установите Лаунчер

1. Откройте [страницу скачивания](https://xernel.cc/ru/launcher/download).
2. Вставьте ключ и нажмите **Скачать лаунчер**.
3. Сохраните файл `.exe` в отдельной папке, например `C:\XERNEL\`.

Если файл не скачался, проверьте загрузки браузера и нажмите **Скачать ещё раз**.

{% hint style="info" %}
Лоадер индивидуален для каждого пользователя в целях безопасности.

По этой причине скачивание с официального сайта обязательно.
{% endhint %}

## 4. Запуск продукта <a href="#jgmqeowmiuhr" id="jgmqeowmiuhr"></a>

### Запустите программу

1. Запустите лаунчер от имени администратора.
2. Если появится выбор региона, выберите сервер и нажмите **ПРОДОЛЖИТЬ**. Если появится окно входа, введите ключ и нажмите **ИНИЦИАЛИЗАЦИЯ**.
3. Выберите **AION 2**.
4. Нажмите **ЗАПУСТИТЬ**.

{% hint style="info" %}
Если появится запрос на загрузку драйвера, выберите **ДА** при первом запуске после перезагрузки. Выбирайте **НЕТ**, только если драйвер этого продукта уже успешно загружен после этой перезагрузки. При ошибке загрузки остановитесь и откройте раздел решения проблем.
{% endhint %}

### Запустите игру <a href="#dtcryucglxpa" id="dtcryucglxpa"></a>

1. После запуска программы запустите **AION 2**.
2. Войдите в игровой мир и дождитесь его загрузки.
3. Нажмите **Delete**.

Нажимайте **Delete** только после входа в игровой мир.

{% hint style="info" %}
Если игра или программа вылетела, повторите весь порядок запуска с начала: запустите программу → запустите AION 2 → войдите в мир → нажмите **Delete**.
{% endhint %}
