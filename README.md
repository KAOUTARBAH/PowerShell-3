# PowerShell-3

### 1. Lancer les calculatrices
    powershell
    Start-Process calc.exe
    Start-Sleep -Seconds 1
    Start-Process calc.exe
    $AllProcess = Get-Process

![lancer commandes](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/clac.png)

**Trouve la ligne de commande qui permettra d'avoir à l'écran les différentes lignes de processus qui contiennent** "calc"
### Il y a 2 méthodes différentes: à partir de la variable $AllProcess 
    $AllProcess | Where-Object {$_.Name -like "*calc*"}

![all Process](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/allProcess.png)


### A partir de la recherche direct avec la commande Get-Process
    Get-Process | Where-Object {$_.Name -like "*calc*"}

![get Process](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/getprocess.png)


### Récupère l'historique des commandes que tu as tapées avec Get-History
    Get-History
![get History](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/gethistory.png)