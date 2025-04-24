# Principio de Inversión de Dependencias (DIP) #

## Proposito ##

Las clases deben depender de abstracciones, no de implementaciones concretas.

## Motivación ##

Actualmente, la clase Turno interactua directamente con la clase Notificación. Si se reemplaza Notificación por otro tipo, como NotificacionMail o se tiene que utilizar esa clase, se tendría que modificar Turno para tal vez agregar nuevos parametros de envio. Para evitarlo, se puede utilizar una interfaz llamada Notificador, que se inyecta a Turno. En vez de instanciar una notificación concreta dentro de Turno, esta clase recibiría una interfaz Notificador como dependencia externa y la clase Notificacion deberia derivar a la clase correspondiente.



