##### TAREA 01 - CREACIÓN DE MAPAS TEMÁTICOS CON QGIS Y PUBLICACIÓN DE RESULTADOS EN QGIS CLOUD

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

1.	Descarga del programa QGIS versión 3.4.13.
2.	Configuración del idioma para instalación de plugins.
3.	Creación de la cuenta en Qgis Cloud, usuario: jsortegac.
4.	Instalación del plugin QGisCloud.

PANTALLAZO 1
![img1](imagen/PANTALLAZO1.JPG)

5.	Descarga de información del portal de datos abiertos de Bogotá en formato shp: valor de referencia metro cuadrado de Bogotá y unidad de planeamiento zonal

![img1](imagen/PANTALLAZO2.JPG)
![img1](imagen/PANTALLAZO3.JPG)

6.	Se cargan los datos descargados SHP en QGIS

![img1](imagen/PANTALLAZO4.JPG)

7.	En la herramienta de propiedades de la respectiva capa, pestaña simbología, se selecciona el método de clasificación y la configuración respectiva en cuanto a los parámetros, como se muestra a continuación: 

MÉTODO DE CLASIFICACIÓN CATEGORIZADO
![img1](imagen/PANTALLAZO5.JPG)

MÉTODO DE CLASIFICACIÓN GRADUADO 
![img1](imagen/PANTALLAZO11.JPG)

8. Se obtienen las siguientes clasificaciones:

**Resultado Mapa Categorizado**

![img1](imagen/PANTALLAZO6.JPG)

**Resultado Mapa Graduado**
![img1](imagen/PANTALLAZO12.JPG)


# Publicación de los Mapas en el servidor mediante QGisCloud

8. Inicialmente, se ingresa el usuario y contraseña de la cuenta creada en el QGis Cloud en la ventana Cloud Settings

![img1](imagen/PANTALLAZO7.JPG)


9. Posteriormente, en la pestaña Upload Data se agregan las capas que van a subirse en el servidor

![img1](imagen/PANTALLAZO8.JPG)


10. Ahora bien, se guarda el proyecto en formato .qgz
![img1](imagen/PANTALLAZO9.JPG)


11. Finalmente, se selecciona la opción de publicar mapa
![img1](imagen/PANTALLAZO10.JPG)

12. Finalmente se visualizan los mapas creados:
![img1](imagen/PANTALLAZO13.JPG)
![img1](imagen/PANTALLAZO14.JPG)


Éste proceso se repite para la publicación del otro mapa.

*Ventajas/desventajas/dificultades/diferencias*

-QGIS es un software libre que permite ejecutar diversas funciones de análisis espacial y de publicación de mapas en la web.

-Se generaron diversos problemas en la ejecución de los procesos, razón por la cual fue necesario repetir diferentes procesos.

*URL de mapas en la web*

# Mapa 1, Método de clasificación Categorizado
https://qgiscloud.com/jsortegac/Tarea_1_Galerias/?bl=&st=&l=OpenStreetMap%2CGalerias_proj%2CGalerias_valor&t=Tarea_1_Galerias&e=998795%2C1004298%2C1002409%2C1006031

WMS: 
https://wms.qgiscloud.com/jsortegac/Tarea_1_Galerias/

# Mapa 1, Método de clasificación Graduado
https://qgiscloud.com/jsortegac/Tarea_b_Galerias/?bl=&st=&l=OpenStreetMap%2CGalerias_proj%2CGalerias_valor&t=Tarea_b_Galerias&e=999055%2C1004335%2C1002669%2C1006068

WMS: 
https://wms.qgiscloud.com/jsortegac/Tarea_b_Galerias/

