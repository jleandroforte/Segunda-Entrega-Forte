# Segunda-Entrega-Forte
Segunda pre-entrega del curso de Data Sciente 46320


El dataset con el que vamos a trabajar recopila datos de ventas y actividad de los clientes en el sitio web de una farmacia online a lo largo de 90 días.

Tenemos información sobre varias características de los productos que serán detalladas en secciones siguientes, sus precios, los precios de la competencia y comportamiento de los clientes, si hacen click en un producto, si los colocan en una canasta de productos y finalmente si compran un producto. Nótese que no todas las líneas representan ventas.

La clave del dataset es que la farmacia sigue una política de 'pricing dinámico' donde los precios de cada producto son ajustados diariamente, dentro de ciertas bandas.

**Objetivos**

Nuestro objetivo va a ser predecir el revenue, y para ello vamos a utilizar 2 enfoques:

**Modelo de Regresion**

basandonos en lo siguiente:

> 1. Nuestros datos están etiquetados. En principio, no tenemos la necesidad de hacer un análisis no supervisado.

> 2. La variable independiente es el revenue, o ingresos que generan las ventas (no todas las líneas representan ventas, por tanto, el revenue es 0 en muchas líneas), es una variable numérica continua, es decir, no son dicótomicas como podría requerir una regresión logística, con lo cual un modelo de regresión, en principio, se adecúa a nuestros objetivos. Recordemos que el objetivo al final del curso es usar este dataset para construir un modelo que **prediga** el revenue en base a las restantes variables donde, fundamentalmente, lo que cambia es el vector de precios.

**Modelo de clasificación decision tree**

En este caso, no vamos a predecir directamente el revenue, sino la variable order, que, recordemos, toma valores 0 y 1, cuando es 1, significa que una línea representa una venta, y esa venta tiene un revenue asociado. Es decir, corremos ligeramente el foco del análisis, y como paso intermedio, exploramos **que variables determinan las ventas**
