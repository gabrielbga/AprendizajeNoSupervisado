# Proyecto Final de Aprendizaje No Supervisado
## Implicaciones del crecimiento económico chino en Colombia: Construcción de un CLI bajo propuesta OCDE
![Colombia-China](https://tse3.mm.bing.net/th?id=OIP.C8eqQAjvo9lxY5gEnxca0wHaDM&pid=Api&P=0&h=180)

### Resumen:

Construcción de un indicador de seguimiento a la actividad económica de Colombia que complementa el trabajo iniciado por la OCDE (Organización para la Cooperación y Desarrollo Económico) en la creación de un indicador adelantado compuesto (En adelante CLI por sus siglas en inglés) para la economía de varios de sus países miembros. Dicho indicador está diseñado con el fin de proveer señales tempranas ante puntos de inflexión en los ciclos de negocios o fluctuaciones de la actividad económica alrededor de su nivel potencial de largo plazo (OCDE, 2023).

### Metodología y variables utilizadas:

Se usa la metodología de componentes principales para construir un CLI para Colombia a partir de seis variables relevantes según la literatura económica: 

* El área aprobada para construcción de edificaciones 
* El número de licencias otorgadas según el área aprobada
* El índice de precios al consumidor (IPC)
* Las importaciones CIF en dólares
* El índice de confianza del consumidor (ICC) 
* El índice de expectativas del consumidor (IEC). 

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


### Base de Datos: [Archivo de Base de datos](https://github.com/gabrielbga/AprendizajeNoSupervisado/raw/main/ProyectoFinal/BDD.xlsx)
