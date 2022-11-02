//QUE ES DEPENDENCY INJECTION

La inversión de dependencias es un principio que describe un conjunto de técnicas destinadas a disminuir el acoplamiento entre los componentes de una aplicación. Es uno de los principios SOLID más populares y utilizados en la creación de aplicaciones, frameworks y componentes por las ventajas que aporta a las mismas.

La inversión de dependencias suele también conocerse como inversión de control. En inglés, los términos más frecuentemente utilizados son "dependency inversion", abreviado como "DI", e "inversion of control" o simplemente "IoC".

//ESTRUCTURA

1. Tiene bastantes líneas de código de "fontanería", dedicadas a instanciar y preparar las dependencias, en lugar de centrarse en su misión, que es eliminar una factura y notificar al administrador.

2. Observa además que, muchas de esas líneas deberían repetirse en otros métodos de la clase que requirieran los servicios de estos componentes. Por ejemplo, otros métodos, como Add() o Update(), probablemente necesitarían acceder al repositorio de facturas y quizás también al componente de notificación.

3. Estamos atando inexorablemente la implementación de InvoiceServices a InvoiceRepository e EmailNotifier. Cualquier modificación en estas últimas podría afectar a la primera, o incluso requerir cambios en ésta.

4. Complicamos la reutilización de la clase, puesto que siempre va a ir unida a los componentes de los que depende.

5. No quedan claras las dependencias de la clase. Para conocerlas deberíamos leer todo su código y ver qué clases externas utiliza. Aunque en ese ejemplo no es un problema porque es poco código, en clases más extensas sí sería bastante complicado determinarlas.

6. Dificultamos la realización de pruebas unitarias, puesto que no hay forma de probar únicamente el correcto funcionamiento del método Remove() de InvoiceServices sin probar al mismo tiempo el funcionamiento de las clases de las que depende.

[![image.png](https://i.postimg.cc/rpvsphR2/image.png)](https://postimg.cc/p9JRGJBs)
