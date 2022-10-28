//QUE ES LA LISTA DE PATRONES DE SINGLETON?

  El patron de diseño Singleton, tambien conocida instancia unica esta diseñado para restringir la creacion de objetos pertenecientes a una clase o el valor de un tipo a un unico objeto.
  Su intencion consiste en garantizar que una clase solo tenga una instancia y proporcionar un punto de acceso global a ella. No se encarga de la creacion de objetos en si, sino que se enfoca en la restriccion en la creacion de un objeto.
  
  [![image.png](https://i.postimg.cc/W4HpgkGt/image.png)](https://postimg.cc/zLT113P1)

  El patron Singleton asegura que una clase tenga solo una instancia y proporciona un punto de acceso global a esa instancia. Lleva el nombre del conjunto singleton, que se define como un conjunto que contiene un elemento. La oficina del presidente de los Estados Unidos es un Singleton.
  
  [![image.png](https://i.postimg.cc/X7qbcJvC/image.png)](https://postimg.cc/yWMt77c1)
  
  
 //LISTAS DE VERIFICACION.
  
  - Definir un 'static' atributo privado en la clase de "instancia unica" tambien es una funcion de acceso publico en la clase
  - La realizacion con una "inicializacion diferida"(creacion en el primer uso) en la funcion de acceso.
  - Defina todos los constructores para que sean 'protected' o 'private'.
  - Solo los clientes pueden usar la funcion de acceso para manipular el Singleton
