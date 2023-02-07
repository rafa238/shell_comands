Comandos
tee -> Copia la el input a cada archivo
cat -> Permite ver el contenido de archivos, concatena archivos
which -> Nos dice la ruta de un comando 
greep -i PATRON archivo.csv-> buscar patron en ignore case en el archivo.csv
wc arhivo.csv -lwc -> contar cuantas lineas tiene, letras, bits y nombre del archivo

comprimir:
tar -cvf <nombreComprimido>.tar <carpeta a comprimir> -> Comprimir un archivo a .tar
tar -cvzf <nombreComprimido>.tar.gz <carpeta a comprimir> -> Comprimir un archivo a .tar.gz
tar -xvf <nombreDescomprimir>.tar -> Descomprimir un archivo .tar al original
tar -xvzf <nombreDescomprimir>.tar.gz -> Descomprimir un archivo .tar.gz al original
zip -r <nombreComrpimido>.zip <Carpeta a comprimir> -> Genera una compresion .zip
unzip <nombreComrpimido>.zip -> Descomprimir un archivo .zip


Procesos:
CRTL + Z -> Stop tarea
CTRL + C -> Terminar el proceso
CTRL + D -> Terminar y guardar cambios
ps -> Mostrar procesos o comandos corriendo en la terminal
top -> mostrar los procesos y si presionamos k podemos matar algunos
htop -> interfaz de consola para eliminar procesos
job -> Todos los procesos en el background
fg <task number> -> permite traer al foreground (CMD actual visible) y terminar la tarea
bg <tasknumber> -> permite traer la tarea al bakcgroud (Ejecutar en segundo plano) y liberar el cmd actual
operador & -> manda la task al background

RED
ifconfig -> ver las tarjetas de red, ips y mas aras de subred de nuestra pc
ping <conexion> -> sirve para comprobar conexion
curl <conexcion> -> ver con que contesta  (html u otros)
traceroute <conexion> -> ver la ruta que sigue para conectar a una direccion
netstat -i -> igual que ifconfig pero amigable

Busquedas
find ./ -type f -name '*.txt' -size 20M 
Filtramos los archivos con nombre en terminacion .txt, tipo file, y 20 megas 


Wildcards
[[:upper:]]* Busca archivos que empiezen con una letra en uppercase
[[:digit::]]? Busca elementos con un numero


Operadores
< -> Redirige el input de un comando a un archivo
> -> Redirige el output de un comando a un archivo
| -> salida de un comando se pasa como entrada del siguiente

Operadores de control
& -> Realiza comandos asincronicamente en hilos de proceso
&& -> Encadena comandos y se detiene cuando uno fall
|| -> Encadena comandos no importa si alguno da error

Link simbolico
ln -s "ruta que queremos" "alias"

Permisos
chmod {u(+ ó -)x u(+ ó -)w u(+ ó -)r} modificar permiso de usuario para execute, write ó read
chmod {go(+ ó -)x go(+ ó -)w go(+ ó -)r} modificar permiso de global o others para execute, write ó read