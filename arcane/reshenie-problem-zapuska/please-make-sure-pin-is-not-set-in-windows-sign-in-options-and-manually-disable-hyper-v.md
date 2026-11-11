# Please make sure PIN is not set in Windows sign-in options and manually disable Hyper-V

<figure><img src="../../.gitbook/assets/image (416).png" alt=""><figcaption></figcaption></figure>

1. Отключите Windows Hello пароль для корректной работы автоматической утилиты.

<figure><img src="../../.gitbook/assets/image (414).png" alt=""><figcaption></figcaption></figure>

2. Запустите утилиту "[Fixit](https://e.pcloud.link/publink/show?code=XZpuraZ8CQyIFjpxi5h6XD8nIcGSpbmmU9k)", дождитесь окончания проверки и перезапустите ПК.
3. Нажмите F3 после перезагрузки в окне VBS.

{% hint style="danger" %}
Внимание! Обязательно отключите пароль к системе Windows, так как во время автоматических фиксов может быть сброшен TPM модуль, в случае если вы не отключили пароль, ваш пароль к Windows не сработает и вам придеться воспользоваться Windows Recovery Option.
{% endhint %}
