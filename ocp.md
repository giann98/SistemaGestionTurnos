# Principio de Abierto/Cerrado (OCP) #

## Proposito ##

Una clase debe estar abierta para ser extendida, pero cerrada para ser modificada.

## Motivación ##

La clase Notificación puede crecer en funcionalidades o de notificaciones a enviar, por ejemplo se pueden ir agregando diferentes medios de notificación, como puede ser envio por mail, por whatsapp o generar un push en la aplicación. Al aplicar el principio OCP, no se debe modificar la clase actual Notificación, sino que se deben crear subclases por cada tipo de notificación, como puede ser NotificacionEmail, NotificacionWhatsapp.


