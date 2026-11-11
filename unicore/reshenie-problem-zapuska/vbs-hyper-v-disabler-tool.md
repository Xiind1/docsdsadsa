# VBS / Hyper-V Disabler Tool

## Ошибка "VBS" и "HyperV" в launcher

<img src="https://unicore-2.gitbook.io/instruction-ru/~gitbook/image?url=https%3A%2F%2F2582495776-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FLdxCokJEnpQ3wG4zbVLX%252Fuploads%252FDKYySqkw6eXHWRN9DEOd%252Fimage.png%3Falt%3Dmedia%26token%3D5e38bc2c-51fc-4261-849f-016931becd49&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=a801d99add8fea4f3c0b07a1ea4c9b9f&#x26;sv=3" alt="" height="604" width="789">

{% hint style="info" %}
Для корректной работы hypervisor вам необходимо отключить встроенный hyper-v в Windows и VBS.
{% endhint %}

1. Отключите Windows Hello пароль для корректной работы автоматической утилиты.
2. Запустите утилиту "[Fixit](https://mega.nz/file/M3ZAzAZS#I6Upy8kNTzJeguqC4V9ZE_8fXBrtPOj5HwtU2JIWE80)", дождитесь окончания проверки и перезапустите ПК.
3. Нажмите F3 после перезагрузки в окне VBS.
4. Откройте launcher и проверьте вкладку System Health снова.

{% hint style="danger" %}
Внимание! Обязательно отключите пароль к системе Windows, так как во время автоматических фиксов может быть сброшен TPM модуль, в случае если вы не отключили пароль, ваш пароль к Windows не сработает и вам придеться воспользоваться Windows Recovery Option.
{% endhint %}
