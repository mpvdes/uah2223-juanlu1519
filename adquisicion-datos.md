# Módulo 7: Adquisición de Datos

## Sobre los datos y su extracción (Yolanda)

Gran cantidad de datos que se generan con cada movimiento que hacemos, físicos o en la red.

### Tipos de datos

- Públicos: administraciones

- Privados: empresas, rrss...

### Accesibilidad de los datos

Datos *Open Data*, fáciles de buscar y descargar. Suelen ser digitales y accesibles.

Hay otros como Twitter y Amazon que son más complicados de obtener.

### Acceso a los datos

#### Web scraping

Robot que hace peticiones a una web para extraer información específica.

No siempre es legal, te pueden bloquear la ip. Puede violar las leyes de propiedad intelectual.

Importante mirar las políticas específicas sobre el scraping. El fichero *robots.txt* de una web te indica qué está deshabilitado.

#### Uso de API's

Aplicaciones proporcionadas por algunos sitios web para acceder a sus datos. Twitter, por ejemplo, tiene la suya.

### Extración de datos a través de las APIs

API es el acrónimo de Interfaz de Programación de Aplicaciones.

Suelen estar desarrolladas en varios lenguajes de programación (Java, Python, R, C++, Ruby, etc.)

Una de las ventajas de usar APIs es que se pueden automatizar los procesos y repetir la tarea periódicamente si el contexto de la aplicación lo requiere.

### Ejemplos de APIs

- Opendatasoft

- INE

- Servicio datos abiertos del Ajuntament de Barcelona

- Idealista

- [Ayuntamiento de Madrid](https://datos.madrid.es/portal/site/egob/menuitem.214413fe61bdd68a53318ba0a8a409a0/?vgnextoid=b07e0f7c5ff9e510VgnVCM1000008a4a900aRCRD&vgnextchannel=b07e0f7c5ff9e510VgnVCM1000008a4a900aRCRD&vgnextfmt=default)

- IMDB

- Reddit

- Flickr

- Banco Mundial

- API de Spotify...

### Uso de APIs

No todas son iguales.

A veces hay requisitos de acceso, más o menos restrictivos.

### Cómo proporcionan los datos

Normalmente en formanto JSON. También pueden estar en csv y excel.

### Tipo solicitudes a API

Hay una serie de comandos, por ejemplo:

- GET: obtener datos en un formato específico

- POST: agregar datos.

- DELETE: eliminar datos.

- PUT: actualizar datos.

### Códigos de estado/respuesta de una API

Primero realizo una petición mediante una url.

La petición devuelve cierto código de respuesta.

Entre los códigos de respuesta podemos encontrarnos:

- 200: Bien.

- 204:

- 401: Falló la autenticación.

- 403:

- 404: No se encuentra el servidor/web.

- 500:

### Pasos para conectarse y llamar a las API mediante Python

1. Importar la librería para hacer peticiones http: request.

```
import requests
```

2. Realizar una acción para conectarse a la API. 

3. Imprime el código de respuesta. La variable ````status_code```` nos permite consultar el estado de conexión.


## (Martín Nadal)

### [Mapas del descontento](http://mapas.muimota.net/)

Scrapear manifestaciones y representarlas en un mapa interactivo.

TagExplorer: seleccionar las etiquetas que hay en las noticias.

### Proyecto [*In the air*](http://intheair.es/)

### [Wikidata](https://docs.google.com/presentation/d/16ix20yk9-dScyxo6sLvjeDGGpMRyvHSWfPtAcrMslvc/edit#slide=id.gcb9a0b074_1_0)

#### [SPARQL](https://query.wikidata.org)

En *Ejemplos* podemos encontrar varios ejemplos, uno muy útil es *cats*, donde nos indica cuantos gatos hay en la Wikipedia. A partir de ahí podemos modificar parámetros: país, edad de retiro...

```
#Gatos
SELECT ?item ?itemLabel ?jubilacion
WHERE 
{
  ?item wdt:P31 wd:Q146. # Debe ser un gato
  ?item wdt: P3001 ?jubilacion
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". } # Helps get the label in your language, if not, then en language
}
```

En *autolanguage* podemos cambiar el idioma de las respuestas.
En *WHERE* podemos añadir ítems a la tabla.
En *SELECT** modificamos los índices de las columnas de la tabla.
**CTRL + ESPACE**, autocompletar
wdt wikidataterm, p es propiedad
wd wikidata, q cualificador

Automáticamente se pueden generar gráficos, mapas, etc.

FILTROS: Por ejemplo, dentro de WHERE podemos filtrar por valores. FILTER(?population < 50000). También se puede ordenar con ```ORDERBY```

Luego podemos guardar esa tabla en diferentes formatos.

### ¿De qué están hechas las webs?

#### Protocolo HTTP

Requerimiento a la web.

Cookies/Session, conexión cliente/servidor.

#### HTML

Title, Body, Headers, Image...

#### DOM

### [Scrappers basados en Python](https://docs.google.com/presentation/d/1pIZGxEnERaz8HgKObu7d7bbixuQHmPPQhQybQOTQcJo/edit#slide=id.gc6f73a04f_0_0) 

#### Requests

#### BeautifulSoup

#### Selenium


