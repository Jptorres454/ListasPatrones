//QUE ES FACTORY?

  Es para crear objetos como implementar un algoritmo. Una superclase especifica todo el comportamiento estandar y generico(Usando "marcadores de posicion" virtuales puros ara los pasos de creacion), y luego delega los detalles de creacion de las subclases que proporciona el cliente.
  Es un diseño sea mas personalizable y solo un poco mas complicado. Otros patrones de diseño requiren nuevas clases, mientras que el metodo factory solo requiere una nueva operacion.
  
//ESTRUCTURA
  
  La implementacion del metodo factory discutida en Gang of Four(abajo) se supones en gran medida con la abstract factory. Por esa razon, la presentacion de este capitulo se centra en el enfoque que se ha vuelto popular desde entonces.
  ![image](https://user-images.githubusercontent.com/107562989/198632719-5016d744-8a16-4b11-8660-618350053b2e.png)

  Una definicion cada vez mas popular de metodo de fabrica es: un'static' metodo de una clase que vuelve un objeto del tipo de esa clase. Pero a diferencia de un constructor, el objeto real que devuelve podria ser una instnacia de una subclase. A diferencia de un constructor, los metodos de fabrica pueden tener nombres diferentes y mas descriptivos como por ejemplo('Color.make_RGB_color(float red, float green, float blue)'y'Color.make_HSB_color(float hue, float saturation, float brightness)').
  ![image](https://user-images.githubusercontent.com/107562989/198635663-b5563f42-935d-454b-8aeb-03a03b21195c.png)
  
  El cliente esta totalmente desvinculado de los detalles de implementacion de las clases derivadas. La creacion polimorfica ahora es posible.
  ![image](https://user-images.githubusercontent.com/107562989/198636292-2082153a-c7f7-4896-864a-da69dbd3c7e1.png)
   
   El metodo Factory define una interfaz para crear objetos, pero permite que las subclases decidan que clases instanciar. Las prensas de moldeo de plastico e inyectan el plastico en moldes de las formas deseadas.
   La clase de juguete(autoovil, figura de accion, etc.) esta determinada por el molde.
   ![image](https://user-images.githubusercontent.com/107562989/198637453-8881b722-e504-4930-8162-a5397bdd4f0f.png)
