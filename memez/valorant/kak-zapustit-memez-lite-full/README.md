---
icon: circle-chevron-right
---

# Как запустить Memez Lite / Full

<figure><img src="../../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

**МОЙ FUNPAY** - [https://funpay.com/users/4526933/](https://funpay.com/users/4526933/)

***

## **1. Подготовка системы к запуску продукта**&#x20;

### 1.1 Установка нужных библиотек и архиватор

1. **Visual C++ Redistributable**

* Установите последние версии - х64: [ссылка](https://drive.google.com/file/d/1-MAtvixkw43959-WtNi-VQU_weMeZsc-/view?usp=sharing) | х86: [ссылка](https://drive.google.com/file/d/14BXKselMkLJjviLU2OQoP8HezQH1QV6p/view?usp=sharing)
* Запустите приложение и следуйте инструкциям

2. **DirectX**

* Установите последнюю версию - [ссылка](https://drive.google.com/file/d/19jF0U9gxYGgPWNBFyVe-dTOA0S-nOEMG/view?usp=sharing)
* Запустите приложение и следуйте инструкциям

3. **WinRAR**&#x20;

* Установите последнюю версию - [ссылка](https://drive.google.com/file/d/10_CpTVkO-4uzPlhhYki8XqnnCVlWVJLA/view?usp=sharing)

### **1.2 Отключение Безопасности Windows**

* Перейдите в параметры системы (вы можете нажать комбинацию WIN + I)
* Откройте **Безопасность Windows**
* Отключите параметр **"Защита в реальном времени" и остальные параметры защиты**

<figure><img src="../../../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

#### **Окончательно отключите Безопасность Windows с помощью dControl**

* **Google Drive** - [ссылка для загрузки](https://drive.google.com/file/d/19G3C5Gg1KDr1W05jhwwB6xeMx8PG_IrU/view?usp=sharing) (пароль 1234)
* **Yandex Disk** - [ссылка для загрузки](https://disk.yandex.ru/d/pLPzChHbwskWNQ) (пароль 1234)
* **Mega** - [ссылка для загрузки](https://mega.nz/file/Vr9EUSKB#Sn0bze9l49paasaCZqYPkAodQwo5avSpUWVzo5f4x38)

<figure><img src="../../../.gitbook/assets/image (141).png" alt=""><figcaption><p><strong>Нажмите "</strong><mark style="color:red;"><strong>Отключить Защитник Windows</strong></mark><strong>"</strong> </p></figcaption></figure>

### **1.3** Удаление конфликтующего программного обеспечения

Следующие программы необходимо **полностью удалить**, а не просто закрыть:

* **Античит FACEIT**
* Любой сторонний антивирус (Avast, Kaspersky, McAfee, ESET, Bitdefender и т. д.)

{% hint style="danger" %}
Если установлен FACEIT AC или сторонний антивирус, продукт **не будет работать** независимо от других настроек.
{% endhint %}

### 1.4 Включение виртуализации

Включите: <mark style="color:red;">**VT-X (VT-D)**</mark> <mark style="color:red;"></mark><mark style="color:red;">|</mark> <mark style="color:red;"></mark><mark style="color:red;">**SVM Mode**</mark> <mark style="color:red;"></mark><mark style="color:red;">(AMD CPU) (Виртуализация) (в BIOS)</mark> - Можно проверить включено ли по следующему пути: Диспетчер Задач -> ЦП -> Процессор

<figure><img src="../../../.gitbook/assets/image (120).png" alt=""><figcaption><p><strong>Виртуализация: Включено</strong></p></figcaption></figure>

### 1.5 Включение HyperV

1. Откройте панель управления
2. В панели управления выберите **Программы** -> **Программы и компоненты**.
3.  В списке найти и выбрать для установки компоненты «Платформа Hyper-V»

    Нажать на плюс и поставить везде галочки

    Нажать «ОК»
4.  Откройте CMD от имени админа и введите:

    `bcdedit /set hypervisorlaunchtype auto`

<figure><img src="../../../.gitbook/assets/image (352).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Если опция включения функции "Гипервизор Hyper-V" недоступна (заблокирована), это означает, что в настройках биоса у вас не включена виртуализация.

Если функция "Hyper-V" не отображается, это означает, что компоненты Hyper-V не установлены в вашей системе (скорее всего, потому что у вас установлена ​​Windows Home Edition). В этом случае вы можете следовать этому руководству - [ссылка на руководство](https://pureinfotech.com/install-hyperv-home-windows-11/)
{% endhint %}

### 1.6 Включение изоляции ядра

1. Откройте **Безопасность Windows**, перейди в раздел:                                                Безопасность устройства -> Сведения об изоляции ядра

<figure><img src="../../../.gitbook/assets/image (353).png" alt=""><figcaption></figcaption></figure>

2. Включите **Целостность памяти**

<figure><img src="../../../.gitbook/assets/image (354).png" alt=""><figcaption></figcaption></figure>

## 2. Запуск продукта

### 1. Установите этот батник если у вас Windows 11

[https://loader.colortune.ru/win11\_driver\_OFF.reg](https://loader.colortune.ru/win11_driver_OFF.reg)

(ПКМ на ссылку - сохранить как, если у вас не качается ничего после перехода по ссылке)

Запустите, примените изменения, перезагрузите ПК&#x20;

{% hint style="info" %}
Это требуется сделать только перед первым запуском.
{% endhint %}

### 2. Настройка оверлея для отображения Memez

Для работы Memez Lite/Full потребуется настроить оверлей приложения **Discord**

1. Игра должна быть в "**Windowed Fullscreen"** (в безрамочном режиме), чтобы у нас работал оверлей дискорда.
2. Зайдите в настройки и в разделе **"игровой оверлей"** включите оверлей, затем отключите **"устаревший оверлей"**.
3. Зайдите в настройки и в разделе **"система"** включить **"включить аппаратное ускорение"**

### 3. Установка лаунчера и запуск

{% hint style="danger" %}
ЧИТ ЗАПУСКАЕТСЯ СТРОГО ДО ИГРЫ!
{% endhint %}

1. Скачайте лаунчер: [https://loader.colortune.ru](https://loader.colortune.ru/)
   1. введите код активации
   2. скачайте лаунчер
2. Запустите лаунчер
3. Введите ваш код активации в появившейся консоли и нажмите **Enter**
4. Если все прошло успешно, то у вас будет надпись **"Press f1 in the main menu"**
5. Зайдите в игру и в главном меню нажмите <mark style="color:$danger;">F1</mark>
6. Ожидайте загрузки софта

{% hint style="info" %}
Зайдите в игру 5×5 в рейтинговом или безрейтинговом режиме. Также проверить работу можно в быстрой игре.\
Если у вас нет визуалов в игре, нажмите f5 в начале раунда.
{% endhint %}

***

<h4 align="center">Меню открывается/закрывается на <mark style="color:$danger;">INSERT</mark></h4>
