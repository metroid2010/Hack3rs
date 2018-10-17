## Cómo instalar Kali en una máquina con VirtualBox

Este procedimiento nos vale tanto para la versión de Linux como para la versión de Windows.

### Antes de lanzar VirtualBox

Para crear una máquina virtual (vm) funcional, necesitaremos instalar un sistema operativo.
En nuestro caso, usaremos Kali Linux. Para descargar la iso, id a la [página oficial](https://www.kali.org/downloads) y seleccionad el [entorno de escritorio](https://wiki.archlinux.org/index.php/Desktop_environment) que prefiráis. [El predeterminado](http://cdimage.kali.org/kali-2018.3a/kali-linux-2018.3a-amd64.iso) ([Gnome](https://wiki.archlinux.org/index.php/GNOME)) nos vale.

### Creando la VM

1. Abrimos VB. En la ventana principal de VirtualBox, tenemos un panel a la izquierda donde aparecerán las máquinas que hagamos. Estará en blanco porque aún no tenemos ninguna.
2. Pulsamos en New, arriba a la izquierda.
3. Se abre una ventana que nos pide un nombre para la máquina, y el tipo. Para nuestro caso, elegimos "Linux", y como versión, "Others 64 bits". El nombre queda a vuestra elección.
4. Para la memoria, el valor dependerá de la que tenga vuestro propio equipo. Como regla general, no seleccionéis más de la mitad de lo que tengáis. Entre 1.5GB y 3GB está bien.
5. Ahora tenemos que hacer el disco duro virtual. Esto es un archivo que a ojos de la máquina virtual, actuará como si se tratara de un disco duro físico.
   - Elegimos "Create a virtual hard disk now"
   - El tipo no tiene demasiada importancia. Nos quedamos con el seleccionado por defecto.
   - Elegimos "Dynamically allocated". Esto significa que, en lugar de crearse ocupando su espacio nominal, el disco duro virtual irá creciendo en tamaño según vaya llenándose, hasta alcanzar el máximo configurado.
   - Dejamos el nombre por defecto. Para el tamaño, la elección depende de nuevo de vuestro equipo. Como mínimo, elegid 10GB.

Una vez terminado este proceso, la máquina aparecerá en el panel de la izquierda.
Ya podemos instalar Kali.

### Instalando Kali

1. Abrimos la máquina pinchando encima.
2. Nos pedirá que seleccionemos un disco. Pinchamos en el botón con forma de carpeta, a la izquierda. Buscamos la iso que descargamos antes.
3. Una vez seleccionada, pinchamos "Start".
4. Cuando arranque, saldrá un menú. Pinchamos sobre la ventana para que la máquina capture el teclado y el ratón. Con el teclado, seleccionamos "Graphical Install" y pulsamos Enter.
5. El menú de instalación se abrirá. Elegimos un idioma.
6. Elegimos región y teclado.
7. Como hostname, cualquiera nos vale.
8. Dejamos el dominio en blanco.
9. Introducimos una contraseña para el [superusuario](https://en.wikipedia.org/wiki/Superuser). Es importante, recordadla. O apuntadla en un papel.
10. Elegimos zona horaria.
11. Para el particionado, elegimos las opciones por defecto. ("Use entire disk", "SCSI [...]", "All files in one partition", "Finish partitioning and write changes to disk", "Write changes" -> "Yes")

Empezará la instalación. Esperamos un rato.

