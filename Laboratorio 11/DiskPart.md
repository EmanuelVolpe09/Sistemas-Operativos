DiskPart es un intérprete de comandos de modo de texto que permite administrar objetos
(discos, particiones, volúmenes o discos duros virtuales) mediante el uso de scripts o
directamente desde un símbolo del sistema.

# Particionado

En la realización del tutorial voy a utilizar una máquina virtual box con un disco virtual de
3GB.

Para empezar, pulsamos las teclas WIN+R y buscamos “diskpart.exe“.

Listaremos los discos disponibles utilizando el comando “list disk“.

En la imagen anterior podemos observar que tenemos 2 discos:
–“Disco 0”, que es el disco principal en el que está instalado nuestro sistema Windows.
–“Disco 1” es el agregado de 3GB a nuestra máquina.
Por ahora el disco de 3GB no es reconocido por el sistema porque no tiene ninguna
partición creada ni montada. Para que sea reconocido, seleccionamos el disco desde
diskpart utilizando la expresión “select disk 1” y creamos una partición primaria con
“create partition primary“.

Ahora es turno de darle formato a la partición recién creada. Al realizar esta acción
tendremos que elegir el sistema de ficheros que utilizaremos y podremos asignar una
etiqueta a la nueva partición.

En este caso, el sistema de fichero que utilizaremos será “ntfs” y como nombre de etiqueta
le pondremos “DATOS”. El comando a ejecutar será de este tipo, “format fs=ntfs
label=”DATOS”“.

Cuando termine de formatear el disco, tendremos que seleccionar la partición y activarla
“active“, además de asignarle una letra “assign letter=Z“.

Tal y como asignemos la letra a la partición activa, automáticamente se montará el disco
duro y nos aparecerá una ventana para poder abrirlo.

# Redimensionamiento
En algunas ocasiones solemos crear una partición para guardar nuestros datos en caso de
tener que reinstalar el sistema operativo, como hemos hecho en el paso anterior. Ahora
vamos a ver como redimensionar la partición creada para posteriormente crear nuevas
particiones para tener una mejor organización de nuestros datos (documentos, imágenes,
videos, música).
Ejecutamos de nuevo diskpart y seleccionamos el disco y la partición a redimensionar.

Vamos a redimensionar la partición actual en 1’5GB para posteriormente asignar el
espacio libre a las nuevas particiones. En mi caso la asignación de espacio que voy a
utilizar es la siguiente:
 Documentos: 1’5GB
 Imágenes: 500MB
 Videos: 500MB
 Música: 500MB

Redimensionamos la partición “DATOS” en 1500MB ejecutando “shrink desired=1500“ y
asignamos una nueva etiqueta con “format label=”Documentos”“.

Observamos que la partición tiene ahora 1,5GB y su etiqueta es “Documentos“.

Ahora vamos a crear las siguientes 3 particiones, con formato “FAT32”:
 Imágenes: 500MB, FAT32, LETRA Y
 Videos: 500MB, FAT32, LETRA X
 Música: 500MB, FAT32, LETRA W
Teniendo el disco seleccionado en diskpart, podemos listar las particiones del disco
utilizando “list partition“.

Observamos que solo tenemos una partición de 1’5GB. Vamos a crear 3 nuevas
particiones con los parámetros indicados anteriormente.
Ejecutamos 3 veces “create partition primary size=500” (1 por partición) y listamos las
particiones para comprobar si han sido creadas.

Cuando tengamos las particiones creadas tendremos que darle formato y asignarle la
etiqueta y letra.
Vamos a ver como se haría para  la partición de imágenes.
1.  Seleccionamos la partición 2 “select partition 2“.
2.  Le damos formato e indicamos el nombre de la partición ” format fs=fat32
label=”Imagenes” “
3.  La activamos y asignamos la letra correspondiente.

Comprobamos que se monta la partición y es reconocida por el sistema.

Hacemos los mismos pasos para las particiones de videos y música. Es importante no
olvidar seleccionar la partición ya que si no haremos los cambios en la partición
anteriormente seleccionada.





Conclusión
Ya tenemos nuestras particiones creadas en el nuevo disco duro de la máquina.
