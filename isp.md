# Principio de Segregación de Interfaces (ISP) #

## Proposito ##

Es mejor tener varias interfaces pequeñas y específicas que una sola interfaz grande con métodos que no siempre se usan.

## Motivación ##

Si la clase Administrador se encarga de registrar profesionales y a su vez puede asignar o modificar turnos, la interfaz que utilice el administrador no debe ser la misma interfaz que tiene que ver la clase Paciente por ejemplo para solicitar o modificar un turno. De esta manera, deben generarse las interfaces necesarias para cada clase dependiendo de que permisos y cosas pueda realizar en el sistema. Se pueden separar en 2 interfaces, Interfaz de Registro profesional e Interfaz de Solicitud de Turno



