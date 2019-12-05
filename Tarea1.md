**TAREA 01 - CREACIÓN DE MAPAS TEMÁTICOS CON QGIS Y PUBLICACIÓN DE RESULTADOS EN QGIS CLOUD**

## MAPA DE VALOR METRO CUADRADO DE TERRENO EN LA LOCALIDAD DE TEUSAQUILLO - BOGOTÁ D.C

*Cuál es el problema a tratar?*

Conocer el valor metro cuadrado de terreno de las diferentes manzanas catastrales ubicadas en la UPZ – Galerías de la localidad de Teusaquillo en la ciudad de Bogotá, teniendo como referencia los datos suministrados por la Unidad Administrativa Especial de Catastro Distrital – UAECD. 

*Por qué un mapa ayuda a resolverlo?*

Porque el mapa da la posibilidad de visualizar todas las manzanas catastrales que abarcan la Unidad de Planeamiento Zonal de Galerías con su respectivo valor metro cuadrado de terreno,  

*Descripción del mapa temático*

El mapa de valor metro cuadrado de terreno permite visualizar la superposición de las manzanas catastrales ubicadas en la Unidad de Planeamiento Zonal con su respectivo valor metro cuadrado de terreno  (el cual puede tener fines comerciales y catastrales), mediante polígonos representados por un color el cual permite evidenciar las diferencias de valor en la zona de estudio.

*Descripción de los métodos de clasificación seleccionados*

Los métodos de clasificación seleccionados fueron los siguientes:

**Categorizado**
El método categorizado genera una representación diferente por cada registro en el atributo de V_REF, el cual hace referencia al valor metro cuadrado de terreno. Con éste método, si existen dos registros con el mismo valor, serán representados por el mismo color.

**Graduado**
El método graduado genera intervalos de valor a partir del atributo seleccionado (el cual debe ser de tipo cuantitativo). Permite seleccionar el modo para establecer los intervalos con los cuales se van a representar el valor metro cuadrado de terreno, éste puede ser intervalo igual, cuantil, rupturas naturales, desviación estándar y/o pretty breaks. Igualmente, tiene como parámetro el número de clases, es decir, el número de intervalos para la representación de la variable. Con éste método, se representa con un color diferente cada intervalo. 

*-Cuál es mejor para la variable seleccionada? Por qué?*

Para la variable seleccionada, la cual es de tipo cuantitativo, el mejor método de clasificación es el graduado, puesto que, teniendo en cuenta la cantidad de datos, si se representa de forma categorizada no va a ser clara la representación al no disponer de una amplia gama de colores para representar cada valor. No obstante, si se generan rangos de valor, es posible comprender y tener mayor claridad de los valores en la zona de estudio. 

*Listado de fuentes de datos seleccionados*

Los datos fueron adquiridos del portal de datos abierto de Bogotá, los cuales se pueden encontrar en las siguientes URL:

Valores metro cuadrado de terreno:
https://datosabiertos.bogota.gov.co/dataset/valor-de-referencia-por-metro-cuadrado-de-terreno

UPZ:
https://datosabiertos.bogota.gov.co/dataset/unidad-de-planeamiento-bogota-d-c

*Descripción del procedimiento utilizado*

1.	Descarga del programa QGIS versión 3.4.13
2.	Configuración del idioma para instalación de plugins
3.	Creación de la cuenta en Qgis Cloud, usuario: jsortegac
4.	Instalación del plugin QGisCloud.

![img1](PANTALLAZOS/PANTALLAZO1.JPEG)

5.	Descarga de información del portal de datos abiertos de Bogotá en formato shp: valor de referencia metro cuadrado de Bogotá y unidad de planeamiento zonal

PANTALLAZO 2 Y 3

6.	Se cargan los datos descargados SHP en QGIS

PANTALLAZO 4

7.	En la herramienta de propiedades de la respectiva capa, pestaña simbología, se selecciona el método de clasificación y la configuración respectiva en cuanto a los parámetros: 

MÉTODO DE CLASIFICACIÓN CATEGORIZADO
PANTALLAZO 5

MÉTODO DE CLASIFICACIÓN GRADUADO 
PANTALLAZO 11

8.	 Se obtienen las siguientes clasificaciones:

### Resultado Mapa 1

PANTALLAZO 6

### Resultado Mapa 2
PANTALLAZO 12



*Ventajas/desventajas/dificultades/diferencias*
*Proyecto QGIS*
*URL de mapas en la web*
