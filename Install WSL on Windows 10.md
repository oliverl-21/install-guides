# Install WSL on Windows 10
>[MS WSL Install Guide](https://docs.microsoft.com/de-de/windows/wsl/install-win10)

>For x64 systems: Version 1903 or higher, with Build 18362 or higher.


[![Youtube Video](https://img.youtube.com/vi/D7Em1wjMiak/0.jpg)](https://www.youtube.com/watch?v=D7Em1wjMiak)

## 1. WSL aktivieren
* Powershell als Administrator ausführen und folgende befehle eingeben:
```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
* Restart your Computer
* Download and Install [WSL Kernel Update](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
## 2. WSL 2 aktivieren
* Powershell öffnen und folgenden Befehl ausführen:
```powershell
wsl --set-default-version 2
```
## 3. Linux Distribution wählen
* [Microsoft Store](https://aka.ms/wslstore) öffnen und Distribution auswählen
  * [Debian](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
  * [Ubuntu 20.04](https://www.microsoft.com/store/apps/9n6svws3rx71)


## Optional: Windows Terminal

Als moderne alternative für die alte `cmd.exe` gibt es von Microsoft ein neues Terminal dass alle Konsolen (WSL, Powershell, CMD, Azure CLI, usw.) vereint und auf den aktuellen Stand bringt. [Windows Terminal Download](https://aka.ms/terminal)

> min. Windows 10 1903 oder später

![Windows Terminal](https://docs.microsoft.com/en-gb/windows/terminal/images/dynamic-profiles.png)

[Dokumentation](https://docs.microsoft.com/en-gb/windows/terminal/)

