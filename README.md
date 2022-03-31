[img1]: https://github.com/Grxbriel/Ejercicio-de-clase-2-SI/blob/850d45e9176a8bb6298851118ff2b02d1d3eb877/1.png "Imagen1"
[img2]: https://github.com/Grxbriel/Ejercicio-de-clase-2-SI/blob/65bedacd2c7937958f57fddd16a6f8cf012bf221/2.png "Imagen2"
[img3]: https://github.com/Grxbriel/Ejercicio-de-clase-2-SI/blob/65bedacd2c7937958f57fddd16a6f8cf012bf221/3.png "Imagen3"
[img4]: https://github.com/Grxbriel/Ejercicio-de-clase-2-SI/blob/1b3c33dfc0cecd32d9d3a38d876473169fef9b9b/4.png "Imagen4"

# 💻 Ejercicio-de-clase-2-SI
---
## 1️⃣ EJERCICIO 1

**1. Crea la siguiente estructura de carpetas:**

Nos situamos en el directorio `C:\Users\gabri\Documents\DAM\Sistemas Infórmaticos\Ejercicio-de-clase-2-SI` y mediante `MD "", CD y CD..` creamos los directorios

![Imagen 1][img1]

**2. Sitúate en la carpeta TABLAS**
~~~
CD APLI/EXCEL/TABLAS
~~~
**3. Vuelve a la carpeta raíz**
~~~
CD..
~~~
**4. Muestra el contenido de la carpeta PROG**
~~~
CD PROG
DIR
~~~
![Imagen 2][img2]

**5. Borra la carpeta PASCAL**
~~~
RMDIR PASCAL
~~~
![Imagen 3][img3]

**6. Sitúate en la carpeta VARIOS y desde allí crea una nueva carpeta dentro de WORD llamado PRACT**
~~~
CD VARIOS
CD.. && CD APLI/WORD && MKDIR PRACT
~~~
Y luego usamos el comando `ls` para ver el contenido de la carpeta WORD

![Imagen 4][img4]

**7. Sitúate en PRACT y desde allí muestra el contenido de la carpeta EXCEL**

~~~
CD APLI/WORD/PRACT
CD.. && ls ./EXCEL
~~~

**8. Desde TABLAS muestra el listado de archivos y carpetas de la carpeta raíz**

~~~
Ejercicio-de-clase-2-SI\APLI\EXCEL\TABLAS> ls ../../..
~~~

**9. Sitúate en la carpeta APLI y desde allí crea una subcarpeta llamada AGENDA dentro de VARIOS**

~~~
CD APLI && CD.. && MKDIR VARIOS/AGENDA
~~~

**10. Borra la carpeta EXCEL**

~~~
Ejercicio-de-clase-2-SI> RMDIR APLI/EXCEL
~~~

**11. Desde la carpeta raíz, crea en ella una subcarpeta llamada NUEVO**

~~~
Ejercicio-de-clase-2-SI> MKDIR NUEVO
~~~

**12. Desde PRACT muestra el contenido de WORD**

~~~
CD APLI/WORD/PRACT/ && ls ..
~~~

## 2️⃣ EJERCICIO 2

**1. Utilizando el editor de textos de MS-DOS, crea un archivo de texto denominado EJER.TXT, con el siguiente contenido, y almacénalo dentro de la carpeta TEXTOS (dentro de la estructura del ejercicio anterior):**

>"La información dentro de los discos se almacena en forma de archivos. Un archivo o fichero es un conjunto de datos que MS-DOS almacena en un disco y cuyo control interno es realizado por el sistema operativo, aunque desde el punto de vista lógico el control es del usuario"

~~~
NEW-ITEM ejercicio.txt

SET-CONTENT ./ejercicio.txt

MV ejercicio.txt ./APLI/WORD/TEXTOS
~~~


**2.Copia el archivo EJER.TXT en AGENDA**

~~~
CD ../../.. && CP APLI/WORD/TEXTOS/ejercicio.txt VARIOS/AGENDA
~~~

**3. Borra el archivo almacenado en la carpeta TEXTOS.**

~~~
rm -r APLI/WORD/TEXTOS/
~~~

**4. Añade el siguiente párrafo al archivo EJER.TXT:**

>"Cada archivo tiene un nombre y una extensión que los distingue del resto de archivos"

~~~
SET-CONTENT ejercicio.txt

cmdlet Set-Content at command pipeline position 1
Supply values for the following parameters:
Value[0]: La información dentro de los discos se almacena en forma de archivos. Un archivo o fichero es un conjunto de datos que MS-DOS almacena en un disco y cuyo control interno es realizado por el sistema operativo, aunque desde el punto de vista lógico el control es del usuario
Value[1]: Cada archivo tiene un nombre y una extensión que los distingue del resto de archivos
~~~

**5. Copia el archivo EJER.TXT en la carpeta BASIC.**

~~~
CD ../.. && CP VARIOS/AGENDA/EJER.txt PROG/BASIC
~~~

**6. Cambia el nombre del archivo almacenado en AGENDA por FICHERO.TXT**

~~~
REN EJER.txt FICHERO.txt
~~~

**7.Mueve el archivo FICHERO.TXT a la carpeta BASIC**

~~~
CD ../.. && MV VARIOS/AGENDA/FICHERO.txt PROG/BASIC
~~~

**8. Abre el archivo EJER.TXT y borra la primera frase; almacena el nuevo archivo con el nombre NUEVO.TXT dentro de la carpeta BASIC.**

Se nos abrirá un editor de texto y eliminamos la primera línea del documento. Después cambiaremos el nombre del fichero:
~~~
notepad.exe EJER.txt

Ren EJER.txt NUEVO.txt
~~~

**9. Copia el archivo NUEVO.TXT en la carpeta NOTAS.**

~~~
CD ../.. && CP PROG/BASIC/NUEVO.txt APLI/WORD/NOTAS/
~~~

**10. ¿Cuántos archivos hay en la carpeta BASIC? ¿Y en NOTAS?**

En la carpeta BASIC nos encontramos con 2 archivos y en NOTAS nos encontramos con 1 solo archivo.

## 3️⃣ Ejercicio 3
Borra la carpeta ACCESS y en su lugar crea una nueva carpeta llamada ASTRO

Puesto que ACCES es un directorio vacio bastara con realizar lo siguiente:

rmdir .\PARTE1\APLI\ACCESS\
A continuación realizamos el siguiente comando para crear la carpeta ASTRO:

mkdir .\PARTE1\APLI\ASTRO
Así quedará la estructura del directorio:

Ejercicio 3.1

Crea la siguiente estructura de subcarpetas dentro de la carpeta ASTRO.

Ejercicio 3.2

Para crear la estructura mostrada debemos hacer lo siguiente:

a. Primero nos movemos a la carpeta ASTRO:

  cd .\PARTE1\APLI\ASTRO\
b. Procedemos a crear la estructura de directorios:

mkdir HISTORIA
mkdir CIENCIA
cd .\HISTORIA\
mkdir DATOS1
mkdir DATOS2
cd ..\CIENCIA\
mkdir ASTRO1
mkdir ASTRO2
Después de hacer esto nos quedara la siguiente estructura:

Ejercicio 3.2.1

Sitúate en la carpeta CIENCIA y desde allí muestra el listado de archivos y subcarpetas de la carpeta HISTORIA

Primero nos ubicamos en la carpeta CIENCIA:

cd .\APLI\ASTRO\CIENCIA\
Después mostramos el listado de archivos y subcarpetas de HISTORIA con tree. Utilizamos el parametro /f para que muestre tambien los archivos:

tree /f ..\HISTORIA\
Esto nos mostrará lo siguiente:

Ejercicio 3.3

Utilizando el editor de MS-DOS crea el siguiente archivo de texto y guárdalo con el nombre TYCHO.TXT dentro de la carpeta DATOS1

“La importancia de Tycho Brahe (1546-1601) es debida a sus trabajos observacionales, que registraron posiciones notables del Sol, la Luna y los planetas”

Ubicados en la carpeta raíz realizamos el siguiente comando para crear el archivo con texto:

cd .\APLI\ASTRO\HISTORIA\DATOS1\
New-Item TYCHO.txt 
Set-Content .\TYCHO.txt
Con set-content se nos mostrará una interfaz donde podremos introducir el texto.

Utilizando de nuevo el editor de textos de MS-DOS crea el siguiente archivo de texto, y guárdalo con el nombre KEPLER.TXT dentro de la carpeta DATOS2

Set-Content -Path .\KEPLER.txt
Copia los archivos TYCHO.TXT y KEPLER.TXT en la carpeta CIENCIA

Primero copiamos TYCHO.txt:

copy ..\DATOS1\TYCHO.txt ..\..\CIENCIA\
copy .\KEPLER.txt ..\..\CIENCIA\
Y nos quedará una estructura de directorios así:

Ejercicio 3.6

Cambia de lugar los archivos almacenados en DATOS1 y DATOS2 de forma que TYCHO.TXT quede guardado dentro DATOS2 y KEPLER.TXT en DATOS1

Movemos KEPLER a DATOS1 desde la carpeta DATOS2:

  move .\KEPLER.txt .
Después movemos TYCHO a DATOS2 desde la carpeta DATOS1:

 move .\TYCHO.txt ..\DATOS2\
Crea un nuevo archivo formado por la unión de los dos anteriores (sin volver a escribir el texto) y guárdalo dentro de la carpeta HISTORIA con el nombre TOTAL.TXT

Desde la carpeta CIENCIA, donde estan alojados los 2 archivos que debemos unir ejecutamos lo siguiente:

type *.txt > nuevo.temp
ren .\nuevo.temp .\nuevo.txt
El archivo lo he creado en CIENCIA, por lo que lo movere a HISTORIA:

move .\nuevo.txt ..\HISTORIA\
Abre el archivo KEPLER.TXT almacenado en la carpeta CIENCIA y añade el siguiente texto:

“Kepler aplicó sus teorías a los satélites de Júpiter, descubiertos por Galileo a través de un pequeño telescopio, cuya introducción en la observación astronómica constituye uno de los hitos de la astronomía.”

Para ello realizamos lo siguiente:

echo "Kepler aplicó sus teorías a los satélites de Júpiter, descubiertos por Galileo a través de un pequeño telescopio, cuya introducción en la observación astronómica constituye uno de los hitos de la astronomía." >> .\KEPLER.txt
Cambia el nombre del archivo anterior por GALILEO.txt

ren .\KEPLER.txt .\GALILEO.txt
Y nos quedará una estructura de archivos y directorios así:

Ejercicio 3.10

Ejercicio 4
Crea en la carpeta raíz de la unidad A: una carpeta denominada TECINFO

mkdir A
mkdir .\A\TECNIFO
Crea dentro de TECINFO el siguiente archivo de texto y llámalo HARD.TXT

“El HARDWARE está constituido por los elementos físicos del ordenador. Consta esencialmente de componentes electrónicos que proporcionan el soporte necesario para la interpretación y ejecución de las operaciones elementales que realiza el ordenador”

Para hacer esto primero nos movemos a la carpeta TECNIFO y añadimos el texto con echo

cd .\A\TECNIFO\
echo "El HARDWARE está constituido por los elementos físicos del ordenador. Consta esencialmente de componentes electrónicos que proporcionan el soporte necesario para la interpretación y ejecución de las operaciones elementales que realiza el ordenador" > HARD.txt
Crea dentro de TECINFO el siguiente archivo de texto y llámalo SOFT.TXT

“El SOFTWARE es el conjunto de elementos lógicos necesarios para que el ordenador realice las funciones que se le encomiendan. Está formado por los programas, es decir, por un conjunto ordenado de instrucciones, comprensibles por la máquina, que permiten desarrollar tareas concretas”

echo "El SOFTWARE es el conjunto de elementos lógicos necesarios para que el ordenador realice las funciones que se le encomiendan. Está formado por los programas, es decir, por un conjunto ordenado de instrucciones, comprensibles por la máquina, que permiten desarrollar tareas concretas" > SOFT.txt
Mueve el contenido de TECINFO a la carpeta APLI del disquete A utilizado para realizar los ejercicios anteriores

Desde el disco A hacemos lo siguiente:

move .\TECNIFO\* ..\PARTE1\APLI\
Crea un nuevo archivo formado por la unión de HARD.TXT y SOFT.TXT, sin volver a escribir el texto, y guárdalo en la carpeta AGENDA con el nombre ORDER.TXT

Primero nos movemos a la carpeta APLI para luego unir los dos archivos de texto. Este archivo donde lo unimos tendrá la extencion .temp por lo que después lo renombraremos a ORDER.txt y finalmente lo moveremos a AGENDA.

cd ..\PARTE1\APLI\
type *.txt >nuevo.temp
ren .\nuevo.temp ORDER.txt
move .\ORDER.txt ..\VARIOS\AGENDA\
Elimina la carpeta TECINFO

Elimino la carpeta TECNIFO desde la APLI.

rmdir ..\..\A\TECNIFO\
Copia a la vez los archivos HARD.TXT y SOFT.TXT en la carpeta VARIOS

Ubicados en APLI movemos los dos archivos a VARIOS.

 move .\*.txt ..\VARIOS\
Cambia la extensión de los archivos contenidos en AGENDA por .TYP

Nos movemos a AGENDA y procedemos a cambiarle la extención:

cd ..\VARIOS\AGENDA\
ren .\ORDER.txt ORDER.typ
Cambia la primera letra del nombre de todos los archivos del directorio APLI que empiecen por la letra C y tengan extensión DOC de forma que empiecen con la letra S

Nos ubicamos en el directorio APLI y cambiamos los nombres de los archivos que coincidan:

cd .\APLI\
ren .\C*.doc S*.doc
Copia los archivos contenidos en la carpeta APLI que tengan extensión DOC en la carpeta AGENDA

Desde la carpeta APLI hacemos lo siguiente:

 copy *.doc ..\VARIOS\AGENDA\
