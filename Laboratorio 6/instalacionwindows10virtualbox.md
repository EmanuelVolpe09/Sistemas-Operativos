# Requisitos de Windows 10

## 1) Requisitos mínimos

-	Procesador de 1 GHz
-	1gb de RAM (32 bits) o 2gb de RAM (64 bits)
- 16 GB para el sistema operativo (32 bits) o 20 GB para el sistema operativo (64 bits)
- Tarjeta gráfica DirectX 9 o posterior con controlador WDDM 1.0
- Pantalla mínima de 800 x 600

## 2) Actualizaciones posibles

Debes tener Windows 7 SP1 o Windows 8.1 Update para poder actualizar.

V = se admite la actualización completa y se incluyen los datos personales, la configuración y las aplicaciones.

D = degradación de edition; se mantienen los datos personales, pero se quitan las aplicaciones y la configuración.

## WINDOWS 10

|            | Windows 10 Home | Windows 10 Pro | Windows 10 Pro Education | Windows 10 Education | Windows 10 Enterprise |
| ---------- | --------------- | -------------- | ------------------------ | -------------------- | --------------------- |
| Home       |                 |       V        |            V             |           V          |                       |
| Pro        |        D        |                |            V             |           V          |           V           |
| Education  |                 |                |                          |                      |           D           |
| Enterprise |                 |                |                          |           V          |                       |

## WINDOWS 8.1

|                   | Windows 10 Home | Windows 10 Pro | Windows 10 Pro Education | Windows 10 Education | Windows 10 Enterprise |
| ----------------- | --------------- | -------------- | ------------------------ | -------------------- | --------------------- |
| (Core)            |        V        |       V        |            V             |           V          |                       |
| Conectado         |        V        |       V        |            V             |           V          |                       |
| Pro               |        D        |       V        |            V             |           V          |           V           |
| Pro Student       |        D        |       V        |            V             |           V          |           V           |
| Pro WMC           |        D        |       V        |            V             |           V          |           V           |
| Enterprise        |                 |                |                          |           V          |           V           |
| Embedded Industry |                 |                |                          |                      |           V           |

## WINDOWS 7

|                   | Windows 10 Home | Windows 10 Pro | Windows 10 Pro Education | Windows 10 Education | Windows 10 Enterprise |
| ----------------- | --------------- | -------------- | ------------------------ | -------------------- | --------------------- |
| Starter           |        V        |       V        |            V             |           V          |                       |
| Home Basic        |        V        |       V        |            V             |           V          |                       |
| Home Premium      |        V        |       V        |            V             |           V          |                       |
| Profesional       |        D        |       V        |            V             |           V          |           V           |
| Ultimate          |        D        |       V        |            V             |           V          |           V           |
| Enterprise        |                 |                |                          |           V          |           V           |

## 3) Sobre el espacio recomendado por VirtualBox

VirtualBox sugiere 50 GB para la instalación del SO, pero Microsoft nos dice que lo mínimo es entre 16 y 20 GB. Eso es por que lo que sugiere VirtualBox son los requisitos recomendados, para una buena función del sistema. Si lo instalamos con los requisitos mínimos de Windows 10, va a correr pero mal por la falta de espacio, ya que apenas va a tener espacio para el sistema.

# Instalación de Windows 10 en VirtualBox

## Documentación de cómo instalé Windows 10 en VirtualBox.

1) Usé una ISO comprimida, la cual es la de Windows 10 1909.753 Pro
2) Cree una máquina virtual en VirtualBox con la ISO correspondiente, 4gb de RAM, 50 GB de espacio, y 2 núcleos.
3) Empezé a instalar la máquina, en -20 minutos se instaló por completo.
4) Inicié la máquina y navegué por el sistema.
5) Instalé varios navegadores compatibles.
6) Cree un volumen nuevo, ya que al instalar la máquina había dejado 35gb libres sin formatear.
7) Intenté conectarme con Conexión Remota a la máquina virtual pero fallé.
8) Instalé las Guest Additions de VirtualBox
9) Conecté la PC a la Red de la máquina anfitrión.

# Acá unas capturas:

![image](https://github.com/EmanuelVolpe09/Sistemas-Operativos/assets/171646936/a123f3b0-5562-479a-890d-5858db0d8e94)
![image](https://github.com/EmanuelVolpe09/Sistemas-Operativos/assets/171646936/05274c0d-f9e1-4697-a02a-6b40def51228)
![image](https://github.com/EmanuelVolpe09/Sistemas-Operativos/assets/171646936/d6a753c1-11f9-44ba-b68c-57bfc46a5340)
