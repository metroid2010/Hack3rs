## Cómo instalar VirtualBox en Linux

Normalmente, suele ser tan sencillo como buscar "virtualbox" en el gestor de paquetes de vuestra distro, e instalar directamente.

Para Debian y basados en Debian (Ubuntu, Mint...):
```$ sudo apt update && sudo apt install virtualbox```

Para Arch y basados en Arch (Manjaro, Antergos...):
```$ sudo pacman -Syu && sudo pacman -S virtualbox```

Una vez esté instalado, ya puedes lanzar la aplicación. Por ejemplo, desde la consola:
```$ virtualbox

### Troubleshooting (AKA 'Houston, tenemos un problema!')

En ciertos casos, puede darse que al arrancar nos tire un error como
```The vboxdrv kernel module is not loaded```

Para corregirlo, podemos reiniciar el sistema, o cargar el módulo directamente con:
```$ sudo modprobe vboxdrv```

Con esto ya debería funcionar todo. Si no: [Keep Calm y pon una issue](https://github.com/guluc3m/Hack3rs/issues)

## Cómo instalar VirtualBox en Windows

Simplemente ve a la [página de descargas en la web oficial](https://www.virtualbox.org/wiki/Downloads) y selecciona el instalador para 'Windows hosts'.
Una vez descargado, lánzalo y sigue las instrucciones.
