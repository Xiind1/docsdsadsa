# Error: VMX/SVM is not supported

_**•**_**&#x20;Решение: Чтобы исправить эту ошибку, перейдите в «Панель управления» -> «Программы и функции» -> «Включить или выключить функции Windows» и убедитесь, что «Платформа виртуальной машины» и «Hyper-V» отключены.**

**Если ошибка не исчезла, откройте cmd от имени администратора и введите следующую команду**`bcdedit /set hypervisorlaunchtype off` **затем нажмите Enter и перезагрузите компьютер.**

**Если у пользователя Windows 11 и предыдущие способы не помогли ему, то следует запустить PowerShell от имени администратора и вставить туда(полностью) следующую команду:**

```
takeown /F "C:\Windows\System32\hvix64.exe"
icacls "C:\Windows\System32\hvix64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):F
takeown /F "C:\Windows\System32\hvax64.exe"
icacls "C:\Windows\System32\hvax64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):F
del "C:\Windows\System32\hvix64.exe"
del "C:\Windows\System32\hvax64.exe"
```
