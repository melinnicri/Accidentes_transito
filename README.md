# Proyecto Individual: 

# Accidentes de Tránsito de la Ciudad Autónoma de Buenos Aires, Argentina, 2016-2021. 
## Amelia Herrera Briceño 
## melinnicri@gmail.com 
## Enero, 2024
 


Trabajo rol de Data analyst acerca de los accidentes de tránsito ocurridos entre los años 2016- 2021, de la Ciudad Autónoma de Buenos Aires, Argentina. 

Los accidentes de tránsito son una de las principales causas de muerte y lesiones en la ciudad. Según el gobierno porteño, los factores que contribuyen a los accidentes son el incumplimiento de la ley de tránsito, el exceso de velocidad, el no respetar las señales de tránsito, el no usar cinturón de seguridad o apoya cabezas y el conducir con cansancio. Además, los medios de transporte más involucrados en los accidentes son las motos, seguidas por los autos y los colectivos. Los accidentes de tránsito generan un alto costo social y económico, así como un impacto negativo en la calidad de vida de las personas.

Se entregan bases de datos con información acerca de los homicidios y víctimas (data desde páginas oficiales argentinas). 
Se realiza un ETL y EDA, respectivamente, utilizando Studio Visual Code notebook, librerías Panda, Numpy, Matplotlib, y su presentación final en PowerBI.

KPIs solicitadas: 

1) Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior (semestre año 2021-2020). 

Definimos a la tasa de homicidios en siniestros viales como el número de víctimas fatales en accidentes de tránsito por cada 100.000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100.000. 

2) Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior (año 2021-2020). 

Definimos a la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100.
 
3) Con datos de cantidad de víctimas por comuna, se toman las comunas con más accidentados para calcular la tasa de mortalidad por siniestros viales. Para ello, debes dividir el número de víctimas fatales por el número de habitantes de cada comuna y multiplicar por 100.000. Así se obtiene la tasa de mortalidad por cada 100.000 habitantes, que es un indicador estandarizado que permite comparar entre comunas. En esta tercera KPI, se pide reducir en 20% la tasa en la Comuna 1.

Aquí se escoge la Comuna 1, por el Top 5 de Accidentes de tránsito fatales, con una población promedio (extraído desde Censo de los años disponibles, 2010 y 2022).

*Las 15 comunas de Ciudad Autónoma de Buenos Aires: 
COMUNA 1: Retiro, San Nicolás, Puerto Madero, San Telmo, Montserrat y Constitución. 
COMUNA 2: Recoleta. 
COMUNA 3: Balvanera y San Cristóbal. 
COMUNA 4: La Boca, Barracas, Parque Patricios y Nueva Pompeya. 
COMUNA 5: Almagro y Boedo. 
COMUNA 6: Caballito. 
COMUNA 7: Flores y Parque Chacabuco. 
COMUNA 8: Villa Soldati, Villa Riachuelo y Villa Lugano. 
COMUNA 9: Liniers, Mataderos y Parque Avellaneda. 
COMUNA 10: Villa Real, Monte Castro, Versalles, Floresta, Vélez Sarsfield y Villa Luro. 
COMUNA 11: Villa General Mitre, Villa Devoto, Villa del Parque y Villa Santa Rita. 
COMUNA 12: Coghlan, Saavedra, Villa Urquiza y Villa Pueyrredón. 
COMUNA 13: Núñez, Belgrano y Colegiales. 
COMUNA 14: Palermo. 
COMUNA 15: Chacarita, Villa Crespo, La Paternal, Villa Ortúzar, Agronomía y Parque Chas.


Archivos: 
"New_Acd_transito/Accidentes.ipynb" 

Conclusiones: 
De acuerdo con los resultados obtenidos en PowerBI, podemos concluir que: 

-	Entre los años 2016 y 2021, en CABA, los accidentes de tránsito tendieron a disminuir, en parte por la pandemia (restricción movilización) y nuevamente aumentaron saliendo de este encierro.

-	Es llamativo que en las mañanas hubieran más accidentes (7 horas), se suponen “descansados”.

-	La tasa de mortalidad promedio por cada 100.000 habitantes entre los años 2016 y 2021 es de 3,5 (717 víctimas fallecidas en total).

-	El tipo de accidente de tránsito más frecuente es atropellamiento de peatones por colectivos y choque de motos con autos, donde también la cantidad de fallecidos es alta. 

-	Las edades de las víctimas fallecidas con mayor frecuencia son del rango 20-29 años y en su mayoría del sexo masculino. 

-	El top 5 (por sobre 60 víctimas fatales) por comunas de CABA, se encuentran Comuna 1 (Retiro, San Nicolás, Puerto Madero, San Telmo, Montserrat y Constitución); Comuna 4 (La Boca, Barracas, Parque Patricios y Nueva Pompeya); Comuna 7 (Flores y Parque Chacabuco), Comuna 8 (Villa Soldati, Villa Riachuelo y Villa Lugano), Comuna 9 (Liniers, Mataderos y Parque Avellaneda) como total por rango años 2016-2021. 




Los índices KPIs:
 
1)	En los primeros seis meses (Enero-Junio del 2020), hay cierta Tasa de mortalidad por accidentes de tránsito por cada 100000 habitantes. En el tramo semestral (Julio-Diciembre, 2020) hubo una reducción de esta tasa del 58% con respecto del semestre anterior. Por tanto, se cumple con la reducción de más del 10%, como también en el segundo semestre 2021, 14%, con respecto del semestre anterior.

2)	En cuanto a Tasa de mortalidad por moto, hubo una disminución del 64,3% de un año a otro (2020-2021), por lo que se logra reducir en más del 7%.

3)	En cuanto a la Tasa de mortalidad por accidentes de tránsito por cada 100000 habitantes de la Comuna 1, ya que era la comuna con más fallecidos por accidentes de tránsito, seguido de la Comuna 4, Comuna 7, Comuna 8, Comuna 9, entre los años 2016 y 2021, hay una reducción de más del 20% en el 2018 y 2020.

Mientras más tránsito vehicular, más accidentes, por lo que tomar las medidas de precaución, como respetar las señales de tránsito, transitar a una velocidad prudente, mantener el cinturón de seguridad como el uso de cascos y ropa apropiada para motos (cuero antidesforramiento), cruzar en zona habilitada, descansar lo necesario para conducir vehículos, no beber alcohol, ni consumir drogas psicotrópicas que afecten la conducción, 


Mientras más tránsito vehicular, más accidentes. Por lo tanto, es importante tomar medidas de precaución para evitar accidentes. Algunas de las medidas que se pueden tomar son:
•	Respetar las señales de tránsito: Las señales de tránsito están diseñadas para mantener el orden en las carreteras y garantizar la seguridad de los conductores y peatones. Es importante respetar estas señales para evitar accidentes.
•	Mantener el vehículo en buen estado: es importante realizar un mantenimiento preventivo cada cierto tiempo.
•	Transitar a una velocidad prudente: Conducir a una velocidad adecuada es fundamental para evitar accidentes. La velocidad debe ser ajustada a las condiciones del tráfico y del clima.
•	Mantener el cinturón de seguridad como el uso de cascos y ropa apropiada para motos (cuero antidesforramiento): El uso del cinturón de seguridad y de cascos es obligatorio en muchos países. Estos elementos de seguridad pueden salvar vidas en caso de accidentes. Además, es importante usar ropa adecuada para motos, como cuero antidesforramiento, para protegerse en caso de caídas.
•	Cruzar en zona habilitada: Los peatones deben cruzar la calle en las zonas habilitadas para ello. Cruzar la calle en lugares no autorizados puede ser peligroso y aumentar el riesgo de accidentes.
•	Descansar lo necesario para conducir vehículos: Conducir cansado o con sueño puede ser peligroso. Es importante descansar lo suficiente antes de conducir para evitar accidentes.
•	No beber alcohol, ni consumir drogas psicotrópicas que afecten la conducción: El alcohol y las drogas psicotrópicas pueden afectar la capacidad de conducción y aumentar el riesgo de accidentes. Es importante evitar su consumo antes de conducir.
FIN…_@v
