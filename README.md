CONFIGURAR RED WIFI POR GPO

1. Crar el arhivo XML necesario, ese archuvo se puede generar exportando la configuracion de las redes wifi de nuestro equipo 
       comando: netsh wlan export profile key=clear folder="CARPETA DONDE GUARDAR LA EXPORTACION"

2. crear .bat con el comando para importar la configuracion del archivo XML 
       Comando:    netsh wlan add profile filename="RUTA DEL ARCHIVO"

3. Crear GPO para ejecutar el archivo .bat en el inicio de sesion para cargar la informacion de la red wifi desde el archivo XML
