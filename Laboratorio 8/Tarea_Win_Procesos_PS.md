# Tarea: Procesos - PowerShell

Una vez vistos los procesos, vamos a realizar una serie de scripts que nos permitirán obtener información acerca de los procesos y realizar acciones sobre ellos.

``` powershell
Get-Process
Stop-Process
```

Referencias:

* [Get-Process](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/get-process?view=powershell-6)
* [Stop-Process](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/stop-process?view=powershell-6)


## Ejercicio 1

Realiza un Script que obtenga el los detalles del proceso cuyo nombre sea `MicrosoftEdge`

Get-Process chrome (en la PC de la escuela no está instalado Edge y no se puede instalar debido al internet).

## Ejercicio 2

Realiza un Script que muestre todos los procesos cuyo nombre sea `svchost`

Get-Process svchost

¿Qué hace este proceso? ¿Porqué hay tantos?

Es un proceso que se utiliza en la familia NT de Windows, y sirve para hospedar servicios del sistema.

## Ejercicio 3

Realiza un Script que muestre la ruta al ejecutable del proceso de `MicrosoftEdge`

Get-Process chrome | Format-List *

## Ejercicio 4

Realiza un Script que detenga el proceso del Bloc de notas

Stop-Process -Name "notepad"

## Ejercicio 5

Realiza un script que muestre **tan solo** el tiempo de la CPU de un proceso dado (por ejemplo `notepad`). 

Get-Process chrome | Format-Table CPU

## Ejercicio 6

¿Qué muestra el siguiente script?

``` powershell
Get-Process | where {$_.mainWindowTitle} | Format-List id, name, mainwindowtitle

Muestra todos los procesosque tengan una ventana, en formato de lista que diga la id, el nombre, y el título de la ventana.
```
