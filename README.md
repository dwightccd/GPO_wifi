CONFIGURAR RED WIFI POR GPO

1. Crar el arhivo XML necesario, ese archuvo se puede generar exportando la configuracion de las redes wifi de nuestro equipo 
2.            comando: netsh wlan export profile key=clear folder="CARPETA DONDE GUARDAR LA EXPORTACION"

2. crear .bat con el comando para importar la configuracion del archivo XML 
3.            Comando:    netsh wlan add profile filename="RUTA DEL ARCHIVO"

3. Crear GPO para ejecutar el archivo .bat en el inicio de sesion para cargar la informacion de la red wifi desde el archivo XML, el archivo .bat y XML deven estar accesibles desde la red para cualquier usuario para que se aplique la GPO correctamente, la configuracion de la GPO es:
4.          User cConfiguration
5.                Polices
6.                    Windows Settings
7.                          Scripts
