# Variación en los sólidos, sedimentos y cobertura vegetal en el Humedal Nacional Térraba-Sierpe, Osa, Puntarenas, Costa Rica en la estación seca - lluviosa,  2018 - 2019  

### Esta página corresponde a una recopilación del trabajo final realizado en el curso de Fotogrametría y Teledetección, ciclo II, año 2021.  
#### Autores del trabajo: 
- Allan Chinchilla;
- David Youna;
- Jose Umaña.

## Resumen

En dicho trabajo consiste en un estudio de teledetección en el Humedal Nacional Térraba-Sierpe, el cual se encuentra localizado en el cantón Osa, Puntarenas. Es uno de los manglares más extensos de Centroamérica con más de 14 000 Ha, se encuentra en condiciones climáticas tropicales, debido a esto, presenta condiciones húmedas durante todo el año. Esto incrementa el desarrollo de una cobertura tropical y la respectiva dinámica de dispersión de sedimentos. Para este estudio realizaron una comparación por medio de imágenes satelitales de Landsat 8 y Sentinel 2 entre los años 2018-2019, para así determinar patrones con respecto a la variación de la cobertura vegetal, sólidos y sedimentos disueltos en el manglar. Los resultados obtenidos en el estudio arrojaron variaciones en la época seca y lluviosa en cuanto a los sólidos y sedimentos disueltos en el agua, asi mismo, la cobertura vegetal muestra diferencias mínimas entre los periodos de estudio. 

<img src="Térraba-Sierpe1.jpg" Height="400" width="600">

*Fig 1*. Humedal Nacional Térraba-Sierpe. Tomada de: [QCOSTARICA](https://qcostarica.com/humedal-nacional-terraba-sierpe/)


## Metodología

1.**Colección de imágenes y bandas**

Los procesos de recopilación de información se realizaron por medio de Google Earth Engine. Para el calculo de índice de sedimentos disueltos, utilizaron tres bandas (B2, B4 y B8) de la colección sentinel S2 (Sentinel-2 MSI: MultiSprectral Instrument, Level-1C), estas bandas se multiplican por 3, por 5 y por 2, respectivamente, para así realizar una sumatoria final, generando una nueva colección, con los valores ajustados. 
Para el NDVI utilizaron las bandas B5 y B4, mediante el método de NormalizedDifference, utilizando la colección LandSat 8 (USGS Landsat 8 Collection 1 Tier 1 and Real-Time Data TOA Reflectance)

2.**Procesamiento de los datos**

Para la colección del índice de sedimentos, se filtraron las imágenes por fechas, también utilizaron la propiedad llamada *“Cloudy_Pixel_Percentage”* con *“Less_Than”* con un valor de 20, así seleccionan las imágenes con menos nubosidad.  Para un análisis cuantitativo utilizaron de apoyo una imagen RGB con máscara de nube. Además, seleccionan dos sectores para así comparar las imágenes en ambas estaciones (época seca/lluviosa), las variables comparadas fueron el valor de longitud de onda contra la reflectancia total. Valores tomados desde los metadatos de la colección Sentinel S2.  
Para el NDVI, con las bandas seleccionadas, por medio del NormalizedDifference, con una paleta de colores especificas mostraron de una mejor manera el índice. 

# Resultados

## Sedimentos disueltos y sólidos en el Humedal Nacional Térraba – Sierpe.  
Identificaron zonas con aumento o disminución de arrastre de sedimentos, así mismos sedimentos disueltos en el agua, el mayor arrastre de sedimentos se presenta sobre la desembocadura del Río Térraba, de igual forma para el estero presente en el humedal.
Igualmente, detectaron sólidos, los cuales se clasificaron o se determinaron como sólidos en las líneas de costa establecidas, por lo cual los resultados variaron debido al aumento o disminución de las mareas.  En las reflectancias, las tendencias entre estaciones fueron similares.  Los sedimentos presentan una mayor reflectancia en los valores del infrarrojo cercano, pero al encontrarse por debajo o disueltos en el agua, los valores pueden variar.  

<img src="Colección2.png" Height="200" width="300">

*Fig 2*. Sedimentos disueltos y sólidos en el Humedal Nacional Térraba-Sierpe. Tomada de Chinchilla, Young y Umaña, 2021.

## NDVI  
No identificaron cambios anormales en la cobertura vegetal en las dos estaciones, los valores de los pixeles del índice se mantuvieron constantes. Para el año 2018, los valores son ligeramente mayores, a diferencia del periodo 2019. Pudieron identificar una ligera disminución en el volumen de agua en Humedal. 

<img src="NDVI_HNTS.png" Height="200" width="300">

*Fig 3*. NDVI del Humedal Nacional Térraba-Sierpe. Tomada de Chinchilla, Young y Umaña, 2021.

### Referencias:

[1.](https://www.researchgate.net/publication/324756318_Cobertura_y_Distribucion_de_las_Especies_de_Mangle_en_el_Humedal_Nacional_Terraba-Sierpe_Costa_Rica) Acuña, J., Quesada, A y Vargas, C. (2018). Cobertura y Distribución de las Especies de Mangle en el Humedal Nacional Térraba-Sierpe, Costa Rica. Anuario do Instituto de Geociencias. 

[2.](https://areasyparques.com/areasprotegidas/humedal-nacional-terraba-sierpe/) Áreas Protegidas y Parques Nacionales de Costa Rica. (2013). Humedal Nacional Térraba-Sierpe. 

[3.](https://www.kerwa.ucr.ac.cr/bitstream/handle/10669/11077/Humedal_terrabasierpe.pdf?sequence=1) Arroyo, D. (2013). Humedal Nacional Térraba-Sierpe Nuevos pasos en nuestra acción social e  investigación. Escuela de Biología, Universidad de Costa Rica.   

[4.](http://www.gisandbeers.com/busqueda-sedimentos-solidos-disueltos-gee) GIS&Beers. (2019). Búsqueda de sedimentos y sólidos disueltos en GEE. 

[5.](https://repository.usc.edu.co/bitstream/handle/20.500.12421/4453/IMPORTANCIA%20DE%20LOS%20HUMEDALES%20.pdf?sequence=3&isAllowed=y) Ibarguen, V y Bernal, D. (2019). Importancia de los humedales naturales y artificiales en el ámbito socio-ambiental. Una revisión bibliográfica. Universidad Santiago de Cali, Colombia.

[6.](https://repositorio.catie.ac.cr/bitstream/handle/11554/1576/El_manglar_de_Terraba_Sierpe.pdf?sequence=1&isAllowed=y) Mainardi, V. (1996). El manglar de Térraba-Sierpe en Costa Rica. Centro Agronómico Tropical de Investigación y Enseñanza, Turrialba, Costa Rica.

[7.](https://www.ramsar.org/sites/default/files/documents/pdf/lib/lib_manual2006s.pdf) Secretaría de la Convención de Ramsar. (2006). Manual de la Convención de Ramsar: Guía a la Convención sobre los Humedales (Ramsar, Irán, 1971), 4a. edición. Secretaría de la Convención de  Ramsar, Gland (Suiza).
