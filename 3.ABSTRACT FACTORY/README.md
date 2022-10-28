//QUE ES LA ABSTRACT FACTORY?
  
  La creación de familias de objetos relacionados o dependientes sin especificar directamente sus clases concretas. El objeto "fábrica" tiene la responsabilidad de proporcionar servicios de creación para toda la familia de plataformas. Los clientes nunca crean objetos de plataforma directamente, le piden a la fábrica que lo haga por ellos.

  Este mecanismo facilita el intercambio de familias de productos porque la clase especifica del objeto de fabrica aparece solo una vez en la aplicacion, donde se instancia. La aplicacion puede reemplazar al por mayor toda la familia de productos simplemente instanciando una instancia concreta diferente de la Abstract Factory.
  
  ![image](https://user-images.githubusercontent.com/107562989/198640951-63e3cfce-47c9-4ee6-8d52-4f6eacf555d8.png)

//ESTRUCTURA
  
  El metodo de Abstract Factory define un metodo de fabrica por producto. Cada metodo Factory encapsula el 'new' operador y las clases de productos concretas y especificas de la plataforma. Luego, cada "plataforma" se modela con una clase derivada de factory.
  ![image](https://user-images.githubusercontent.com/107562989/198643185-38e5475b-3482-4a4e-a1cf-0f0e134da4db.png)
  
