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

## Recursos
[Apuntes ciencia de datos](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/5d1f8301cf6a3/13899773?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1680220800000&X-Blackboard-Signature=PD8Fk7l2pcatdQpgtva6j58IiHzGO3XirKUQHgrJny0%3D&X-Blackboard-Client-Id=309366&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%2701-Estad%25C3%25ADstica-descriptiva.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEKL%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaDGV1LWNlbnRyYWwtMSJIMEYCIQD0aky8uwWYDWgv%2Be6ggep45w9XbYotspozS%2BbxT8ULuwIhAK1e%2Fp%2FLao6EJeLfAg7jNzY1XBKKcAS5mJm4h%2BHb18FRKr4FCHsQAxoMNjM1NTY3OTI0MTgzIgzI%2F64YPBtkfh1XWyEqmwVnqNNQ4YSGtbHbA8pZNGEv9GvhjuBbIBijah2iDNcz%2Fsn8xvMy9xjIYs53hoj41LtSR7y5hyh11FKpNvqAsb0vDjzM6a0LILxe%2F%2FE3g6bm7nGvqrQp46ORkQDCWg70BCAl9gUTQ8BoC%2BqAESELjFH8cIcQtKfVxR4k%2BLVyK949fT%2B8PcmCEcycEMlUhnCR92y3xStADa2AG1V2lFA8V889Jwjw26nb7hpKOPQomK3uCaMmsjxf3tC%2F6fTsg2PtLKqJAQrAK51DEYGBb15BaHf6i8BPIqyU0I0PRBQuPeNyhyCmwxiz6cBgvisrx4o1yBaM2H%2FbwXjnL%2BJ4OeGlouIxzUfpoy6T%2BvcbKVouutgvj8hp8SSwehJajakPXY7MG5IUBR6YuSXfFbz5dOYiWCJGcOUKD%2BL761UseEhnZVUpZcoitl2fDuzklfaWyPUYn8rgY%2BuRTOCQOTiI%2BoD%2B%2B%2FsdLAOUSRAv2I2aPf77mZroeuJD1TmCpk5Qi32fg2vtuHpIzxGaQVJs8ADaHJH49NFtG2u4eX90nJCtK6Hpeu3i90zBZLotzy7nxjVdHLec9mYqKzIfQRmFRkqydlCx9d29Nui%2FRCKIQJRoAu4Y%2BLJ9ZOufxct48b%2FWVsA640k5PhbPVHWtWJUbflyvqTlxfa8FjbwwESSnWAKZNFydfcNHcE6ET5iDUI9x7sG%2BtXc7QVvYZ0mStZnM4LNoqnrbhiw32RQ0J94Pc5TUmaftpCFtx91FVyQREAHIvLVU6L3EPoddMCe81Y%2BoWfZ1VdpZtyH1lt4F%2FWLz73ME6x1B%2FSAH9lgopF67nI3YGvIeMm5gB11NAJsFybXc9AwuLYeH96KnwmHxJaoeP6VsUhnsLSd1X3lorNJAYu4qrwc1MKqcl6EGOrABi4eDUgPXREaKsCop%2FyecCYj5hE%2B7u1Y1v6k8bRM6REmixzo5yDG%2FLGgaO1tUCwSLMi3eysO1P3AWV8jvphmh%2BTSDZtJxqeYXGAKHCF0yauBvREP2xOAysdfTsQScIIPlo8OoLvF8p1NE04U%2BB3FeY%2BzB98mEXIQHqwtVec2DKCM3lPemcnQYoDG1X%2BtWEw174MZ3HCiVuolsn9b2ClKtnAGNAMA8Zj6e3EgorBusMjg%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230330T180000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PLSPNBABGZ%2F20230330%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=3e002c4c1a34db9a0c28ffdc651a8d907e3c0804e568323ef5cc1cdf1822b47a)

[Ejercicios](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/5d1f8301cf6a3/13899391?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1680285600000&X-Blackboard-Signature=JKsS6bRu8IxOoGjZKdffdr9dPMiC%2Ff101jX19cgd3Wg%3D&X-Blackboard-Client-Id=309366&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%27M6T01EJ.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjELb%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaDGV1LWNlbnRyYWwtMSJGMEQCIEtZTeFUOm8S%2BsKw5ON7fdsWV5rbDq1DkesUbmAUngP3AiB2%2FX8942vt7lRSO3GDEnQQIjjAV3zoaCKFLee0K4eslCrHBQiP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAMaDDYzNTU2NzkyNDE4MyIMK4mqOm8ee%2BWMgVZHKpsFQdjAfNF4X5Oue3XCCl%2Bug9sLTfaRiQc19MQNmigNXUOGqBTeKDxh6fwa7uTwJKFplEMKxA1B1UT3XNP3l0w174t5rhca5p8SInidX9I%2FRb%2Fd7U9mjCh8Cj6e29xVYpLYlgiVwc3oEyZaknF%2B6FI%2B9nzuI6TZi21ar3vi3pCLfk91Zagv0A3r0m5wku5v3EQWRzlpxOjhZINkZpiu%2BtyiylIBJTdOikoJl6%2BYENtdMb5v9DebklxIXIrnCEaey0OYwX0TBM%2BVZBbSUkc8XMKmTczvRNVXlQuTLfw%2BY%2F0ZYJvsRQT77J9nzNmkkElspmu4hMCiCPvlv7B%2FtEc%2BChpeNFJ6M%2F8b9o484VDFDiaccZaC%2BW60QB6r%2F2YXsFj0VGL6zhOkWZcWel2H5KmWBYvs6RJwwLgHfur9nz8trhqlG20yNgz8w2W01WFirFBRV6xkSWVtC24DjGs5u9vkerTqRugJJmscTytBzeXquQztTde7%2BpTO%2BpdmoGPLooZRCnc45j6lqHNQAi3pz8QncMXzYcRmpNZBqlaxivoCWSrVE4dj2VdaDFfw9%2BBCGLR2WJFK323LQadpYJVTpaEVY%2BGak4zY8c0rc0Q3AFja08JpuAT2VTYAvfneNb1IEG5GVqwoEtQCQhG6RDJhiF%2Bs%2FR3TSAvtWwnM8FWJ9jZzTZ%2FVwHey%2F6Ip2kUfAC4qPf7V8JmahVpS3au3h7YoQQmKKUR2znqMiktqZzG8Ki%2FECQAwgLorAuhAb3LB9bide0CWPmrnMtyCadx2lhTzhz6wkLfCXUutwlKHlfmjod2Z3LwRjUZYtBXPgKJqC1u7JkrHIISnIIXiHEYggBdk7tl2PbKGnieXfANtCVgHbukVAW0wTtwDFMmtnoGafCcfpTDmxpuhBjqyAdVRQLdYFt1A%2FZl3lMDG2JwZCg9ArUsRzquDOQrwSPNVY6xHJHrv0EJT6co%2FvXcuZEsmGLIyjrmRTqO6UyWob0vU%2BrOkZHWGyhI1AbG1s7AeP14xdoBGJiYqt6btAAGmimDIhBWi%2BRwKepqEMHni2av%2BmMYtCBFlUXzqvjHTE8V2f9vkIzbS7t57LF6SKzWatbUmNnqrXqW3%2FZcKGko5jEcsBNDnw%2BaBhodsxJOXzzf72D8%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230331T120000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PL476RA5X2%2F20230331%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=65fb631a6bedba7e6803ff3cf5e0d1250445d1c719024152fb8ec2fa9949356a) M6T1EJERCICIOS
