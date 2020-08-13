# The-Battle-of-Neighborhoods
Project developed in the context of the course Applied Data Science Capstone

English:

RELATIONSHIP BETWEEN THE STRATUM AND THE LOCATION OF VENUES IN BOGOTÁ

My hometown, Bogotá, has a population of close to 8 million inhabitants and is geographically divided into 20 localities, each with different characteristics at the same time, each locality is geographically divided by neighborhoods for a total of 1922 neighborhoods. In addition to this geographical division, Bogotá has a division by strata, each area of the city is classified depending on the characteristics of the dwellings, the urban environment of the area and the urban context. This is how the city is subdivided into 6 socio-economic strata, 1 being the lowest and 6 the highest. This in order to identify areas of action and distribute the cost of public services; where the highest strata subsidize the lowest and these at the same time can access educational or health benefits given the stratification. This has allowed the city to quickly identify vulnerable sectors and this is how, among other things, it has managed to guarantee free of charge to strata 1 and 2 the minimum vital consumption of water (the first and only city in Colombia). Based on the significant number of architectural, cultural, and historical heritage in the city of Bogotá, the heritage layer 1 was created, which provides the aforementioned benefits to the owners of these properties.

According to The Economist, on an economic level, Bogotá stands out for its economic strength associated with the size of its production, the facilities to create companies and do business, financial maturity, the attraction of global companies and the quality of its human capital. It is the main market in Colombia and the Andean Region, and the first destination for foreign direct investment that reaches Colombia (70%). It has the highest nominal and per capita GDP in the country, contributing most of the national total (24.5%), and is the sixth city by size of GDP in Latin America (about USD 106 678 million) with a nominal GDP per capita of USD 11,594 and a GDP PPP per capita of USD 20,120, it is also the largest business platform in Colombia where most of the high impact ventures occur. The above reasons make Bogotá a business target for world-renowned brands.

Bogotá is considered a multicultural city because it has received inhabitants from all regions of the country, either because they seek better opportunities for their businesses, a greater educational offer or because of the armed conflict that has hit the rural regions of Colombian territory since the 1950s. . The people who come to Bogotá for reasons of forced displacement are people who, for the most part, do not have enough resources to survive in the city, so it is imperative to live in the lower-income neighborhoods where the payment of public services is the highest. low possible but living conditions are more difficult.

For the Bogotá mayor's office and the institutions that monitor the quality of life of its inhabitants, such as the Secretary of Housing, the Ministry of Health and the Bogotá Chamber of Commerce, among others, it is important to know the opinion of its citizens and identify if there is a trend. in the location of the places with the best quality of service and if these places have the variety of adequate services to meet the needs that increase the quality of life of citizens.

The quality of life indicators that are taken into account to give the quality of life index according to the Mercer firm (https://mobilityexchange.mercer.com/quality-of-living-reports) that placed Bogotá in position 128 Among more than 450 cities are the following: consumer goods, economic environment, accommodation, medical and health considerations, natural environment, political and social environment, public services and transportation, recreation, schools and education, sociocultural environment. Of the previous indicators, I consider that they are related to the information that can be obtained from FourSquare are the following consumer goods, economic environment, socio-cultural environment and recreation.

* COMPARE STRATIFICATION WITH POINTS WHERE INTERNATIONAL BRANDS ARE LOCATED

Due to the stratification condition it is expected and as a citizen I have been able to observe that the majority of international brands that arrive in Bogotá decide to locate their points of sale in the upper strata since the inhabitants of these neighborhoods have a much greater economic capacity than in the lower strata, so the first objective of the work will be to find if there is a relationship between brands of international stature and their location in high-strata properties in Bogotá. I hope to do this by following the following steps:

  1- Generate DF of places in Bogotá by request to FourSquare.
  
  2- In which stratum are the international places located? (The stratification JSON map of Bogotá will be used https://datosabierto.bogota.gov.co/dataset/manzana-estratificacion-bogota-d-c) A stratum column is added to the DF.
  
  3- List of international brands (scraping from https://www.value.today/world/world-top-1000-companies and / or https://www.forbes.com/global2000/#5197437e335d).
  
  4- From the list of places in Bogotá we only keep the international places.
  
  
* CLUSTERIZATION IN CONTRAST WITH STRATIFICATION

Another analysis that I would like to do is to apply the cluster method of the places in Bogotá in terms of quality, price and trend characteristics to see if there is a relationship between these characteristics and the stratum of the property where the place is located. When applying the cluster method it will be necessary to classify the clusters in various qualities of places, I would expect to obtain a cluster in which the places have high marks given by many users, many opinions and many photos taken by users this cluster would be the one of the places With better characteristics, surely you will also see a cluster in which there are low ratings given by few users and few opinions these will be considered places and given by few users, this would be the cluster with the worst characteristics for the public. Once this classification from best to worst places by cluster has been made, it will be possible to define in which stratum they are located.In this way we could see if the best places are in the neighborhoods where citizens with the highest purchasing power live (strata 5 and 6) or if they are distributed indistinctly to the stratum of the neighborhood where they are located.

  1- Add to the DF of places in Bogotá a column about your score, number of evaluations for your score, number of comments and the opinion of prices given by the public. The above information will be obtained through requests to FourSquare.
  
  2- Clustering using 6 nodes of the types of places and add their label to the DF of places
  
  3- Classify the 6 clusters according to the grouping characteristics from 1 to 6, with 6 being the best and 1 the worst
  
  4- Obtain graphs in which the results obtained and their respective analysis are evidenced.


Español:

RELACION ENTRE EL ESTRATO Y LA UBICACION DE LUGARES EN BOGOTÁ

Mi ciudad natal, Bogotá, cuenta con una población cercana a 8 millones de habitantes y está dividida geográficamente en 20 localidades cada una con características diferentes a la vez cada localidad está dividida geográficamente por barrios para un total de 1922 barrios. Además de esta división geográfica, Bogotá tiene una división por estratos, cada zona de la ciudad está clasificada dependiendo de las características de las viviendas, el entorno urbano de la zona y el contexto urbanístico. Es así como la ciudad se subdivide en 6 estratos socio-económicos, siendo el 1 el más bajo y el 6 el más alto. Esto con el fin de identificar zonas de acción y distribuir el costo de los servicios públicos; en donde los estratos más altos subvencionan a los más bajos y estos a la vez pueden acceder a beneficios educativos o de salud dada la estratificación. Esto le ha permitido a la ciudad identificar rápidamente sectores vulnerables y es así como, entre otras cosas, ha logrado garantizarle gratuitamente a los estratos 1 y 2 el consumo mínimo vital de agua (primera y única ciudad de Colombia).Es necesario añadir que con base a la importante cifra de patrimonio arquitectónico, cultural, e histórico que hay en la ciudad de Bogotá, se creó el estrato 1 patrimonial, que brinda de los beneficios mencionados anteriormente a los poseedores de esos predios.

Según The Economist, en el plano económico, Bogotá se destaca por su fortaleza económica asociada al tamaño de su producción, las facilidades para crear empresas y hacer negocios, la madurez financiera, la atracción de empresas globales y la calidad de su capital humano. Es el principal mercado de Colombia y de la Región Andina, y el primer destino de la inversión extranjera directa que llega a Colombia (70 %). Tiene el mayor PIB nominal y per cápita del país, aportando la mayor parte al total nacional (24,5 %), y es la sexta ciudad por tamaño del PIB en Latinoamérica (de unos USD 106 678 millones) con un PIB per cápita nominal de USD 11.594 y un PIB PPA per cápita de USD 20.120, igualmente es la plataforma empresarial más grande de Colombia en donde ocurren la mayoría de los emprendimientos de alto impacto. Las anteriores razones hacen que Bogotá sea objetivo empresarial de marcas reconocidas a nivel mundial.

Bogotá es considerada una ciudad multicultural debido a que ha recibido habitantes de todas las regiones del país, ya sea porque buscan mejores oportunidades para sus negocios, mayor oferta educativa o por el conflicto armado que ha golpeado desde los años 50 las regiones rurales del territorio colombiano. Las personas que llegan a Bogotá por razones de desplazamiento forzado son personas que en su mayoría no tienen los suficientes recursos para subsistir en la ciudad por lo que se hace imperante vivir en los barrios de estaros más bajos donde el pago de servicios públicos es el más bajo posible pero las condiciones de vida son más difíciles. 

Para la alcaldía de Bogotá y las instituciones que monitorean la calidad de vida de sus habitantes tal como la secretaria de habitad, ministerio de salud y cámara de comercio de Bogotá entre otros, es importante conocer la opinión de sus ciudadanos e identificar si hay una tendencia en la ubicación de los lugares con mejor calidad en servicio y si estos lugares tienen la variedad de servicios adecuados para suplir las necesidades que incrementan la calidad de vida de los ciudadanos. 

Los indicadores de calidad de vida que se tienen en cuenta para dar el índice de calidad de vida según la firma Mercer (https://mobilityexchange.mercer.com/quality-of-living-reports) que ubico a Bogotá en la posición 128 entre mas de 450 ciudades son los siguientes: bienes de consumo, ambiente económico, alojamiento, consideraciones médicas y de salud, entorno natural, entorno político y social, servicios públicos y transporte, recreación, escuelas y educación, entorno sociocultural. De los anteriores indicadores considero que se relacionan con la información que se puede obtener de FourSquare son los siguientes bienes de consumo, ambiente económico, ambiente socio cultural y recreación.


* COMPARAR ESTRATIFICACIÓN CON PUNTOS DONDE MARCAS INTERNACIONALES SE UBICAN

Debido a la condición de estratificación se espera y como ciudadano he podido observar que la mayoría de marcas internacionales que llegan a Bogotá deciden ubicar sus puntos de ventas en los estratos altos puesto que los habitantes de estos barrios tienen una capacidad económica mucho mayor que en los estratos más bajos, por lo que como primer objetivo de trabajo será encontrar si hay una relación entre marcas de talla internacional y su ubicación en los predios de estratos altos en Bogotá. Esto espero realizarlo siguiendo los siguientes pasos: 

  1- Generar DF de lugares de Bogotá mediante solicitud a FourSquare.
  
  2- ¿En qué estrato están ubicados los lugares internacionales? (Se usara el mapa JSON de estratificación de Bogotá https://datosabiertos.bogota.gov.co/dataset/manzana-estratificacion-bogota-d-c) Se agrega un columna de estrato al DF.
  
  3- Listado de marcas internacionales (scraping de https://www.value.today/world/world-top-1000-companies y/o https://www.forbes.com/global2000/#5197437e335d).
  
  4- Del listado de lugares de Bogotá solo nos quedamos con los lugares internacionales.
  
  
* Clusterizacion para contrastar con la estratificación

Otro análisis que me gustaría hacer es aplicar el método de clúster de los lugares de Bogotá en cuanto a las características de calidad, precio y tendencia para ver si hay una relación entre estas características y el estrato del predio donde está ubicado el lugar. Al aplicar el método de clúster se hará necesario clasificar los clúster en varias calidades de lugares, esperaría obtener un clúster en el que los lugares tengan calificaciones altas dadas por muchos usuarios, muchas opiniones y muchas fotos tomadas por usuarios este clúster sería el de los lugares con mejores características, seguramente también se verá un clúster en la que hay bajas calificaciones dadas por pocos usuarios y pocas opiniones estos serán considerados lugares  y dadas por pocos usuarios este sería el clúster con los lugares de peores características para el público. Una vez hecha esta clasificación de mejores a peores lugares por clúster se podrá definir en qué estrato están ubicados De esta forma podríamos ver si los mejores sitios están en los barrios donde habitan los ciudadanos con mayor capacidad adquisitiva (estratos 5 y 6)  o si están distribuidos de forma indistinta al estrato del barrio donde se ubican.

  1- Agregar al DF de lugares de Bogotá una columna sobre su puntuación, número de valoraciones para su puntuación, número de comentarios y la opinión de precios dada por el público. La anterior información se obtendrá mediante solicitudes a FourSquare.
  
  2- Hacer clustering usando 6 nodos de los tipos de lugares y agregar su etiqueta al DF de lugares
  
  3- Clasificar los 6 clúster según las características de agrupación de 1 a 6 siendo 6 los mejores y 1 los peores 
  
  4- Obtener graficas en las que se evidencien los resultados obtenidos y su respectivo análisis.
