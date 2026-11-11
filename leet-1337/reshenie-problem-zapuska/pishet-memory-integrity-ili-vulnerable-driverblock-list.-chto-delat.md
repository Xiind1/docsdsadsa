# Пишет Memory integrity или Vulnerable Driverblock list. Что делать?

Вам нужно нажать на кнопку "OPEN", она откроет для вас настройки изоляции ядра. В них нужно выключить тумблеры "Целостность памяти" и "Чёрный список уязвимых драйверов". После этого необходимо перезагрузить компьютер и всё заработает.

Если у вас вырезан Windows Defender или по какой-то причине нет одного из тумблеров, то нужно открыть командную строку от имени администратора и вписать следующие команды:

* `reg add "HKLM\SYSTEM\CurrentControlSet\Control\DeviceGuard\Scenarios\HypervisorEnforcedCodeIntegrity" /v Enabled /t REG_DWORD /d 0 /f`
* `reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\CI\Config" /v VulnerableDriverBlocklistEnable /t REG_DWORD /d 0 /f`

После чего, как и в способе выше, нужно будет перезагрузить компьютер.
