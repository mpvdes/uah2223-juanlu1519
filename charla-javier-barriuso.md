# Taller Javier Barriuso (Barri)

[Twitter Javier Barriuso](https://twitter.com/BarriPdmx)
[Telegram](t.me/BarriPdmx)

## Gephi

Nodos = cuentas

Aristas = conexiones entre cuentas

### Extracción de datos

Los datos podemos encontrarlos en:

- [Github de Mariluz Congosto](https://github.com/congosto) T-hoarder para poder extraer datos de Twitter, pedirselos a la API de Twitter

### Estadísticas > Ejecutar modularidad

En el apartado Estadísticas. Lo que toquemos aquí lo modificaremos en el laboratorio de datos. Podemos exportar estos datos en formato tabla.

### Apariencia > Partición > Modularity Class

Darle color a cada cuenta. Estos colores se pueden cambiar pinchando en el color,

### Tamaño > Ranking > n_rts

Para filtrar por número de Retweets.

### Distribución > Force Atlas 2

Separa las comunidades que peor se llevan y une a las que más relación tienen.

### Mostrar etiquetas 

Para ver cuales son las cuentas que aparecen.

### Tamaño de nodos > Ranking > Grado de entrada

Cuanto más grande sea el nodo, más grande será la etiqueta.

### Evitar solapamiento

Abre los nodos para que no se solapen.

### Filtros > Topología > Componente gigante > "Arrastramos" a Consultas

Para eliminar del grafo los nodos aislados.

### Centrar el grafo

### Distribución > Rotar > Ponemos el ángulo que queremos

Para poner las cuentas de izquierda en el lado izquierdo.

### Previsualización > Exportar

Podemos imprimir el grafo en png, pdf, svg.

En "mostrar etiquetas", añadimos el nombre de las cuentas. También podemos modificar el tipo de letra, el tamaño, color de borde, etc.

## t-hoarder kit

Para la extracción de datos de twitter.

Tambien se puede hacer con [RStudio](https://github.com/congosto/t-hoarder_R)
