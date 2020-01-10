##¿Qué es el bash?

Interprete de comandos que ejecuta de una en una las instrucciones ingresadas por el usuario o por medio de un script devolviendo resultados,  
es decir funciona como una interfaz entre el Kernel de Linux y los usuarios o programas del modotexto. Incorpora mejoras sobre su shell   predecesora (sh), al ser desarrollada por GNU se incorpora por defecto en las distros actuales.

## ¿Qué es shell?  

El shell es la parte de un sistema operativo que se encarga de ejecutar ordenes básicas para el manejo de este, algunas características de un   shell son control de procesos, redirección de entrada/salida y lenguaje para escribir ordenes por lotes (scripts).  

## ¿Qué fue lo mas difícil sobre este tema?  

Las operaciones con archivos en diferentes ramas de directorios.  

## ¿Pudiste usar todos los comandos del bash?  

Pude usar la mayoría de los comandos del bash que se observaron.  

## En tu opinión, ¿Cuales son los comandos mas importantes de aprender y por qué?  

Considero que los más importantes son aquellos que se utilizan para moverse entre los diferentes directorios, así como los que se utilizan   
para crear, editar y eliminar archivos y directorios.  

## ¿Puedes recordar para que son los siguientes comandos?  

### pwd  

Print Working Directory, se utiliza para conocer la ubicación del directorio de trabajo actual.  

### ls    

Para mostrar los archivos y carpetas del directorio actual.   

### mv  

Se utiliza para mover archivos y directorios de lugar, asi como para renombrar estos, ejemplos tomados desde  
https://www.comoinstalarlinux.com/mv-linux/:  

Cambiar el nombre de un archivo  
$ mv nombre1.txt archivo1.txt  

Renombrar un directorio  
$ mv directorio nueva-carpeta  

Mover archivos de ubicación  
$ mv archivo1.txt ./nueva-carpeta  


### cd  
Change Directory, cambiar directorio ejemplos de uso tomados desde https://www.comoinstalarlinux.com/comandos-linux-cd/:  

cd sin argumentos dirige al directorio por default de usuarios, /home/usuario donde «usuario» es el nombre de usuario con que ingresaste a tu sistema linux.  

cd indicando el directorio al que se desea cambiar  
$ pwd  
/home/user  
$ cd Descargas  
$ pwd  
/home/user/Descargas  

Para cambiar a otro directorio estando en otra subcarpeta diferente se puede indicar la ruta completa de la forma:  
$ pwd  
/home/user/Descargas  
$ cd /home/user/Documentos  
$ pwd  
/home/user/Documentos  

Otra hacer lo mismo es indicar el directorio anterior y luego al que deseas llegar, así:  

$ pwd  
/home/user/Descargas  
$ cd ../Documentos  
$ pwd  
/home/user/Documentos  

Otro ejemplo:  
$pwd  
/home/user  
$ cd /etc/cron.daily/  
$ pwd  
/etc/cron.daily  

Ejemplo estando en /home/user y cambiando al directorio /etc/cron.daily  
$cd /var/cache/apt  
$ pwd   
/var/cache/apt  

../  
Regresar al nivel inmediato superior del directorio  

### touch  
Crea un archivo vacío, si el archivo existe se actualiza la hora de modificacion; ejemplo creando el archivo prueba.txt  
en el directorio home:  
$ touch /home/prueba1.txt  

### mkdir  
Make Directory, se utiliza para crear un directorio  

### less    
Para mostrar texto en la pantalla de la terminal, muestra el contenido de un archivo linea por linea y no se puede editar el texto.  
Sintaxis:  

Less[modificadores] nombre_de_archivo  

Modificadores u opciones:  
  
-c Limpiar la pantalla antes de mostrar  
+n Inicia el archivo desde un numero dado  
:p Examina el archivo previo  
:d Elimina el archivo actual de la lista de archivos  
e  Adelante una línea (o N líneas).  
-S Deshabilitar auto-ajuste de líneas (las líneas largas serán visibles por navegación lateral).  
-g Solo se resalta la coincidencia actual de cualquier texto buscado.  
-M Mostrar datos de navegación  
ng Saltar a línea número n.  
=  (signo igual) Información del archivo en curso.  
h  Ayuda (help)  
q  Salir  

Ejemplo:  
Less +3 index.php : Muestra el archivo empezando por la tercera líneas  
less -M readme.txt : Lee archivo “readme.txt”.  
file * | less : Facilitar analisis de archivos.  
grep -rin void *.* | less -SI -p void : Facilitar la búsqueda de “void”.  

### rmdir  

rm  
Eliminar directorios  

Eliminar un directorio vacio:     
$ rmdir nombreDirectorio  

Si el directorio contiene archivos o subdirectorios, rmdir no lo eliminará.  

Se debe usar rm -r (agregando la opción recursiva -r al comando rm) para eliminar un directorio y su contenido, incluyendo cualquier   subdirectorio y sus archivos, del modo siguiente:  

$ rm -r nombreDirectorio  


### help  

El comando de ayuda se utiliza para encontrar informacion acerca del uso y sintaxis de otros comandos, tambien muestra información en linea sobre los comandos disponibles y el entorno de shell.   