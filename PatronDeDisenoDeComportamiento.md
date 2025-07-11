#  📖 Anexo - Aplicación de Patrón de Diseño de Comportamiento - Facade #

Los patrones de diseño de Comportamiento se enfocan en cómo interactúan los objetos entre sí y cómo se reparten las responsabilidades. Permiten mejorar la comunicación entre objetos sin acoplarlos fuertemente.

Para este caso seleccionamos el patrón Observer, que permite definir una dependencia de uno a muchos entre objetos de manera que cuando alguno cambie de estado se notifiquen a sus dependientes de manera automática.

En este sistema, lo vamos a utilizar para que cuando se confirme un turno o se realice una modificación en el mismo, notifique automaticamente al profesional y al paciente.

## Motivación ##

En el sistema de gestión de turnos se debía notificar automáticamente a pacientes y profesionales cada vez que se confirmaba, modificaba o cancelaba un turno. Originalmente, esta lógica de envío estaba embebida dentro de las clases Turno y ServiciosTurnos, lo cual provocaba una alta dependencia entre la lógica de negocio y el canal de notificación.

Este diseño era poco flexible y escalable. Por ejemplo, agregar un nuevo canal (como SMS o WhatsApp) requería modificar directamente estas clases, rompiendo el principio de abierto/cerrado.

Para resolver este problema, se aplicó el patrón Observer. La clase Turno se transformó en el Sujeto Observable, y las clases como NotificadorMail o NotificadorSMS implementan la interfaz ObservadorNotificacion.

 ## Estructura de Clases ##
+ [Diagrama Clases Singleton](https://drive.google.com/file/d/18EXj6MZd9iqKkE2AVVxL3Uo1zE0w5z1b/view?usp=sharing)
<img width="671" height="664" alt="image" src="https://github.com/user-attachments/assets/96593647-bc4b-414f-890c-f0cb7882f06c" />
