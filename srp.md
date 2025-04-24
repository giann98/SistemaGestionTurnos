# Principio de Responsabilidad Única (SRP) #

## Proposito del principio: ##

Este principio establece que cada clase debe tener una única responsabilidad y, por lo tanto, una sola razón para cambiar. Evita que una clase tenga demasiadas funciones, lo que facilita el mantenimiento del sistema.

## Motivación: ##

La clase Turno actualmente almacena la información del turno (fecha, hora, estado) y gestiona el vínculo con el paciente y el profesional. Si en un futuro se comenzara a incluir lógica adicional como validaciones de reglas complejas (por ejemplo, "no se pueden otorgar más de 10 turnos por día para un profesional"), se estaría rompiendo el SRP, para solucionar esto se podría generar una nueva clase llamada por ejemplo ValidadorTurno.

