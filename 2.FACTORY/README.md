//QUE ES FACTORY?

  Es para crear objetos como implementar un algoritmo. Una superclase especifica todo el comportamiento estandar y generico(Usando "marcadores de posicion" virtuales puros ara los pasos de creacion), y luego delega los detalles de creacion de las subclases que proporciona el cliente.
  Es un diseño sea mas personalizable y solo un poco mas complicado. Otros patrones de diseño requiren nuevas clases, mientras que el metodo factory solo requiere una nueva operacion.
  
//ESTRUCTURA
  
  La implementacion del metodo factory discutida en Gang of Four(abajo) se supones en gran medida con la abstract factory. Por esa razon, la presentacion de este capitulo se centra en el enfoque que se ha vuelto popular desde entonces.
  ![image](https://user-images.githubusercontent.com/107562989/198632719-5016d744-8a16-4b11-8660-618350053b2e.png)
