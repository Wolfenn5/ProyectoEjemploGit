# **Practica 1: Introduccion a Git**

## **Descripcion**

El script de HolaMundo.py imprime un mensaje en terminal
    
    Hola Git

Mientras que el objetivo de la practica tiene como fin aprender a utilizar los comandos basicos de Git desde iniciar un repositorio remoto y local hasta hacer commits y subir los cambios realizados al repositorio remoto.

## **Instrucciones de uso**

Para ejecutar el programa *HolaMundo.py* desde visual studio code, en la esquina superior derecha hay un simbolo de flecha similar a *"play"* con la leyenda *Run Python File*. Se da clic en el boton y se ejecutara el programa HolaMundo.py de Python.

## **Comandos utilizados**

**Primer comando:** 

    git init

Se utilizo para inicializar el repositorio de Git.

**Segundo Comando:** 

    git add HolaMundo.py

Se utilizo para subir el archivo *HolaMundo.py* al area de preparacion, aunque este puede ser reemplazado por cualquier nombre del archivo que se desee subir o utilizar un punto de la forma **git add .** para subir todos los archivos.


**Tercer Comando:**

    git commit -m "Se agrego el programa de Hola Mundo en Python"

Se utilizo para hacer un commit donde -m indica que ira con un mensaje, en este caso *"Se agrego el programa de Hola Mundo en Python"*.

**Cuarto Comando:**

    touch debug.log

Se utilizo para crear un archivo de prueba *debug.log*.

**Quinto Comando:**

    touch .gitignore

Se utilizo para crear el archivo .gitignore.

**Sexto Comando:** 

    git add .gitignore

Se utilizo para mandar el archivo .gitignore al area de preparacion.

**Septimo Comando:**

    git commit -m "Se agrego el archivo .gitignore"

Se utilizo para hacer un commit donde -m indica que ira con un mensaje, en este caso *"Se agrego el archivo .gitignore"*.

**Octavo Comando:**

    git status

Se utilizo para verificar que el archivo debug.log sea ignorado y no aparezca en la lista de archivos no rastreados.

**Noveno Comando:**

    git add HolaMundo.py

Se volvio a utilizar ese comando ya que se realizo un cambio en el archivo *HolaMundo.py* con el fin de guardar los cambios hechos en el archivo y mandarlos al area de preparacion.

**Decimo Comando:**

    git commit -m "Se actualizo el mensaje en HolaMundo.py"

Se utilizo para hacer un commit donde -m indica que ira con un mensaje, en este caso *"Se actualizo el mensaje en HolaMundo.py"*.

**Onceavo Comando:** 

    git remote add origin https://github.com/Wolfenn5/ProyectoEjemploGit.git

Se utilizo para conectar el repositorio local creado con el primer comando al repositorio remoto de la direccion indicada. Donde *origin* solo funge como un *ALIAS*. Por convencion se suele utilizar **_origin_**. Y donde master indica la rama del repositorio (principal).

**Doceavo Comando:**

    git push origin master

Se utilizo para subir los cambios realizados al repositorio remoto.

**Treceavo Comando:**

    touch README.md

Se utilizo para crear el archivo README y utilizarlo con lenguaje markdown.

## Notas sobre el archivo .gitignore

Este archivo se creo con el fin de ignorar todos los archivos con extension .log. Aunque tambien se pueden agregar mas tipos de archivos que se desee ignorar como archivos temporales, binarios, compilados etc.

Lo que hace util a este archivo es que cuando se realicen cambios y commits, los archivos que se indiquen seran ignorados y no seran enviados tanto al area de preparacion como al repositorio remoto.

Para el caso de la practica solamente contiene un comentario y la siguiente linea para indicar que ignore todos los archivos de extension:

    *.log

Para comprobar que el archivo debug.log no se subio al repositorio se utilizo el comando **git add .** para indicar que se suban todos los archivos ("incluyendo *debug.log*"). Al subir todos los cambios con los comandos correspondientes incluyendo este README.