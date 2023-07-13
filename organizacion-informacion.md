# Módulo 10 - Organización de la información

[Apuntes módulo 10](https://docs.google.com/presentation/d/1Z-CMnCVXWctdpzXSTtzpXVTQicJ0ey7Y9BfhNMeX8Uk/edit#slide=id.p)

[Más Apuntes Módulo 10](https://docs.google.com/presentation/d/1alE7mRgCqqbYePIDtQxxAEgaGpyCFMTDUWfWLqAENIg/edit?usp=sharing)

## Ficheros de datos

### JSON

*JavaScript Object Notation*. Formato de texto sencillo para el intercambio de datos. Como los diccionarios de Python.

### CSV

*Comma Separated Values***. Formato abierto sencillo para representar datos en forma de tabla. La primera fila normalmente es la cabecera de la tabla.

### YAML

## Bases de datos relacionales

Base de datos relacional (BDR) es un tipo de base de datos (BD) que cumple con el modelo relacional. La información está organizada en una o más de una tabla. Cada tabla tiene columnas y filas/tuplas. Un identificador identifica cada fila.

![Base de datos relacionales](https://www.aluracursos.com/blog/assets/base-de-datos-relacional/img3.png**

### ¿Qué es una base de datos?

Cualquier colección de información relacionada. Se puede guardar en papel o en un ordenador.

### Escala

- Hay que tener un seguimiento de cada uno de los productos que se venden.

- Tener en cuenta la seguridad.

- Los accesos

- Qué permisos tiene cada usuario

- ...

### BBDD

La bases de datos reside en un gestor de bases de datos.

### C.R.U.D.

**Create Read Update Delete**

## SQL

*Structured Query Language*. Lenguaje que nos permite hacer consultas a esa base de datos formada por un conjunto de tablas relacionadas.

**SELECT**, **FROM** y **WHERE** son los comandos principales.

Gestor de Base de datos:

- Ayuda a los usuarios a crear y mantener la base de datos relacional. Ej: *mysql*, *sqlite*, *postgreSQL*.

### Palabras importantes

- Create: crear.

- Drop: eliminar.

- Alter : alterar.

### Tipos de datos

Cada columna tiene un tipo de datos y solo vamos a poder guardar datos de ese tipo en esa columna.

- INT

- DECIMAL

- VARCHAR: cadena de carácteres de longitud N.

- DATE: en formato YYYY-MM-DD.

- TIMESTAMP: YYYY-MM--DD HH:MM:SS

- BLOB: no se usa mucho pero es , un *binary large object*.

- TEXT: de longitud N, un máximo de 64k.

- MEDIUMTEXT: máximo 16mb.

- LONGTEXT: máximo de 4gb.

## NoSQL

Cualquier base de datos que no sea relacional. Las más conocidas son **mongoDB**, **apache cassandra** y **GraphQL**. CSV, JSON...

## BDOG

Una base de datos orientada a grafos (BDOG) representa la información como nodos de un grafo y sus relaciones con las aristas del mismo, de manera que se pueda usar teoría de grafos para recorrer la base de datos ya que esta puede describir atributos de los nodos (entidades) y las aristas (relaciones).

## SPARQL y RDF

## Wikidata

## Tablas y claves

![Tablas y claves](https://jesuscasillas.files.wordpress.com/2013/09/keyprimary.gif)

Todas deben tener una clave principal o clave ajena para identificar al usuario inequívocamente (DNI, correo electrónico, nombre de usuario...).

### Relación n a n

La relación entre tabla no tiene por qué ser siempre 1 a 1. Ej: un alumno pertenece a muchas clases y una clase pertenece a muchos alumnos.

## XAMPP

### Primeros pasos

- Lanzar el programa

- Elegir programas a utilizar

- Escribir "localhost" en mi navegador.

### phpMyAdmin

- En **Databases** podemos crear nuevas bases de datos. La veremos en el margen izquierdo del programa.

#### Crear una tabla sencilla

CREATE TABLE agenda(
id INT, 
nombre VARCHAR(20), 
apellidos VARCHAR(50), 
nacimiento DATE );

#### Elegir la tabla como primaria

ALTER TABLE agenda ADD PRIMARY KEY (id);

#### Eliminar tabla

DROP TABLE agenda

#### Añadir datos a nuestra tabla

INSERT INTO agenda VALUES (1,'Paul','McCartney','1942-06-18')

INSERT INTO agenda VALUES (2,'Ringo','Starrr','1940-07-01');

#### Autoincremento

Nosotros ya hemos puesto el autoincremento al crear la tabla:

CREATE TABLE agenda(
	id INT PRIMARY key AUTO_INCREMENT,
	nombre VARCHAR(20),
	apellidos VARCHAR(50),
	nacimiento DATE
)

Al escribir:

INSERT INTO agenda (nombre,apellidos) VALUES ('Mick','Jagger');

Metemos esos datos y rellena el ID pero el nacimiento es NULL,

#### Select

La instrucción que vamos a usar más:

SELECT nacimiento FROM musicos

##### Filtrar con Select

Ejemplo: que me devuelva todos los músicos nacidos antes de 1950.

SELECT nombre FROM musicos WHERE nacimiento < '1950-01-01'
SELECT * FROM musicos WHERE year(nacimiento) < 1951

Ejemplo: me devuelve el nombre, apellido y año de nacimiento de la tabla *músicos*.

SELECT nombre,apellidos, YEAR(nacimiento) FROM 'musicos';

##### Filtrar con Order

SELECT * FROM employee ORDER by super_id, salary (filtrar empleados por id de su superior y salario)

SELECT * FROM employee ORDER by salary DESC (orden descendente)

SELECT * FROM employee ORDER by salary LIMIT 3 (solo quiero que me devuelva 3)

##### Renombrar con As

SELECT first_name AS nombre FROM employee

##### Filtrar con Distinct

SELECT DISTINCT(super_id) FROM employee (todos los que son jefes de alguien, o sea managers)

##### Filtrar con Count

SELECT COUNT(*) AS num_empleados FROM employee (me dice el número de empleados)

##### Filtrar con Year

SELECT first_name, last_name, YEAR(birth_day) FROM employee

SELECT first_name AS nombre, last_name AS apellido, YEAR(birth_day) AS anyo FROM employee WHERE YEAR(birth_day) > 1965

##### Filtrar con Between

SELECT first_name as nombre, last_name as apellido, year(birth_day) FROM employee WHERE year(birth_day) BETWEEN 1965 AND 1970

SELECT first_name as nombre, last_name as apellido, year(birth_day) FROM employee WHERE year(birth_day) > 1965 and year(birth_day) < 1970

##### Filtrar con ISNULL

SELECT * FROM `employee` WHERE super_id IS NULL (Empleados que no tienen jefe)

SELECT * FROM `employee` WHERE super_id IS NOT NULL (Empleados que sí tienen jefe)

##### Filrar con LIKE

SELECT * FROM employee WHERE first_name LIKE "J%" (no me importa lo que vaya detrás del porcentaje)

SELECT * FROM employee WHERE first_name LIKE "%M" (todos los nombres que acaben en "m")

SELECT * FROM employee WHERE first_name LIKE "%a%" (todos los nombres que contengan "a")

SELECT * FROM employee WHERE first_name LIKE "_a%_" (cuya segunda letra sea una "a")

##### Filtrar con AVG (para medias)

SELECT AVG(salary) FROM employee

##### Filtrar con SUM (para sumatorios)

SELECT SUM(salary) FROM employee

##### Filtrar con GROUP BY (para agrupar)

SELECT sex, AVG(salary) AS "sueldo_medio" FROM employee GROUP by sex

##### Filtrar con UNION

SELECT branch_name FROM branch

UNION

SELECT first_name FROM employee

(Nos ha unido las dos consultas. Tienen que tener el mismo nombre de columnas)

##### Filtrar con JOIN

###### Inner join : combinar filas de dos o más tablas basándose en columnas comunes

SELECT * FROM employee JOIN branch ON employee.branch_id = branch.branch_id

SELECT emp_id, first_name, last_name, branch_name FROM employee JOIN branch ON employee.branch_id = branch.branch_id

SELECT employee.emp_id, first_name, last_name, SUM(total_sales) FROM employee JOIN works_with ON employee.emp_id = works_with.emp_id GROUP by employee.emp_id

#### Consultas anidadas

##### Primera consulta

SELECT DISTINCT(emp_id) from works_with WHERE total_sales>30000; (Me devuelve 101, 105)

##### Segunda consulta (anidada)

SELECT * from employee where emp_id IN ( SELECT DISTINCT(emp_id) from works_with WHERE total_sales>30000 ); 



#### Exportar tabla

Podemos cambiar el nombre de las columnas antes de exportar:


## Wikidata (SPRQL)

```
#Intel

SELECT ?item ?itemLabel ?image ?next

WHERE 

{

 ?item wdt:P279 wd:Q12047070. # Must be of a cat

 ?item wdt:P18 ?image.

 OPTIONAL{

  ?item wdt:P156 ?next.

 }

 SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". } # Helps get the label in your language, if not, then en language

}
```
