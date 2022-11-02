//QUE ES PROXY

El patrón Proxy sugiere que crees una nueva clase proxy con la misma interfaz que un objeto de servicio original. Después actualizas tu aplicación para que pase el objeto proxy a todos los clientes del objeto original. Al recibir una solicitud de un cliente, el proxy crea un objeto de servicio real y le delega todo el trabajo.

//ESTRUCTURA

1. La Interfaz de Servicio declara la interfaz del Servicio. El proxy debe seguir esta interfaz para poder camuflarse como objeto de servicio.

2. Servicio es una clase que proporciona una lógica de negocio útil.

3. La clase Proxy tiene un campo de referencia que apunta a un objeto de servicio. Cuando el proxy finaliza su procesamiento (por ejemplo, inicialización diferida, registro, control de acceso, almacenamiento en caché, etc.), pasa la solicitud al objeto de servicio.

Normalmente los proxies gestionan el ciclo de vida completo de sus objetos de servicio.

4. El Cliente debe funcionar con servicios y proxies a través de la misma interfaz. De este modo puedes pasar un proxy a cualquier código que espere un objeto de servicio.

[![image.png](https://i.postimg.cc/Sx3WbfrH/image.png)](https://postimg.cc/TKjyrmBc)
