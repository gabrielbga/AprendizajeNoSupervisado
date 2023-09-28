# Proyecto Final de Aprendizaje No Supervisado
## Implicaciones del crecimiento económico chino en Colombia: Construcción de un CLI bajo propuesta OCDE
![Colombia-China](https://tse3.mm.bing.net/th?id=OIP.C8eqQAjvo9lxY5gEnxca0wHaDM&pid=Api&P=0&h=180)

### Resumen:

Se define el problema/reto al que se enfrenta el equipo, resaltando el resultado principal que se espera del trabajo sin entrar en los detalles. [15 puntos]

El problema a abordar en el proyecto se basa en la construcción de un indicador de seguimiento a la actividad económica de Colombia con el fin de complementar el trabajo iniciado por la OCDE (Organización para la Cooperación y Desarrollo Económico) en la construcción de un indicador adelantado compuesto (En adelante CLI por sus siglas en inglés) para la economía de varios de sus países miembros. Dicho indicador está diseñado con el fin de proveer señales tempranas ante puntos de inflexión en los ciclos de negocios o fluctuaciones de la actividad económica alrededor de su nivel potencial de largo plazo (OCDE, 2023).

Por otra parte, el Banco de la República desarrolló en 2011 un proyecto relacionado con la construcción de un indicador de las condiciones financieras de Colombia (Banco de la República, 2011) a partir de un análisis de componentes principales. Sin embargo, la investigación usó un rango de variables cuantitativas y cualitativas de los mercados financieros más relevantes de Colombia y no se emplearon variables sectoriales, de comercio exterior o encuestas de expectativas del consumidor. De esta manera, el trabajo se basó en la elaboración de un indicador financiero más que en un indicador adelantado de actividad económica real. Por otra parte, el ejercicio contemplaba el periodo entre julio de 1991 y junio de 2010, por lo que la mayor parte de los datos de la década de los noventa debió completarse a través de métodos para el tratamiento de valores perdidos ante la poca disponibilidad de datos. Otros trabajos relacionados, como el desarrollado por Hatzius et. al, en 2010, también contemplan exclusivamente variables financieras (NBER, 2010).

Así las cosas, se usará la metodología de componentes principales para construir un CLI para Colombia a partir de seis variables relevantes según la literatura económica: 

i) El área aprobada para construcción de edificaciones
ii) el número de licencias otorgadas según el área aprobada
iii) el índice de precios al consumidor (IPC), 
iv) las importaciones CIF en dólares, 
v) el índice de confianza del consumidor (ICC) y el índice de expectativas del consumidor (IEC). 

Una vez construido el índice a través de los principales, se realizarán ejercicios de elasticidad entre el CLI de China -construido previamente por la OCDE- y el CLI colombiano aportado en este proyecto, con el fin de cuantificar el efecto que tiene sobre la actividad económica de Colombia una rebaja de 1 punto porcentual en el crecimiento económico esperado de China para 2023.

El proyecto aporta a la literatura el primer CLI para Colombia y otorga una cuantificación al efecto que tiene el crecimiento económico de China en Colombia, dada la relación comercial entre ambos países y que incide de manera directa en las cuentas nacionales del país latinoamericano.


### Metodología y variables utilizadas:

 La metodología de construcción del índice se basa en una preselección de variables con relevancia económica que cumple con ciertas consideraciones prácticas: misma periodicidad, no están sujetas a revisiones significantes constantemente, los datos deben ser oportunos y estar disponibles muy pronto después del período al que se refiere y es preferible que no haya valores perdidos o missing values. Para esto, utilizamos un total de 30 variables y 222 registros.

 - El área aprobada para construcción de edificaciones 
 - El número de licencias otorgadas según el área aprobada 
 - El índice de precios al consumidor (IPC)
 - Las importaciones CIF en dólares
 - El índice de confianza del consumidor (ICC)
 - El índice de expectativas del consumidor (IEC).  
 - Las Exportaciones en millones de dólares.
 - Balanza comercial de bienes en millones dólares.
 - Tipo de Brent en Dólares por barril.
 - El índice del dolar (DXY).
 - Tasa de cambio del dólar en pesos colombianos USDCOP.
 - US10Y Tesoro a 10 años en porcentaje.
 - US2Y Tesoro a 2 años en porcentaje.
 - US5Y Tesoro a 5 años en porcentaje.
 - TES 10Y Títulos de Tesorería en porcentaje.
 - CDS 5Y Credit Default Swaps a 5 indice. 
 - Banrep vs. Fed en puntos porcentuales.
 - Tasa de cambio del dólar en Euros EURUSD.
 - Tasa de cambio del dólar en Yenes USDJPY.
 - Tasa de cambio del dólar en Libras GBPUSD.
 - Tasa de cambio del dólar en Dólares Canadienses USDCAD.
 - Tasa de cambio del dólar en Coronas USDSEK.
 - Tasa de cambio del dólar en Francos USDCHF.
 - Remesas en millones de dólares.
 - Onzas de Oro por dólar.
 - Kilovatios de Gas por hora.
 - Valor de libra del café en dólares.
 - Inversión extranjera directa en millones de dólares.
 - Inversión extranjera de portafolio de dólares. 

Las fuentes de datos para la información del proyecto son: El DANE para las variables: Área aprobada, número de licencias, importaciones, tasas de cambio (euro, yen. libra, dólar, coronas, francos) e IPC. Fedesarrollo para: ICC, inversión extranjera directa y de portafolio en millones de dólares,  e IEC. De la plataforma invest(10) una plataforma pública donde se pueden extraer diversos datos económicos extrajimos Brent, Tesoros a 2, 5 y 10 años, puntos porcentuales, onzas de oro por dólar y kilovatios de gas por hora. El tipo es numérico para cada una de las variables y a continuación se presentan estadísticas descriptivas sobre los datos.
Las medidas de tendencia central muestran dispersión entre los datos debido a grandes desviaciones estándar que harán difícil la maximización de la varianza al momento de realizar análisis de componentes principales.

Tal como lo dicta la literatura económica, existen unos niveles de correlación altos entre las variables de la muestra, puesto que cada una de las variables suele servir para explicar la evolución de la actividad económica en un país como Colombia. Por ejemplo: Existen correlaciones positivas fuertes (Mayores o iguales al 80%) entre IPC- USDCOP, IPC- USDSEK, IPC - Reservas, Exportaciones - Importaciones, USDCOP - Remesas, USDCAD - DXY, USDSEK - DXY, GBPUSD - ICC. Existen correlaciones negativas fuertes (Mayores o iguales al 80%) entre  IPC - GBPUSD, USDCOP - ICC, USDCAD - ICC, USDCAD - ICE, EURUSD - DXY, ORO - USDCHF
El IPC tiene una correlación superior al 0,7 en valor absoluto con el ICC y el IEC. La correlación es negativa y ello se debe a que los tres indicadores están mostrando una tendencia en el consumidor colombiano: Una menor confianza y expectativas del consumidor afecta directamente la inflación de dicha economía ya que ante variaciones en sus expectativas de consumo implica un cambio en los precios de los bienes contemplados en el IPC. (Ver Anexo 2, gráfica de correlación)
Se observa la correlación positiva entre ICC e IEC por ser variables que tratan de explicar patrones en los hábitos de consumo del colombiano. Se observan patrones de comportamiento entre todas las variables escogidas con el IPC. La variables que presentan un menor grado de patrón de comportamiento frente al resto son Área aprobada y Número de licencias, pero entre ellas si existe un comportamiento más marcado. Así mismo, observamos que la mayoría de las variables sigue una distribución similar a la normal con leves sesgos a la derecha y a la izquierda. (Ver Anexo 3, Correlograma)


### Conclusiones

Se concluye que la estimación del indicador adelantado de la actividad económica para Colombia (CLI) denota una correlación importante y estadísticamente significativa con el CLI para China. En este orden de ideas, la metodología implementada a partir de Análisis de Componentes Principales (PCA) resulta útil para tratar de calcular un indicador que sea pertinente para inversionistas y hacedores de política económica sobre la evolución de la actividad en el sector real, puesto que la mayoría de índices desarrollados con la misma metodología pretenden calcular un índice de condiciones financieras. Con base en los hallazgos, encontramos que dicho método resulta eficiente a la hora de reducir la dimensionalidad de la matriz de variables explicativas a través de combinaciones lineales que recogen la mayor variabilidad posible de dichas variables. Por otra parte, encontramos en el criterio de Kaiser y en el análisis gráfico de varianza acumulada, dos métodos complementarios a la hora de determinar el número óptimo de componentes a utilizar. Así las cosas, con base en la construcción del índice, encontramos que un aumento de una unidad en el CLI de China, aumenta en 0.08 unidades el indicador colombiano, dando cuenta de la importancia comercial del país asiático en las cuentas nacionales de Colombia.

### Bibliografia



### Contribuyentes
* Lina Marcela Ladino Solis
* Alejandra González Pinzón
* Gabriel García Bolaños
* Diego Alejandro Gómez

### Agradecimientos
Profesor: Ignacio Sarmiento y cuerpo de monitores.

#### Propuesta Inicial: [Propuesta PDF]()

#### Base de Datos: [Archivo de Base de datos](https://github.com/gabrielbga/AprendizajeNoSupervisado/blob/main/ProyectoFinal/Entregable/BDD_.xlsx)

#### NoteBook: [Notebook Proyecto](https://github.com/gabrielbga/AprendizajeNoSupervisado/blob/main/ProyectoFinal/Entregable/Proyecto%20-%20Entrega%202%20V2.ipynb)
