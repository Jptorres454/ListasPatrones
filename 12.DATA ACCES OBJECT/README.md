//QUE ES DATA ACCES OBJECT

Dado lo anterior, el patrón DAO propone separar por completo la lógica de negocio de la lógica para acceder a los datos, de esta forma, el DAO proporcionará los métodos necesarios para insertar, actualizar, borrar y consultar la información; por otra parte, la capa de negocio solo se preocupa por lógica de negocio y utiliza el DAO para interactuar con la fuente de datos.

//ESTRUCTURA

1. El BusinessObject creo u obtiene una referencia al DataAccessObject.

2. El BusinessObject solicita información al DataAccessObject
 - El DataAccessObject solicita la información al DataSource
 - El DataAccessObject crea una instancia del TransferObject con los datos recuperados del DataSource
 - El DataAccessObject response con el TransferObject creado en los pasos anteriores.

3. El BusinessObject actualiza algún valor del TransferObject
 - Más actualizaciones

4. El BusinessObject solicita el guardado de los datos actualizados al DataAccessObject.
 - El DataAccessObject guarda los datos en el DataSource.
 
[![image.png](https://i.postimg.cc/1zKwV1P1/image.png)](https://postimg.cc/v1ccCjc0)
