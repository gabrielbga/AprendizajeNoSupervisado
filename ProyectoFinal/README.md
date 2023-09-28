# Proyecto Final de Aprendizaje No Supervisado
## Implicaciones del crecimiento económico chino en Colombia: Construcción de un CLI bajo propuesta OCDE
![Colombia-China](https://tse3.mm.bing.net/th?id=OIP.C8eqQAjvo9lxY5gEnxca0wHaDM&pid=Api&P=0&h=180)

### Resumen:

Define el problema/reto al que se enfrenta el equipo, resaltando el resultado principal que se espera del trabajo sin entrar en los detalles. [15 puntos]

El problema a abordar en el proyecto se basa en la construcción de un indicador de seguimiento a la actividad económica de Colombia con el fin de complementar el trabajo iniciado por la OCDE (Organización para la Cooperación y Desarrollo Económico) en la construcción de un indicador adelantado compuesto (En adelante CLI por sus siglas en inglés) para la economía de varios de sus países miembros. Dicho indicador está diseñado con el fin de proveer señales tempranas ante puntos de inflexión en los ciclos de negocios o fluctuaciones de la actividad económica alrededor de su nivel potencial de largo plazo (OCDE, 2023).

Por otra parte, el Banco de la República desarrolló en 2011 un proyecto relacionado con la construcción de un indicador de las condiciones financieras de Colombia (Banco de la República, 2011) a partir de un análisis de componentes principales. Sin embargo, la investigación usó un rango de variables cuantitativas y cualitativas de los mercados financieros más relevantes de Colombia y no se emplearon variables sectoriales, de comercio exterior o encuestas de expectativas del consumidor. De esta manera, el trabajo se basó en la elaboración de un indicador financiero más que en un indicador adelantado de actividad económica real. Por otra parte, el ejercicio contemplaba el periodo entre julio de 1991 y junio de 2010, por lo que la mayor parte de los datos de la década de los noventa debió completarse a través de métodos para el tratamiento de valores perdidos ante la poca disponibilidad de datos. Otros trabajos relacionados, como el desarrollado por Hatzius et. al, en 2010, también contemplan exclusivamente variables financieras (NBER, 2010).

Así las cosas, se usará la metodología de componentes principales para construir un CLI para Colombia a partir de seis variables relevantes según la literatura económica: i) El área aprobada para construcción de edificaciones, ii) el número de licencias otorgadas según el área aprobada, iii) el índice de precios al consumidor (IPC), iv) las importaciones CIF en dólares, v) el índice de confianza del consumidor (ICC) y el índice de expectativas del consumidor (IEC). Una vez construido el índice a través de los principales, se realizarán ejercicios de elasticidad entre el CLI de China -construido previamente por la OCDE- y el CLI colombiano aportado en este proyecto, con el fin de cuantificar el efecto que tiene sobre la actividad económica de Colombia una rebaja de 1 punto porcentual en el crecimiento económico esperado de China para 2023.

El proyecto aporta a la literatura el primer CLI para Colombia y otorga una cuantificación al efecto que tiene el crecimiento económico de China en Colombia, dada la relación comercial entre ambos países y que incide de manera directa en las cuentas nacionales del país latinoamericano.


### Metodología y variables utilizadas:

Se usa la metodología de componentes principales para construir un CLI para Colombia a partir de treinta variables relevantes según la literatura económica: 

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

Una vez construido el índice a través de los principales, se realizan ejercicios de elasticidad entre el CLI de China -construido previamente por la OCDE- y el CLI colombiano aportado en este proyecto, con el fin de cuantificar el efecto que tiene sobre la actividad económica de Colombia una rebaja de 1 punto porcentual en el crecimiento económico esperado de China para 2023.
El proyecto aporta a la literatura el primer CLI para Colombia y otorga una cuantificación al efecto que tiene el crecimiento económico de China en Colombia, dada la relación comercial entre ambos países y que incide de manera directa en las cuentas nacionales del país latinoamericano.

### Conclusiones

Se decide usar dos componentes principales con base en las variables originales. El primer componente recoge los valores macroeconómicos provenientes de la demanda, puesto que los mayores loadings se han asignado a las variables: IPC, importaciones, ICC e IEC. Estas recogen la fortaleza relativa de la demanda interna con el fin de identificar puntos de inflexión en la actividad económica.
El segundo componente recoge los efectos macroeconómicos provenientes de la oferta, puesto que las variables Área aprobada y Número de licencias tienen los mayores loadings y están correlacionados con qué tan fuerte será el sector construcción al momento de ofrecer proyectos de vivienda. Así mismo, la variable importaciones tiene un peso importante ya que muchos de los materiales del sector edificador son importados y continúa reflejando los estímulos que tiene la oferta sobre la actividad económica.
Luego, se concluye que el primer componente principal recoge los choques de demanda y el segundo los de oferta a la hora de construir nuestro índice adelantado de actividad económica colombiana.

### Contribuyentes
* Lina Marcela Ladino Solis
* Alejandra González Pinzón
* Gabriel García Bolaños
* Diego Alejandro Gómez

### Agradecimientos
Profesor: Ignacio Sarmiento y cuerpo de monitores.

#### Propuesta Inicial: [Propuesta PDF](https://github.com/gabrielbga/AprendizajeNoSupervisado/blob/main/ProyectoFinal/Documento%20con%20propuesta%20inicial%5B1%5D.pdf)

#### Base de Datos: [Archivo de Base de datos](https://github.com/gabrielbga/AprendizajeNoSupervisado/raw/main/ProyectoFinal/BDD.xlsx)

#### NoteBook: [Notebook Proyecto](https://github.com/gabrielbga/AprendizajeNoSupervisado/blob/main/ProyectoFinal/Proyecto%20-%20Entrega%201.ipynb)
