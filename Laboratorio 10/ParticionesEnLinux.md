Tutorial particiones en Linux
1. Use fdisk -l para buscar el tamaño total de todos los
discos fijos en su sistema
Respuesta:

![image](https://github.com/user-attachments/assets/f8ee4475-accc-4645-b7b0-004e242f61ce)



2. Cree una partición primaria de 2GB en sdb
Respuesta:

![image](https://github.com/user-attachments/assets/b847ede6-e936-4017-9454-ff297c2c99ae)



Debe quedar así

3. Cree una partición primaria de 4GB en sdb y una
partición extendida de 4GB, dentro dos particiones lógicas
de 2GB

Debe quedar así

4. Asignar un tipo de archivo a las particiones
sdb5 ntfs código 7
sdb6 fat32 código b

5. Guardar w y salir

6. Formatear las particiones
sdb1 ext4 Label datos-ext4
sdb2 ext3 Label datos-ext3
sdb5 ntfs Label datos-ntfs
sdb6 fat32 Label datos-fat32

7. Establecer las etiquetas a las particiones
 e2label /dev/sdb1 datos-ext4
 e2label /dev/sdb2 datos-ext3
 ntfslabel /dev/sdb5 datos-ntfs
 fatlabel /dev/sdb6 datos-fat
En modo grafico debe verse así

8. Montar las particiones
Crear los directorios

9. Montar las particiones

Damos permisos  chmod 777 -R /unidades

10. Con el comando mount vemos todas las unidades montadas
