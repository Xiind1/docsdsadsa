---
icon: circle-chevron-right
---

# Как запустить Matcha

<figure><img src="../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

***

### **1. Установка нужных библиотек и архиватор**

1. **.NET Framework**

* Установите последнюю версию [dotnet-sdk-9.0.301-win-x64.exe](https://builds.dotnet.microsoft.com/dotnet/Sdk/9.0.301/dotnet-sdk-9.0.301-win-x64.exe)
* Запустите приложение и следуйте инструкциям

2. **Visual C++ Redistributable**

* Установите последнюю версию [vc\_redist.x64.exe](https://aka.ms/vs/17/release/vc_redist.x64.exe)
* Установите последнюю версию [vc\_redist.x86.exe](https://aka.ms/vs/17/release/vc_redist.x86.exe)
* Запустите приложения и следуйте инструкциям

3. **DirectX**

* Установите последнюю версию [dxwebsetup.exe](https://download.microsoft.com/download/1/7/1/1718ccc4-6315-4d8e-9543-8e28a4e18c4c/dxwebsetup.exe)
* Запустите приложение и следуйте инструкциям
* В настройках dxwebsetup отключите панель bing

4. **7-Zip или WinRAR** (на ваш выбор)

* WinrRAR - [ссылка для загрузки](https://www.win-rar.com/fileadmin/winrar-versions/winrar/winrar-x64-713ru.exe)
* 7-Zip - [ссылка для загрузки](https://www.7-zip.org/a/7z2501-x64.exe)

***

### **2. Подготовка системы к первому запуску**

1. **Отключение Безопасность Windows**

* Перейдите в параметры системы (вы можете нажать комбинацию WIN + I)
* Откройте **Безопасность Windows**
* Отключите параметр **"Защита в реальном времени"**

<figure><img src="../../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

2. Окончательно отключите **Безопасность Windows** с помощью программы **dControl**

* **Google Drive** - [ссылка для загрузки](https://drive.google.com/file/d/19G3C5Gg1KDr1W05jhwwB6xeMx8PG_IrU/view?usp=sharing) (пароль 1234)
* **Yandex Disk** - [ссылка для загрузки](https://disk.yandex.ru/d/pLPzChHbwskWNQ) (пароль 1234)
* **Mega** - [ссылка для загрузки](https://mega.nz/file/Vr9EUSKB#Sn0bze9l49paasaCZqYPkAodQwo5avSpUWVzo5f4x38)

<figure><img src="../../.gitbook/assets/image (141).png" alt=""><figcaption><p><strong>Нажмите "</strong><mark style="color:red;"><strong>Отключить Защитник Windows</strong></mark><strong>"</strong> </p></figcaption></figure>

{% hint style="warning" %}
Если ваш браузер блокирует загрузку, решение можно найти [здесь](reshenie-problem-zapuska/brauzer-blokiruet-zagruzku-faila.md)
{% endhint %}

3. **Удаление сторонних антивирусов**

* Для этого я рекомендую использовать утилиту Antivirus Removal Tool.\
  Ссылка для загрузки -  [Antivirus\_Removal\_Tool.zip](https://antivirus-removal-tool.com/download/click.php?id=Antivirus_Removal_Tool)
* Извлеките файл из архива в любое удобное для вас место
* Откройте приложение, затем просканируйте систему на наличие антивирусов, для этого нажмите кнопку **Search**

<figure><img src="https://3485125295-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F02EvUuTeHDaIeSMYNRbK%2Fuploads%2FVn39uYo8egEK2m1A5ROP%2Fimage.png?alt=media&#x26;token=94e194d5-147c-496a-90c8-47180300f616" alt=""><figcaption></figcaption></figure>

* После сканирования если антивирус был обнаружен, удалите его через встроенный деинсталлятор.

{% hint style="danger" %}
**ПОСЛЕ ВСЕХ ДЕЙСТВИЙ ПЕРЕЗАГРУЗИТЕ ПК**
{% endhint %}

***

### **3. Установка VPN**

{% hint style="info" %}
Если вы проживаете в России, после недавних событий лучше сразу установить **VPN**.
{% endhint %}

1. **Установите Amnezia VPN** - [ссылка для загрузки](https://github.com/amnezia-vpn/amnezia-client/releases/download/4.8.10.0/AmneziaVPN_4.8.10.0_windows_x64.exe)
2. **Сгенерируйте конфиг Cloudflare WARP для AmneziaVPN**
   1. Инструкция - [https://github.com/ImMALWARE/bash-warp-generator](https://github.com/ImMALWARE/bash-warp-generator)
   2. Советую использовать **Вариант 4: GitHub Codespaces**
   3. После генерации конфига вам нужно его скачать.&#x20;
   4.  Скопируйте ссылку и вставьте в поисковую строку вашего браузера — файл скачается автоматически.

       <figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>
3. **Загрузите конфиг в Amnezia VPN**
   1.  Для этотого откройте приложение и выберите **"File with connection settings"**

       <figure><img src="../../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>
   2.  Выберите файл который вы только что скачали и нажмите **"Open config file"**

       <figure><img src="../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>
   3.  В приложении Amnezia VPN нажмите **"connect"**

       <figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>
4. **Для того чтобы включить VPN нажмите "Connect"**

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

**Если у вас не работает Amnezia VPN, то воспользуйтесь Windscrive VPN**

{% content-ref url="reshenie-problem-zapuska/ustanovka-windscrive-vpn.md" %}
[ustanovka-windscrive-vpn.md](reshenie-problem-zapuska/ustanovka-windscrive-vpn.md)
{% endcontent-ref %}

***

### **4. Регистрация аккаунта**

1.  Присоединитесь к официальному дискорд серверу **Matcha -** [**https://matcha-latte.win**](https://matcha-latte.win/)

    <div data-full-width="false"><figure><img src="../../.gitbook/assets/image (180).png" alt="" width="375"><figcaption></figcaption></figure></div>
2. Зайдите в канал **#redeem-key** нажмите **"Get Role"** и вставьте свой ключ.

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

3. Переместитесь в канал **#register** и перейдите по ссылке **"Register"**

<figure><img src="../../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Если у вас не открывается сайт, то включите VPN который мы ранее установили
{% endhint %}

4. Нажмите **"Register Now"**

<figure><img src="../../.gitbook/assets/image (186).png" alt=""><figcaption></figcaption></figure>

5. Зарегистрируйте аккаунт.

{% hint style="danger" %}
* **Используйте только латиницу (английские буквы) в пароле/имени пользователя**
* **Не используйте специальные символы в пароле/имени пользователя.**
* **Пожалуйста, сохраните свои логины после регистрации, на случай, если вы потеряете их и вам придется повторно покупать&#x20;**_**Matcha**_**.**
* **Избегайте использования&#x20;**_**2FA**_
* **Не меняйте пароль / имя пользователя в keyauth после регистрации, это может привести к потере лицензии!**
{% endhint %}

_1 - Имя_

_2 - Пароль_

_3 - Ключ_

<figure><img src="../../.gitbook/assets/image (188).png" alt=""><figcaption></figcaption></figure>

<p align="center"><strong>После регистрации вы должны увидеть это</strong></p>

<figure><img src="../../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure>

***

### **5. Установка лоадера**

1. Установите **Matcha** - [ссылка для загрузки](https://files.matcha-latte.win/main/matcha-ext.rar)

{% hint style="warning" %}
* Если у вас не скачивается файл, то включите VPN который мы ранее установили
* Если ваш браузер блокирует загрузку, решение можно найти [здесь](reshenie-problem-zapuska/brauzer-blokiruet-zagruzku-faila.md)
{% endhint %}

2. Извлеките файлы из архива в удобное для вас место

### 6. Процесс инжекта

1. Откройте извлечённую папку и устанавливайте драйвер при каждом выключении / перезагрузке компьютера или, по крайней мере, один раз при загрузке компьютера   \
   -> откройте **"map.exe"** и нажмите "ок"

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

2. Затем откройте **"loader.exe"** и введите свои имя пользователя и пароль.   \
   -> нажмите "продолжить"

<figure><img src="../../.gitbook/assets/image (196).png" alt=""><figcaption></figcaption></figure>

3. Запустите **"updater.exe"** чтобы получить последнее обновление

<figure><img src="../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Если у вас не скачивается обновление, то включите VPN который мы ранее установили
{% endhint %}

4. Зайдите в роблокс и запустите файл **"app.exe"**

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

5. Вот и все, можете спокойно играть!

<figure><img src="../../.gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>

<p align="center">Для того что бы закрыть/открыть меню нажмите клавишу <mark style="color:red;"><strong>INSERT</strong></mark></p>

[https://keyauth.cc/panel/jlLwSCRpHGk4cFtbMgZTsggAwaICkjxq/aTu0EHgRuMSZuajMueeHqcd5DOf5jwx1](https://keyauth.cc/panel/jlLwSCRpHGk4cFtbMgZTsggAwaICkjxq/aTu0EHgRuMSZuajMueeHqcd5DOf5jwx1)
