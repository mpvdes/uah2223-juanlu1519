# Medios digitales

## Derechos de autor y Licencias

El software libre cumple estas cuatro libertades:

- Libertad de uso
- Libertad de estudio -> Código fuente (la receta de un programa) abierto, *open source*
- Libertad de distribución
- Libertad de modificar y publicar las modificaciones

Todo software que no sea **software libre**, que no cumple las libertades anteriores, es **software privativo**.

### Derechos de autor

El autor es quien crea una obra.
- Lo es por el hecho mismo de **crear**
- No es necesario ningún trámite
- Ni siquiera tiene que publicarla
- Puede modificarla
- Adquiere **derechos de autor**

Los derechos de autor:
- Se consideran uno de los **derechos humanos fundamentales**
- Son derechos **morales** (reconocimiento de la autoría y potestad de preservar la integridad de la obra (plagio)) y **patrimoniales** (la infracción más común es la de uso o explotación no permitidas)
Los derechos morales son inalienables, irrenunciables, inembargables e imprescimptibles. Los derechos patrimoniales se refieren al derecho de explotar/usar la obra; se pueden ceder, vender, compartir e, incluso, renunciar a ellos; son prescriptibles y cuando prescriben pasa a dominio público.

#### Efecto

No tenemos ningún derecho sobre obras de terceros.

- No podemos decir que es nuestra si no lo es.
- No podemos ocultar la autoría original.
- No podemos usarla sin permiso.
- No podemos compartirla/distribuirla/reproducirla públicamente
- No podemos explotarla económicamente

Excepciones:

- Cita, crítica, parodia
- Uso con fines educativos o fines exclusivamente privados
- En beneficio de personas con discapacidad y sin fines educativos
- Obras situadas en la vía pública

#### Subjetividad

¿Quién decide que es cita, parodia...?

#### Más de un autor

Un problemón, andar con cuidado.

### Licencia

Contrato por el cual una persona recibe un derecho sobre un bien.

- Contrato privado
- Entre el titular de los derechos y un tercero
- Se estipulan las condiciones de cesión de ciertos derechos patrimoniales sobre una obra
- Puede estipularse una contraprestación económica y condiciones/limitaciones al uso de la obra
- Tiene validez legal y se puede incurrir a incumplimiento de contrato

#### Copyright

Es la más restrictiva de todas

#### Dominio público

Ningún derecho reservado, lo menos restrictivo

#### Copyleft

Un grupo de licencias que están en medio de las dos anteriores, algunos derechos reservados. Las más conocidas:

- Creative Commons
- Coloriuris
- Arte Libre
- GNU Free Documentation License (GFDL)

##### Creative Commons

Es fácilmente entendibles (iconos, texto simplificado y texto legal completo, organización de **aplicación internacional** sin fines de lucros creada en EEUU en 2002. Es la más usada. Restringe la autoría, explotación económica/comercial, modificación de la obra y relicenciamiento.
![Tipos de licencias Creative Commons](https://i0.wp.com/biblioteca2.uc3m.es/investigacion/wp-content/uploads/sites/9/2018/04/Creative_Commons_combinaciones.jpg)

## Introducción al diseño gráfico

### Color y modelos de color

El color es una percepción visual que se genera en el cerebro al interpretar las señales nerviosas que le envían los fotorreceptores de la retina del ojo y que a su vez interpretan y distinguen las distintas longitudes de onda que captan de la parte visible del espectro electromagnético.

Es algo subjetivo y difícil de describir y representar.

#### Modelos de color comunes

- RGB: red, green and blue. Para dispositivos que emiten luz.
- CMYK: Cyan, magenta, yellow and key. Para colores impresos.

### Formatos gráficos y tipos de archivos

#### Tipos gráficos

- Mapa de bits: píxel.
- Vectorial
- Mixtos

#### Propiedades de las imágenes

- Tamaño: se mide en píxeles.
- Peso: lo que ocupa en disco.
- Resolución: son metadatos, información que se almacena con la imagen. Se puede variar sin que varíe la imagen.

#### ¿Cómo guardar una imagen Bitmap?

- Sin comprimir
- Comprimiendo
1. Con pérdida
2. Sin pérdida

#### Formatos gráficos Bitmap/Raster más comunes
RAW, BMP, JPG, GIF, PNG, TIFF, PDF, XCF.

#### Formatos gráficos vectoriales más comunes
SVG, PS/EPS, PDF, AI, FHP/FH10/FH11...

## GIMP

### Teclas y tareas imprescindibles

- CTRL
- ALT
- SHIFT

Y sus combinaciones entre ellas: CRTL + Shift, ALT + Shift...

- Escalar imagen: Imagen > Escalar la imagen... Puedo ponerlo, por ejemplo, a la mitad si pongo /2 al lado del número.
- Deshacer: CTRL + Z
- Herramienta recortar: si hago CTRL + SHIFT recorto de manera proporcional. Enter para quedarme con el recorte.
- Herramienta de medida: para rotar y enderezar la imagen
- Rotar: Imagen > Transformar > Rotar. También puedo voltearla horizontalmente, verticalmente...
- Herramienta transformación libre: Ejemplo, poner una imagen en marquesina.
- Herramientas de pintura.
- Guías: Imagen > Líneas guía

## INKSCAPE

Programa de edición de vectores gráficos parecido a Adobe Illustrator.

No genera archivos CMYK. Blender, Scribus y Cyan Software Profile para suplir las carencias.

Paletas improtantes: Relleno y borde, patrón a objetos (capas), alinear y distribuir.

Combinaciones con CTRL, SHIFT, ALT y ESPACIO.

Gradientes

Importar imagen web: Archivo > Importar imagen web...

Duplicar: CTRL + D, no hace falta cortar y pegar. También puedo clonar (Edición > Clonar > Crear clon), y si modifico el padre se modifican el resto de figuras clonadas.

En *Trayecto* tengo varias opciones para unir, diferenciar, etc.

## AUDIO DIGITAL

El oído humano solo percibe sonidos entre 20hz y 20.000hz.

La **frecuencia de muestreo (sample rate)** es cada cuánto tiempo se toma una muestra del valor de la señal analógica. Se mide en hertzios (Hz).
Ej: 44.100 Hz, en 1 segundo se toman 44.100 muestras. Cuanto mayor es, más calidad.
La **velocidad de transmisión (Bitrate)** es la cantidad de espacio físico en bits (peso) que ocupa un segundo de duración de ese audio. Se mide en kBits/seg.

Bitrate constante CBR o variable VBR.

### HERRAMIENTAS INTERESANTES EN AUDACITY

- Reducción de ruido
- Herramienta de envolvente
- Pestaña efecto

## OPENSHOT

### FORMATOS MÁS USADOS

- .mp4
- .avi
- .mkv

### CÓDECS

- h264
- h265
- AAC (audio para vídeos de alta definición)

## LÍNEA DE COMANDOS

### SCRIPTS

Podemos acabarlos en .sh para saber que es un script o añadir una "," al inicio.

sh: ejecutar un script desde la terminal

chmod +x: para que me lo lea como script

#!/bin/bash: se añade al inicio del documento y la consola lo ejecuta con bash. Algunos empiezan con python en vez de bash

set -x : se puede poner justo después de bin bash para que te indique donde falla el script

$ : para indicar parámetros, variables.  Ej: convert "$1" "archivo.png"

exit 0 : se añade en el tecto para finalizar un script

; para concatenar tareas

&& para concatenar tareas si funciona la primera tarea. Ej: sleep 3s && ls

|| ejecuta mi script, y si da error, ejecuta la siguiente tarea. Ej: script.sh || ls

> para mandar un script a un documento de text, por ejemplo.

>> para mandar un script a un texto añadido a los anteriores textos

wc -l : me cuenta las lineas de un texto o directorio. Ejemplo: cat archivo.txt | wc -l

grep : para buscar palabras en mi texto. Ej: cat archivo.txt | grep primer. Me aparecen todas las líneas donde está la palabra "primer"

export PATH=$PATH:/rutademisscripts : para meter la carpeta donde tengo los scripts. Debería modificarlo en .bashrc para que fuera permanente.


## Recursos y otros enlaces

[Programa ilustración Krita](https://krita.org/es/)
