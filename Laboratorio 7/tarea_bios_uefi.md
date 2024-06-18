![image](https://github.com/EmanuelVolpe09/Sistemas-Operativos/assets/171646936/b8be65c5-9562-4d3d-ba68-2bb8000b90e8)
# Tarea: BIOS vs UEFI

## Ejercicio 1

Entra en la BIOS o arranque de tu ordenador, ya sea el de clase o en tu casa, averigua cual es la tecla que nos permite en el arranque entrar en este sistema. Describe el proceso que has seguido y adjunta una captura de pantalla del resultado (puedes utilizar la cámara de tu móvil).
![image](https://github.com/EmanuelVolpe09/Sistemas-Operativos/assets/171646936/65b2afaa-e8a8-464a-8198-671cd0ecda51)
Para entrar a la BIOS de mi máquina virtual de Windows 7, hay que habilitar el EFI en la configuración de la máquina (solo se puede en algunos SO).
Luego se prende la máquina como siempre, y se presiona Enter para entrar a la BIOS.
Después, hay que ir a Boot Manager, y bootear EFI Shell.

## Ejercicio 2

Siguiendo los pasos que hemos visto en clase, obtén la información de tu sistema operativo acerca de si ha arrancado sobre una BIOS o sobre UEFI.

La máquina virtual inicia la BIOS al arrancar el sistema, y normalmente inicia el Windows Boot Manager, pero como cuando activo la EFI Shell no detecta el SO, entonces no bootea nada.
Y UEFI se puede bootear entrando a la BIOS.

## Ejercicio 3

En GNU/LinuX, si hemos arrancado sobre UEFI existirá un directorio que contendrá información acerca de nuestra UEFI. ¿Cúal es? En caso de que exista...¿Cual es el contenido del fichero *systab*?

No existe ningún fichero, y además ni con Super Usuario se puede acceder a los archivos del sistema.


## Ejercicio 4

Obtener información de cual es la temperatura del Microprocesador en tu BIOS/UEFI. Adjunta una captura/foto.
