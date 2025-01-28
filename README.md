# PowerShell-3

### 1. Lancer les calculatrices
    powershell
    Start-Process calc.exe
    Start-Sleep -Seconds 1
    Start-Process calc.exe
    $AllProcess = Get-Process


**Trouve la ligne de commande qui permettra d'avoir à l'écran les différentes lignes de processus qui contiennent** "calc"
### Il y a 2 méthodes différentes: à partir de la variable $AllProcess 
    $AllProcess | Where-Object {$_.Name -like "*calc*"}

![calc Process](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/allProcess.png)
![all Process](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePowercalc.png)


### A partir de la recherche direct avec la commande Get-Process
    Get-Process | Where-Object {$_.Name -like "*calc*"}

![get Process](https://github.com/KAOUTARBAH/PowerShell-3/blob/main/imagePower/getprocess.png)

