# Laboratorio 1: Clonación de Máquinas Virtuales

## Objetivo:
Clonar una máquina virtual para crear una copia exacta.

## Pasos:

### Crear una máquina virtual base:
1. Crear una nueva máquina virtual con una instalación de un sistema operativo (ej: Ubuntu).
2. Realizar configuraciones iniciales básicas (ej: instalación de actualizaciones, herramientas de desarrollo).

### Clonación de la VM:
1. Apagar la máquina base.
2. En el menú de VirtualBox, hacer clic derecho sobre la VM -> Opción "Clonar".
3. Seleccionar "Clonación Completa" para una copia completa o "Clonación Enlazada" si se desea ahorrar espacio en disco (pero compartiendo discos virtuales).

### Verificación:
1. Iniciar ambas máquinas (la original y la clonada) para verificar que ambas funcionan correctamente de manera independiente.

### Informe esperado:
- Captura de pantalla de ambas máquinas corriendo de forma simultánea.
![image](https://github.com/user-attachments/assets/bfd97005-02bb-4258-8eaa-ff6b07127335)
- Comandos que verifiquen que tienen configuraciones de red y hostname diferentes.
![image](https://github.com/user-attachments/assets/3e4ba52f-b593-4e22-9492-85dc05b30c41)
---

# Laboratorio 2: Uso de Guest Additions

## Objetivo:
Instalar y utilizar Guest Additions para mejorar la integración entre el sistema host y las máquinas virtuales.

## Pasos:

### Instalar Guest Additions:
1. Iniciar la máquina virtual.
2. Desde el menú de VirtualBox, ir a "Dispositivos" -> "Insertar imagen de CD de las Guest Additions".
3. Dentro de la VM, abrir un terminal y ejecutar el siguiente comando:
    ```bash
    sudo sh /media/cdrom/VBoxLinuxAdditions.run
    ```
4. Reiniciar la VM.

### Verificación:
1. Probar la redimensión automática de la pantalla.
2. Habilitar y probar la opción de compartir portapapeles y arrastrar y soltar archivos.

### Informe esperado:
- Capturas de pantalla del cambio de tamaño dinámico de la ventana.
![image](https://github.com/user-attachments/assets/9690afb6-8a26-47f5-a6ef-b640c186088b)
- Una demostración de arrastrar un archivo entre el host y la VM.
![image](https://github.com/user-attachments/assets/3b13e193-6ccb-4486-afd0-b17f2f1664b2)
![image](https://github.com/user-attachments/assets/f46e0fdd-f25a-4d49-8879-3120521f0a13)
![image](https://github.com/user-attachments/assets/9cd199ad-6063-48fe-8f9c-3154c364a95e)


