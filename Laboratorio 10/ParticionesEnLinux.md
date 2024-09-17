Tutorial particiones en Linux
1. Use fdisk -l para buscar el tamaño total de todos los
discos fijos en su sistema
Respuesta:

![image](https://github.com/user-attachments/assets/dcbe3a1c-859a-4d62-bd91-76a61c2acc7f)




2. Cree una partición primaria de 2GB en sdb
Respuesta:

![image](https://github.com/user-attachments/assets/b847ede6-e936-4017-9454-ff297c2c99ae)
![image](https://github.com/user-attachments/assets/b3f8cd93-f735-4aef-8979-5769e125fe99)



Debe quedar así

3. Cree una partición primaria de 4GB en sdb y una
partición extendida de 4GB, dentro dos particiones lógicas
de 2GB

![image](https://github.com/user-attachments/assets/a3663fa2-b60c-4135-9946-fe653d675a2a)
---
![image](https://github.com/user-attachments/assets/2be56299-60d6-49b5-9403-c5de7a220850)
---
![image](https://github.com/user-attachments/assets/ddc3d3b8-3fbc-4016-a57a-8f65e0fe5f2e)
---
![image](https://github.com/user-attachments/assets/fe0072a9-7160-4dc1-82de-f0453ad9f19e)
---

Debe quedar así

![image](https://github.com/user-attachments/assets/5b22c69a-50c4-4396-a593-ad437dd8f589)


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
