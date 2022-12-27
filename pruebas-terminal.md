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

mv: Mover un archivo o carpeta

mkdir: Crear un directorio

rm -rf: Eliminar

cd../: Ir hacia atrás en un directorio

env: Ver las variables de entorno

q: Comando útil para salir. También podemos usar :q

apt-cyg install: Para instalar lo que deseemos. Por ejemplo: apt-cyg install nano, para instalar nano. Al tener gemas también podemos usar gem install.

figlet: Útil para escribir ASCII. Por ejemplo: figlet "hola, mundo"

cowsay: En el mismo formato ASCCI, una vaca te dice el texto que le indiques

man: Para ver el manual de un programa

>>: Ponerlo al final de un archivo para crearlo

>: Para redirigir un archivo

wc -l + archivo: Indica cuantas líneas tiene el archivo
wc -c + archivo: Indica cuantos caracteres tiene el archivo
wc -w + archivo: Indica cuantoas palabras tiene
head +archivo: Indica qué categorías tiene el documento

head -10: Te muestra las 10 primeras líneas de un archivo
tail -10: Te muestra las 10 últimas

tldr cut: Sirve para cortar
cat + dos nombres de archivos: Para concatenar dos documentos

-a: Ver los archivos ocultos

## Vincular Cygwin con Github

git add: Añade todos los que no estén trackeados (con .)
git commit: -m + "texto" sube el archivo con los cambios que indicas 
git push: Publicas tus cambios locales

git status: Comprobar como está git

cat../.token: Te enseña el token
