# Acabo de terminar un proyecto que me ha ayudado a aprender mucho sobre el análisis de regresión y preprocesamiento de datos 📊 👏 

Este proyecto trata sobre la estimación de los precios de apartamentos en varias zonas de la ciudad de Valencia, Venezuela. El dataset utilizado fue de la colección de datos de una Inmobiliaria en la misma ciudad. Por lo tanto no podré mostrar ciertos datos sensibles. Sin embargo, si puedo enseñar los resultados y los pasos que utilice para crear este proyecto.

En lo personal siempre me gusta colocar un "Problema" o caso como ejercicio. Para esta ocasión, el problema es el siguiente:

    "Eres un Científico de Datos, el cual fue contratado por la inmobiliaria para     un proyecto. El foco principal de este proyecto consiste en la colocacion de precios en las viviendas

    de clientes nuevos que buscan vender sus propiedades de la mano de la Inmobiliaria. Te vas a basar en un conjunto de datos que te fue proporcionado en donde te indica informacion como

    la zona de la ciudad, el numero de habitaciones y de baños, el numero de puestos de estacionamiento entre otros datos. En este caso la propiedad a vender es un apartamento



    De la misma manera, a partir de estos datos, los ejecutivos de la Inmobiliaria desean tener un analisis descriptivo de la situacion e inventario de las propiedades con las que cuentan para la venta, en un dashboar informativo que cubra las siguientes preguntas:

        * El precio maximo, minimo y promedio de las viviendas manejadas

        * La distribucion, o cantidad, de viviendas captadas por cada zona.

        * La distribución de propiedades captadas por cada ejecutivo.

  

    "
![Screenshot1](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/Screenshot1.png)

    

Nuevamente, es un Problema ficticio para el propósito del proyecto.

Los pasos que realice para llevar a cabo este proyecto fueron:



🧹 En primer lugar realicé una transformación y limpieza de los datos. Existían ciertos datos anómalos entre los registros, que no coincidían con el tipo de dato del campo al que pertenecían. Por ejemplo, en la columna del precio, habían ciertos datos que no eran de tipo numérico, y los convertí a números. Otros contenían texto como "Vendido", los que poseían valores como este, se eliminaban porque no eran relevantes para el proyecto, ya que solo me interesaban los que se tenían en inventario.

![Screenshot2](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/screenshot2.png)


![Screenshot3](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/screenshot3.png)



🔍 Posteriormente, me concentre en realizar análisis en base a las preguntas planteadas inicialmente en el Problema. Calculando el precio máximo, el precio mínimo y el precio promedio. Tambien, la cantidad de apartamentos captados por la Inmobiliaria por cada zona de Valencia. Y por ultimo la cantidad de viviendas captadas por cada vendedor.

![Cantidad de propiedades por zona](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/Cantidad%20propiedades%20por%20zona.png)


![Cantidad de propiedades por captador](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/Cantidad%20de%20propiedades%20por%20vendedor.png)


🔬 Luego, empece a realizar los pasos de procesamiento de datos respectivos para construir el modelo. Verifiqué por medio de gráficos de dispersion la relación entre las variables independientes con la dependiente. A primera vista no se veia una relacion lineal concisa con ninguna de las variables, pero aun así seguí mi camino para ver el resultado final. Posteriormente realice la codificacion de las variables de texto para que pudieran ser tomadas por el modelo (cabe destacar que utilice todas las variables para la construccion del modelo). Y despues dividí el dataset en los sets de prueba y entrenamiento.

![Screenshot6](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/Screenshot6.png)



⚗️Y por ultimo realice la construccion del modelo y su respectivo entrenamiento. Luego para validar su rendimiento, obtuve los valores de R^2 (coeficiente de determinacion) y el valor p. El primero arrojó un resultado optimo (0.9919696791747508). Sin embargo, la significancia estadistica (valor p) no era la mejor. Todos los valores p superaban la medida deseada de 0.05. Por lo que no existia una probabilidad alta de que los datos que se dieran en el modelo fueran producto del azar.

![Screenshot7](https://github.com/ENYEL00/Proyecto-Inmobiliaria/blob/main/Proyecto%20Inmobiliaria/Screenshot7.png)


📝 De igual forma, no me rendi. Utilice el modelo para realizar la prueba del modelo (Es decir, realizar las predicciones junto con el dataset de prueba) y validar la diferencia entre los resultados del modelo y los valores originales. En resumen, los valores predichos no se acercaron a los valores originales y no se pudo realizar la estimacion correctamente.


## En conclusion.

Si bien los datos ya estaban predispuestos a fallar en la estimacion y el proyecto, segui con el proyecto con la intencion de terminar la practica. Los datos no eran los suficientes como para realizar una estimacion correcta y las caracteristicas tampoco eran las suficientes. Es decir, faltaron registros (el dataset no tenia mas de 100 registros) y al mismo tiempo faltaron caracteristicas por tomar en cuenta ya que hay muchas cosas que determinan el valor de una vivienda, y mas en la ciudad de Valencia que es un mercado relativamente inestable. De igual forma, si llegase a conseguir un dataset mas robusto y poder realizar el proyecto con un modelo de Machine Learning mas robusto tambien, no dudare en volver a repetir el proyecto.


## Para terminar.

Al mismo tiempo realice un dashboard con la informacion mas relevante para una empresa en el sector, tomando en cuenta los datos que poseo. No agregue los resultados del modelo, pero el dashboard es algo que dé valor.

![Ver Dashboard]([https://app.powerbi.com/view?r=eyJrIjoiMTY2MGI4MjctZjFhNy00MmQ5LTgxZjUtMGJjYWM0NTgzMWY0IiwidCI6ImNkZWMyMTM0LTAzNjMtNGZkNC04MTU2LTYwMDMwMThmZjQ1MSIsImMiOjR9&pageName=b2429c7251b581496d58](https://app.powerbi.com/view?r=eyJrIjoiMWEyMzFlNGUtZGZlOC00ZWJmLWI3ZWYtYzIyZjgyY2VhNDRkIiwidCI6ImNkZWMyMTM0LTAzNjMtNGZkNC04MTU2LTYwMDMwMThmZjQ1MSIsImMiOjR9))
