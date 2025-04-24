# Principio de Sustitución de Liskov (LSP) #

## Proposito ##

Las subclases deben poder sustituir a sus clases base sin alterar el comportamiento esperado del sistema.

## Motivación ##

La clase Turno que sería la clase base, en caso de generarse diferentes modalidades de turno, como puede ser un turno virtual, debe generarse una nueva subclase, dependiente de Turno, que podría llamarse TurnoVirtual. Sin importar que tipo de turno sea, deberia permitir solicitar turnos sin modificar el comportamiento del metodo confirmarTurno. De esta forma, el metodo deberia permitir confirmar un turno sea virtual o presencial sin modificar la lógica del metodo.




