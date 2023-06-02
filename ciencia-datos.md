# Técnicas de ciencia de datos

## Población y muestra

La población es todo el conjunto de elementos que queremos estudiar y la muestra es la selección que usaremos. A esto último se llama inferencia estadística.
Los caracteres pueden ser cualitativos (color de pelo de unas personas) o cuantitativos (altura de niños).

## Variables estadísticas

Variables discretas: sabemos que solo pueden ser enteros: dedos de una mano, hijos...
Variables continuas: conjunto no numerable: diámetro de una pieza, números float...

## Frecuencias

### Frecuencia absoluta

Cantidad de valores de un objeto. Por ejemplo: 6 manzanas, 2 peras, 9 fresas y 1 kiwi.

### Frecuencia absoluta acumulada

Consiste en ir sumando las frecuencias absolutas. Con el ejemplo anterior:

6+2 = 8 -> 8 + 9 = 17 -> 17 + 1 = 18

### Frecuencia relativa:

Corresponde a las veces que se repite un número en un conjunto de datos respecto al total. Se expresa en porcentajes respecto a 1.

### Frecuencia relativa acumulada:

La suma de las frecuencias relativas.

## Distribuciones

Los datos hay que distribuirlos. Se representan mediante tablas.

Sin agrupar: cuando aparecen los datos con sus frecuencias, cuando tenemos pocos valores distintos.

Agrupados en intervalos: cuando los dividimos por clase. Ejemplo: edades de 10-19, 20-29... Tienen que ser todos iguales. Que no haya una clase con muchos elementos, habrá que ajustar los intervalos. El número de intervalos es K, ej K5. A cada extremo de esos intervalos se le llama **límite de clase**. Puede ser superior o inferior. La **marca de clase** es el punto medio de ese intervalo de clase.**La amplitud de clase** es la diferencia entre límites. Se señala con "a".

## Representación gráfica

### Diagrama de barras

![Diagrama de barras](https://www.jmp.com/es_co/statistics-knowledge-portal/exploratory-data-analysis/bar-chart/_jcr_content/par/styledcontainer_2069/par/image_1203777138.img.png/1594745267192.png)

### Polígono de frecuencias

![Polígono de frecuencias](https://media.gcflearnfree.org/content/61d5c217c4da77185ca9f229_01_05_2022/Co%CC%81mo-usar-un-poli%CC%81gono-de-frecuencias-1.png)

### Diagrama de frecuencias acumuladas

![Diagrama de frecuencias acumuladas](https://www.uv.es/ceaces/base/descriptiva/ejemplos/representa3.gif)

### Histograma

![Histograma](https://asolengin.files.wordpress.com/2014/10/histograma-1.jpg?w=640)

La diferencia con el diagrama de barras es: si hay intervalos, histograma.

### Polígono de frecuencias acumuladas

![Polígono de frecuencias acumuladas](https://www.superprof.es/diccionario/wp-content/uploads/2020/01/pol%C3%ADgono-de-frecuencias-acumuladas-1.gif)

### Diagrama de sectores

![Diagrama de sectores](https://images.nagwa.com/figures/686165050125/1.svg)

### Pictogramas

![Pictogramas](http://1.bp.blogspot.com/-HuZopeK8BvA/UACuwsg1XWI/AAAAAAAABQU/tFbADOdfWkQ/s320/Pictograma.jpg)

O los típicos gráficos que se representan con personas/monigotes.

### Cartogramas

![Cartogramas](http://www.cursosgis.com/wp-content/uploads/2017/02/cartogramas_qgis_1.png)

También conocido como "mapa temático".


## Medidas de centralización

### Media aritmética

Suma todas las frecuencias  y dividirlo por el número de valores. La media de las diferencias a la media, es nula, es decir 0. La suma de los cuadrados de esas diferencias es mínima. Se puede ver afectado por los outlyers.

### Mediana

Valor de la variable que ocupa el lugar central. F(M) = 1/2

### Moda

El valor que más se repite. En las agrupadas, la clase modal es la que tiene más frecuencia. Puede que no sea un valor único, podemos tener más de una moda.

### Cuantiles

Es un valor que deja a su izquierda un valor alfa y a su derecha, 1 - alfa.

Dentro están los cuartiles: 25 (Q1), 50(Q2), 75(Q3). Se representa con Q.

Deciles: se representan con D.

Percentil: P1, 2, 3... P99. El 50 es la mediana. Se representan con P.

Entre todos forman los cuantiles.

## Medidas de dispersión

### Rango o recorrido

La distancia que hay entre el mínimo y el máximo. Ejemplo (8,5,6,3,1,8) sería 8-1 = recorrido 7.

### Recorrido semi-intercuartílico

Diferencia entre cuartiles Q1 y Q3, dividido entre 2. (Q3-Q1)/2. Ejemplo (1,1,3,5,7,8,8). 5 sería la mediana. 1 el Q1, 8 el Q3, el recorrido semi-intercuartílico sería 3,5. La media sería 4,7.

### Varianza

![Varianza](https://www.sage.com/es-es/blog/wp-content/uploads/sites/8/2021/07/Varianza_1.jpg)

Media de los cuadrados de las desviaciones a la media.

#### Varianza muestral o cuasivarianza

Media de los cuadrados de las desviaciones a la media -1.

### Desviación típica

Es la raiz cuadrada positiva de la varianza.

### Desviación típica muestral

Es la raíz cuadrada positiva de la varianza muestral.

### Coeficiente de variación de Pearson

Es el cociente entre la desviación típica y la media.  

## Características de forma

### Sesgo

Simétrica, asimétrica, sesgado (hacia la izquierda o a la derecha).

Si sumamos las desviaciones al cubo3 y nos da 0, es simétrica. Si es positivo, está sesgado a la derecha, si es negativo, a la izquierda.

#### Coeficiente de Fisher

### Curtosis

Podemos ver si está muy apuntado o poco apuntado.

![Curtosis](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcT1n1f_pfBRWXsET7Zk8UbRnzKLDPqsBs5ESL_uh9aKmlDcIpkO)

Si da 0 es normal.

### Momento

Sirven para simplificar cuentas.

## Variables estadísticas bidimensionales

Si llamamos  E a la población, una variable estadística bidimensional es una aplicación de  E → R2

Los resultados se disponen en una tabla de doble entrada (o de contingencia).

### Distribuciones marginales

El centro de gravedad  es la media entre x marginal e y marginal.

![Tabla de doble entrada](https://i.ytimg.com/vi/asnxuGOzX5k/maxresdefault.jpg)

Estos también pueden representarse en gráficos, llamados diagrama de dispersion o nube de puntos.

![Diagrama de dispersión](https://www.ingenioempresa.com/wp-content/uploads/2016/07/Ejemplo-diagrama-de-dispersi%C3%B3n.png)

### Momentos

Fórmula para sacar medias, varianzas, etc.

### Covarianzas

σxy recibe el nombre de covarianza, de gran importancia práctica, se define como la media aritmética de los productos de las desviaciones de la variable x con respecto a su media aritmética, X, por las desviaciones de la variable y con respecto a la media aritmética, Y.

Es como un valor conjunto para las dos, como varian dos juegos de datos.

### Matriz de covarianzas

Es la matriz cuadrada simétrica que tiene en la diagonal principal las varianzas marginales, y fuera de la diagonal principal, las covarianzas.

![Matriz de covarianzas](https://economipedia.com/wp-content/uploads/Captura-de-Pantalla-2019-09-23-a-les-16.23.40.png)

Se llama varianza generalizada al valor |M| = S2x S2y - S2xy >0 y mide aproximadamente al área ocupada por el conjunto de datos.

## Regresión y correlación

En las distribuciones bidimensionales se presentan dos problemas que dan origen a dos teorías:

- Teoría de la **regresión**, que trata de predecir los valores de una variable para valores prefijados de la otra.

- Teoría de la **correlación**, que trata de medir la independencia estadística entre dos variables.

Puede haber diveros tipos de dependencia:

- Dependencia **funcional**, como por ejemplo entre el tiempo y espacio recorrido por un móvil, con una expresión matemática que las relaciona.

- Dependencia **aleatoria**, donde no podemos saber exactamente el valor de la otra, pero sí una idea aproximada, como la relación entre talla y peso de una persona.

### Línea de regresión

Un **ajuste** es la sustitución de un diagrama de dispersión por una línea que, sin que deba pasar por todos los puntos, se adapte lo mejor posible a todos ellos. La función que pretendemos obtener será una línea que llamaremos **línea de regresión**, cuya ecuación puede ser de las formas siguientes:

#### Recta

![Recta regresión](https://ekuatio.com/wp-content/uploads/recta-de-regresion-12-1.png)

#### Parábola

![Parábola regresión](https://3.bp.blogspot.com/-hK_fCWFd3Ko/TsG61j3vMtI/AAAAAAAAAPk/d18NoVeJuoM/s1600/10.PNG)

#### Polinómica

![Regresión polinómica](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8b/Polyreg_scheffe.svg/325px-Polyreg_scheffe.svg.png)

#### Exponencial

![Regresión exponencial](https://www.varsitytutors.com/assets/vt-hotmath-legacy/hotmath_help/topics/exponential-regression/f-er-1-1.gif)

#### Hipérbola

![Regresión hipérbola](https://www.geogebra.org/resource/V2P2az6u/Flu6VVjSfeoh188z/material-V2P2az6u.png)

### Ajuste de los mínimos cuadrados

La recta que nosotros buscamos, la suma de todas las diferencias sea la mínima. Vamos a ajustar esa línea para que nos salga la que los puntos estén más cerca de esa línea.

![Mínimos cuadrados](https://upload.wikimedia.org/wikipedia/commons/9/94/Linear_least_squares2.png)

### Coeficiente de correlación lineal

Para calibrar dicho ajuste. Cuando hagamos esa cuenta debe salirnos entre -1 y +1. Si nos sale 1 es perfecta y directa. Si nos sale -1, la correlación es perfecta e inversa. Si nos sale 0, no hay correlación, están incorreladas. Cuanto más se acerque al 0, más mala es la correlación.

![Coeficiente correlación](https://i.ytimg.com/vi/aKsjilxc5ww/maxresdefault.jpg)

El que dos variables tengan una correlación lineal alta (sea positiva o negativa) puede no significar una relación causa-efecto entre ellas; entre la longitud de los pantalones y la capacidad de leer en los niños de edades comprendidas entre 5 y 9 años existe una correlación alta, los niños de 5 y 6 años leen mal y es frecuente que utilicen pantalón corto, mientra que los niños de 8 y 9 años es frecuente usar pantalones largos y leen bastante bien. ¿Se mejoraría el nivel de lectura entre los niños de 5 y 9 años si todos usasen pantalones largos? En general, hay que tener cuidado al interpretar r.

## Apuntes básicos R

[Apuntes básicos de R, por Alejandro Zappala](https://alayzappala.gitlab.io/apuntes-ciencia-datos/rudimentos-de-r.html)

## Introducción al análisis de redes (sociales)

[Apuntes Introducción al análisis de redes (sociales)](https://alayzappala.gitlab.io/introduccion-al-analisis-de-redes)

### Teoría de grafos

Lo forman nodos (personas) y enlaces/aristas (relaciones o flujos entre nodos).

Pueden ser conexos o inconexos.

### Introducción

- Las redes sociales no son la web. No son el mundo real pero sí un reflejo.

- Los motores de búsqueda tampoco son la web.

- La web no es internet.

- Internet no es lo digital.

- Lo digital no es el mundo.

Las relaciones entre nodos pueden ser simétricas y asimétricas.

### Scrapping y data mining

#### Scrapping

- [Data miner](data-miner.io)

- [Tabula](tabula.com)

- Mediante programación: Python y R.

- APIs de webs y redes sociales.

#### Varios tipos de herramientas

- OpenRefine

- Bloc de notas

- Editores de tablas (excel, libreoffice)

- Con terminal (Bash, Python, R)

### Análisis de los datos

- Tableau

- Datawrapper

- Gephy

- Infogram

- Dipity

- Google Fusion Tables

- Gapminder

- Linkurious

- HYPHE

- Sigma

### Toma de decisiones

¿Son suficientes datos? ¿Son fiables? Repetit el proceso con otras palabras clave y combinaciones. Repetir el proceso con resultados en otro idioma. 

### Documentar el proceso

- Git

- Documentar procesos de análisis

- Indicar origen de las fuentes 

- Máximos detalles posibles

- Formatos abiertos

### Redacción y publicación de resultados

Tener en cuenta el medio donde se va a representar

## Recursos
[Apuntes ciencia de datos](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/5d1f8301cf6a3/13899773?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1680220800000&X-Blackboard-Signature=PD8Fk7l2pcatdQpgtva6j58IiHzGO3XirKUQHgrJny0%3D&X-Blackboard-Client-Id=309366&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%2701-Estad%25C3%25ADstica-descriptiva.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEKL%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaDGV1LWNlbnRyYWwtMSJIMEYCIQD0aky8uwWYDWgv%2Be6ggep45w9XbYotspozS%2BbxT8ULuwIhAK1e%2Fp%2FLao6EJeLfAg7jNzY1XBKKcAS5mJm4h%2BHb18FRKr4FCHsQAxoMNjM1NTY3OTI0MTgzIgzI%2F64YPBtkfh1XWyEqmwVnqNNQ4YSGtbHbA8pZNGEv9GvhjuBbIBijah2iDNcz%2Fsn8xvMy9xjIYs53hoj41LtSR7y5hyh11FKpNvqAsb0vDjzM6a0LILxe%2F%2FE3g6bm7nGvqrQp46ORkQDCWg70BCAl9gUTQ8BoC%2BqAESELjFH8cIcQtKfVxR4k%2BLVyK949fT%2B8PcmCEcycEMlUhnCR92y3xStADa2AG1V2lFA8V889Jwjw26nb7hpKOPQomK3uCaMmsjxf3tC%2F6fTsg2PtLKqJAQrAK51DEYGBb15BaHf6i8BPIqyU0I0PRBQuPeNyhyCmwxiz6cBgvisrx4o1yBaM2H%2FbwXjnL%2BJ4OeGlouIxzUfpoy6T%2BvcbKVouutgvj8hp8SSwehJajakPXY7MG5IUBR6YuSXfFbz5dOYiWCJGcOUKD%2BL761UseEhnZVUpZcoitl2fDuzklfaWyPUYn8rgY%2BuRTOCQOTiI%2BoD%2B%2B%2FsdLAOUSRAv2I2aPf77mZroeuJD1TmCpk5Qi32fg2vtuHpIzxGaQVJs8ADaHJH49NFtG2u4eX90nJCtK6Hpeu3i90zBZLotzy7nxjVdHLec9mYqKzIfQRmFRkqydlCx9d29Nui%2FRCKIQJRoAu4Y%2BLJ9ZOufxct48b%2FWVsA640k5PhbPVHWtWJUbflyvqTlxfa8FjbwwESSnWAKZNFydfcNHcE6ET5iDUI9x7sG%2BtXc7QVvYZ0mStZnM4LNoqnrbhiw32RQ0J94Pc5TUmaftpCFtx91FVyQREAHIvLVU6L3EPoddMCe81Y%2BoWfZ1VdpZtyH1lt4F%2FWLz73ME6x1B%2FSAH9lgopF67nI3YGvIeMm5gB11NAJsFybXc9AwuLYeH96KnwmHxJaoeP6VsUhnsLSd1X3lorNJAYu4qrwc1MKqcl6EGOrABi4eDUgPXREaKsCop%2FyecCYj5hE%2B7u1Y1v6k8bRM6REmixzo5yDG%2FLGgaO1tUCwSLMi3eysO1P3AWV8jvphmh%2BTSDZtJxqeYXGAKHCF0yauBvREP2xOAysdfTsQScIIPlo8OoLvF8p1NE04U%2BB3FeY%2BzB98mEXIQHqwtVec2DKCM3lPemcnQYoDG1X%2BtWEw174MZ3HCiVuolsn9b2ClKtnAGNAMA8Zj6e3EgorBusMjg%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230330T180000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PLSPNBABGZ%2F20230330%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=3e002c4c1a34db9a0c28ffdc651a8d907e3c0804e568323ef5cc1cdf1822b47a)

[Ejercicios](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/5d1f8301cf6a3/13899391?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1680285600000&X-Blackboard-Signature=JKsS6bRu8IxOoGjZKdffdr9dPMiC%2Ff101jX19cgd3Wg%3D&X-Blackboard-Client-Id=309366&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%27M6T01EJ.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjELb%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaDGV1LWNlbnRyYWwtMSJGMEQCIEtZTeFUOm8S%2BsKw5ON7fdsWV5rbDq1DkesUbmAUngP3AiB2%2FX8942vt7lRSO3GDEnQQIjjAV3zoaCKFLee0K4eslCrHBQiP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAMaDDYzNTU2NzkyNDE4MyIMK4mqOm8ee%2BWMgVZHKpsFQdjAfNF4X5Oue3XCCl%2Bug9sLTfaRiQc19MQNmigNXUOGqBTeKDxh6fwa7uTwJKFplEMKxA1B1UT3XNP3l0w174t5rhca5p8SInidX9I%2FRb%2Fd7U9mjCh8Cj6e29xVYpLYlgiVwc3oEyZaknF%2B6FI%2B9nzuI6TZi21ar3vi3pCLfk91Zagv0A3r0m5wku5v3EQWRzlpxOjhZINkZpiu%2BtyiylIBJTdOikoJl6%2BYENtdMb5v9DebklxIXIrnCEaey0OYwX0TBM%2BVZBbSUkc8XMKmTczvRNVXlQuTLfw%2BY%2F0ZYJvsRQT77J9nzNmkkElspmu4hMCiCPvlv7B%2FtEc%2BChpeNFJ6M%2F8b9o484VDFDiaccZaC%2BW60QB6r%2F2YXsFj0VGL6zhOkWZcWel2H5KmWBYvs6RJwwLgHfur9nz8trhqlG20yNgz8w2W01WFirFBRV6xkSWVtC24DjGs5u9vkerTqRugJJmscTytBzeXquQztTde7%2BpTO%2BpdmoGPLooZRCnc45j6lqHNQAi3pz8QncMXzYcRmpNZBqlaxivoCWSrVE4dj2VdaDFfw9%2BBCGLR2WJFK323LQadpYJVTpaEVY%2BGak4zY8c0rc0Q3AFja08JpuAT2VTYAvfneNb1IEG5GVqwoEtQCQhG6RDJhiF%2Bs%2FR3TSAvtWwnM8FWJ9jZzTZ%2FVwHey%2F6Ip2kUfAC4qPf7V8JmahVpS3au3h7YoQQmKKUR2znqMiktqZzG8Ki%2FECQAwgLorAuhAb3LB9bide0CWPmrnMtyCadx2lhTzhz6wkLfCXUutwlKHlfmjod2Z3LwRjUZYtBXPgKJqC1u7JkrHIISnIIXiHEYggBdk7tl2PbKGnieXfANtCVgHbukVAW0wTtwDFMmtnoGafCcfpTDmxpuhBjqyAdVRQLdYFt1A%2FZl3lMDG2JwZCg9ArUsRzquDOQrwSPNVY6xHJHrv0EJT6co%2FvXcuZEsmGLIyjrmRTqO6UyWob0vU%2BrOkZHWGyhI1AbG1s7AeP14xdoBGJiYqt6btAAGmimDIhBWi%2BRwKepqEMHni2av%2BmMYtCBFlUXzqvjHTE8V2f9vkIzbS7t57LF6SKzWatbUmNnqrXqW3%2FZcKGko5jEcsBNDnw%2BaBhodsxJOXzzf72D8%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230331T120000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PL476RA5X2%2F20230331%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=65fb631a6bedba7e6803ff3cf5e0d1250445d1c719024152fb8ec2fa9949356a)

[Apuntes Ciencia datos](https://alayzappala.gitlab.io/apuntes-ciencia-datos/index.html#pr%C3%B3logo)

M6T1EJERCICIOS
