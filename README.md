# Shell
Programa en C que simula una Shell, y permite la ejecución de llamadas al sistema de Linux. El uso de las llamadas
al sistema es realizado mediante comandos.

El propósito específico de este proyecto es ilustrar las llamadas al sistema en Linux, además del manejo básico de
comandos y argumentos dentro de una consola de comandos.

## Compilación
Este proyecto fue diseñado para ser compilado y ejecutado en Linux, por lo que debes contar con este sistema operativo
para poder llevar a cabo los pasos que se describen a continuación.

Para compilar el programa, ejecutar el script de compilación:
```
./build.sh
```
El script creará un directorio dentro de la raíz del proyecto llamado 'build/', y dentro de él se encontrará el binario
'Shell'.

Para compilar manualmente:
```
cc src/main.c -I include/ -o Shell
```

## Ejecución
Para ejecutar la Shell, simplemente ejecutar el binario 'Shell'.
```
./Shell
```

## Comandos
Todos los comandos disponibles en la Shell:
  * `cwd`: Imprime en pantalla el directorio actual.
  * `seconds`: Imprime en pantalla la cantidad de segundos transcurridos desde el primero de Enero de 1970 (EPOCH).
  * `stats`: Imprime en pantalla el uptime del sistema, información de la RAM y procesos actuales.
  * `ls`: Imprime en pantalla los archivos del directorio en donde se ejecute.
  * `mkdir <path>`: Crea un nuevo directorio con el nombre del argumento 'path'. Por defecto, el directorio es generado
  dentro de la ruta donde se encuentre el usuario al momento de la ejecución del comando. Si 'path' contempla
  más de un directorio (a/b/c/dir) el directorio a generar será 'dir' en este caso, dentro de la ruta precedente.
    * path: Nombre del nuevo directorio.
  * `cd <path>`: Mueve al usuario dentro del directorio 'path'.
    * path: Nombre de la ruta a la cual el usuario desea moverse.
  * `Salir`: Termina la ejecución del programa.

## Comandos de Funcionalidades Extra
  * `MAKEITGOOD`: Activa un modo en que la Shell imprime con letras de un color aleatorio. Para desactivarlo basta con 
  usar el comando por segunda vez.
  * `JOKER`: Activa un modo en que la Shell imprime con fondo de un color aleatorio. Para desactivarlo usar el comando
  por segunda vez.
