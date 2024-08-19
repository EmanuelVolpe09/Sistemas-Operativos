# Tarea: Procesos - Process Explorer

Para la realización de las siguientes prácticas deberemos instalar en el Sistema la herramienta Process Explorer:

[Process Explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer#download)

Se trata de un software desarrollado por SysInternals y que fué comprado por Microsoft y ahora se ofrece de manera gratuita desde la página de Microsoft.

## Ejercicio 1

Lanza el Bloc de Notas y el Edge, abre el Process Explorer y comprueba que los procesos han sido lanzados y están en marcha.

![image](https://github.com/user-attachments/assets/7ed25c19-518f-4802-a8e6-ae69d5da1481)
![image](https://github.com/user-attachments/assets/6fd9fb13-7963-49f4-96e8-6a7ca6a13f2d)


Realiza una captura de pantalla.

![Process Explorer](../imgs/Procesos_09.png)
\ 

## Ejercicio 2

Utilizando la opción de menú *Propiedades* sobre notepad.exe, obtén los siguientes datos acerca del ejecutable del Bloc de Notas.

![Propiedades](../imgs/Procesos_10.png)
\

* Path - C:\Windows\System32\notepad.exe
* Linea de ejecución - "C:\WINDOWS\system32\notepad.exe" 
* Directorio actual - C:\Users\vrcompu\
* Usuario que lo ha lanzado - DESKTOP-RH3KU3C\vrcompu
* Proceso que lo ha lanzado (padre) - explorer.exe(7704)
* Versión - 10.0.19041.4355

## Ejercicio 3

Obtén los mismos datos de 4 programas conocidos. Puedes realizar esta tarea en casa.

1 | Paint 3D:
* Path - C:\Program Files\WindowsApps\Microsoft.MSPaint_6.2405.19017.0_x64__8wekyb3d8bbwe\PaintStudio.View.exe
* Linea de ejecución - "C:\Program Files\WindowsApps\Microsoft.MSPaint_6.2405.19017.0_x64__8wekyb3d8bbwe\PaintStudio.View.exe" 
* Directorio actual - C:\Program Files\WindowsApps\Microsoft.MSPaint_6.2405.19017.0_x64__8wekyb3d8bbwe\
* Usuario que lo ha lanzado - DESKTOP-RH3KU3C\vrcompu
* Proceso que lo ha lanzado (padre) - sihost.exe(3624)
* Versión - n/a

2 | Explorador de Windows:
* Path - C:\Windows\explorer.exe
* Linea de ejecución - C:\WINDOWS\Explorer.EXE
* Directorio actual - C:\Windows\System32\
* Usuario que lo ha lanzado - DESKTOP-RH3KU3C\vrcompu
* Proceso que lo ha lanzado (padre) - <Non-existent Process>(6104)
* Versión - 10.0.19041.4717

3 | Calculadora:
* Path - C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_11.2405.2.0_x64__8wekyb3d8bbwe\CalculatorApp.exe
* Linea de ejecución - "C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_11.2405.2.0_x64__8wekyb3d8bbwe\CalculatorApp.exe" 
* Directorio actual - C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_11.2405.2.0_x64__8wekyb3d8bbwe\
* Usuario que lo ha lanzado - DESKTOP-RH3KU3C\vrcompu
* Proceso que lo ha lanzado (padre) - sihost.exe(3624)
* Versión - 11.2405.2.0

4 | Skype:
* Path - CC:\Program Files\WindowsApps\Microsoft.SkypeApp_15.125.3201.0_x64__kzf8qxf38zg5c\Skype\Skype.exe
* Linea de ejecución - "C:\Program Files\WindowsApps\Microsoft.SkypeApp_15.125.3201.0_x64__kzf8qxf38zg5c\Skype\Skype.exe" --share-file="C:\Users\vrcompu\Desktop\procexp64.exe"
* Directorio actual - C:\Program Files\WindowsApps\Microsoft.SkypeApp_15.125.3201.0_x64__kzf8qxf38zg5c\Skype\
* Usuario que lo ha lanzado - DESKTOP-RH3KU3C\vrcompu
* Proceso que lo ha lanzado (padre) - dllhost.exe(14580)
* Versión - 8.125.0.201

PD: Intenté buscar esta info del Editor del Registro y del Visor de Eventos, pero me saltó error y que no tenía permisos.
