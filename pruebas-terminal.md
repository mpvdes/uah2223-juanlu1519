# Pruebas Cygwin

![Logo cygwin](https://w7.pngwing.com/pngs/157/78/png-transparent-kde-on-cygwin-computer-software-computer-icons-microsoft-angle-triangle-microsoft-thumbnail.png "logo de cygwin")

## Instalación de Cygwin

Primero de todo, hay que instalar el programa desde su página oficial https://www.cygwin.com/.

A la hora de instalarlo, tenemos que elegir el repositorio de descarga de los paquetes. Esto es una especie de servidor que nos permite descargar paquetes que necesitaremos en la terminal. Uno de ellos es nano.

## Primeros pasos
Hay que tener claro lo que son los comandos, las acciones y los argumentos.

Por ejemplo: Comando: lynx, Acciones: -source, Argumentos: rawgit.com/transcode-open/...

### Comandos útiles
ls: Enseña los archivos de una carpeta

pwd: Indica dónde estoy

cd: Cambiar directorio/entrar en carpeta

touch: Crear archivos vacíos

nano "pruebas.md": Se abre nano y crea/abre un archivo con ese nombre

history: Ver el historial de lo que hemos hecho en la terminal

less

more: Estos dos últimos son lectores de texto

echo: Este comando te devuelve lo escrito. Por ejemplo podemos usar echo $SHELL para saber cuál es nuestra shell.

mv: Mover un archivo a otro directorio. Ejemplo: archivo.txt/ ../carpeta1

mkdir: Crear un directorio. Por ejemplo, para crear una carpeta llamada mpvd en el directorio anterior: mkdir ../mpvd 

rm -rf: Eliminar

cd../: Ir hacia atrás en un directorio

env: Ver las variables de entorno

q: Comando útil para salir. También podemos usar :q

apt-cyg install: Para instalar lo que deseemos. Por ejemplo: apt-cyg install nano, para instalar nano. Al tener gemas también podemos usar gem install.

figlet: Útil para escribir ASCII. Por ejemplo: figlet "hola, mundo"

cowsay: En el mismo formato ASCCI, una vaca te dice el texto que le indiques

man: Para ver el manual de un programa

'>>': Ponerlo al final de un archivo para crearlo

'>': Para redirigir un archivo

wc -l + archivo: Indica cuantas líneas tiene el archivo

wc -c + archivo: Indica cuantos caracteres tiene el archivo

wc -w + archivo: Indica cuantoas palabras tiene

head +archivo: Indica qué categorías tiene el documento

head -10: Te muestra las 10 primeras líneas de un archivo

tail -10: Te muestra las 10 últimas

tldr cut: Sirve para cortar

cat + dos nombres de archivos: Para concatenar dos documentos

-a: Ver los archivos ocultos

-la: Listar todo, incluso archivos ocultos

wget enlaceimagen -O tituloimagenquequiero.png : Si quiero subir una imagen a Github desde mi repositorio debo hacer ese comando para guardar una imagen en el repositorio. Luego en nano escribo (./img(tituloimagenquequiero.png "descripciónimagen")

file: Te enseña todos los archivos. Si escribo, por ejemplo, file *.md, me enseña todos los que tienen formato .md

grep: Este comando es muy útil para filtrar palabras dentro de archivos o carpetas. Ejemplo: grep -rn \# pruebas-github.md . En este caso se nos muestra las veces que hemos puesto la almohadilla en ese archivo. Si lo quiero hacer en una carpeta: grep -rn \# ../uah2223-juanlu1519/: . Ponemos \ ya que es un caracter, en una palabra o frase no haría falta.

date: Para saber la hora con precisión

man comando o comando --help : Para saber más de ese comando

alias: Para asignarle un alias a lo que deseemos. Por ejemplo: python = python3 . Cada vez que escribamos python se "ejecutará" python3.

## Vincular Cygwin con Github

git add: Añade todos los que no estén trackeados (con .)

git commit: -m + "texto" sube el archivo con los cambios que indicas 

git push: Publicas tus cambios locales

git status: Comprobar como está git

cat../.token: Te enseña el token, que es la contraseña que te pide el programa para subir los cambios

git pull: Lo contrario a git push.


## Programas instalados en la terminal

Fortune

Lolcat

Rdoc

Free

## Guardar token para ver con el comando Echo

### Para guardar el token mientras no cierre la sesión:

1. Grabo el token. Ejemplo: GHT= 'token'

2. Busco el token. Ejemplo: echo $GHT

### Para que sea persistente

1. export GHT= 'token'
2. env | grep GHT
3. echo " export GHT= 'token' " >>~/.bashrc
4. tail -1 ~/.bashrc

## Permisos Linux

Cuando creamos un archivo o exploramos uno ya creado nos aparecen una serie de caracteres de este estilo: -rw-r--r--+1

- r: Significa que tenemos permisos de lectura

- w: Tenemos permiso para escribir

- x: En este caso tenemos permiso para ejecutarlo

Para cambiar estos permisos podemos:

- chmod u+x hola.sh : Al usuario le damos permisos de ejecución en este archivo.

- chown
