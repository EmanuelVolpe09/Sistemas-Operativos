# Cuestionario: Particiones de Disco Duro
### 1. ¿Qué es una partición de disco duro?
- Es una división lógica de una unidad de almacenamiento en la que se guardan datos y archivos. Tienen diferentes formatos, cada uno con ventajas y desventajas.
### 2. ¿Cuáles son los dos esquemas de particionamiento más conocidos?
- GPT y MBR
### 3. ¿Qué es el espacio sin particionar?
- Es una parte del disco que no está particionada, y por lo tanto no tiene una división lógica donde alojar archivos, osea que es inútil hasta que se particione.
### 4. Mencione al menos tres sistemas de archivos y sus características principales.
- NTFS: (New Technology File System) Se usa desde el 2001, en sistemas Windows. Sus límites son particiones de hasta 265 tb, y manejar archivos de hasta 16 tb. Una de sus desventajas es que solo es compatible con Windows, ya que con otros SO, puede convertirse en una unidad de solo lectura o de plano no funcionar.
- FAT32: Sistema anterior al NTFS de Windows. Tiene limitaciones como no poder trabajar con archivos de más de 4 gb, o crear particiones de más de 2 tb.
- exFAT: Sistema también de Microsoft, pero dedicado a las unidades extraíbles como Pendrives. Es como la remasterización de FAT32, y tiene más soporte que NTFS.
### 5. ¿Cómo interpreta un sistema operativo las particiones en un disco duro?
- 
### 6. Describa el esquema de partición MBR.
- Master Boot Record (MBR)
  Estándar antiguo de partición de disco duro, que está dejando de ser compatible con algunos sistemas operativos. Compatible con BIOS
### 7. Describa el esquema de partición GPT.
- Tabla de partición GUID (GPT)
  Estándar moderno de partición de disco duro, que tiene compatibilidad con los sistemas operativos modernos. La ventaja de GPT es el enorme tamaño de la partición, el número de particiones y la capacidad de recuperación. Compatible con UEFI
### 8. ¿Cuáles son los tipos de particiones en un disco duro con MBR?
- Las particiones pueden clasificarse como particiones primarias y particiones extendidas en un disco MBR.
### 9. ¿Cuál es la principal diferencia entre particiones primarias y extendidas?
- La partición primaria es una partición que el ordenador reconoce nada más arrancar. Por tanto, acá se suele instalar el sistema operativo. Como máximo, puede haber 4 particiones primarias en un disco duro.
- En cambio, la partición extendida no es detectada por la BIOS y, por ende, no se puede instalar un sistema operativo en ella. La finalidad de esta partición es la de almacenar datos, aunque sólo podremos tener una de estas particiones.
### 10. Compare el número máximo de particiones en discos MBR y GPT.
- MBR es de hasta 4 particiones primarias (o tres particiones primarias, una partición extendida y unidades lógicas ilimitadas), y GPT es de 128 particiones primarias.
### 11. ¿Cuál es el tamaño máximo de volúmenes admitido por los estilos MBR y GPT?
- MBR es de 2 terabytes, y GPT de 18 exabytes.
