#  📖 Anexo - Aplicación de Patrón de Diseño Estructural - Facade #

Los patrones de diseño estructual definen cómo se relacionan y componen entre sí las clases y objetos. Enfocados en la estructura del sistema, estos facilitan la reutilización de componentes y simplifican relaciones complejas entre objetos.

Para este caso seleccionamos el patrón Facade, que proporciona una interfaz simplificada y única para un conjunto de interfaces en un subsistema complejo.

En este sistema, ServicioTurnos puede actuar como fachada para coordinar la validación, asignación, notificación y persistencia de los turnos.

## Motivación ##

Durante el desarrollo del sistema, se detectó que el proceso de gestión de turnos involucraba múltiples operaciones complejas y distribuidas entre diversas clases: Turno, RepositorioTurnos, ServiciosTurnos, Notificación, etc. Esto provocaba que las clases de alto nivel (como Paciente o Administrador) tuvieran que interactuar con demasiadas dependencias y conocer detalles internos del sistema, violando el principio de ocultamiento.

Para simplificar esta interacción, se aplicó el patrón Facade, mediante la implementación de una clase GestorTurnosFacade. Esta clase actúa como puerta de entrada unificada para todas las operaciones relacionadas con turnos, y delega internamente a las clases correspondientes.

 ## Estructura de Clases ##
+ [Diagrama Clases Singleton](https://drive.google.com/file/d/1qoEI0CsREAPI8j7b6maCZVjrdXr9WWvg/view?usp=sharing)
<img width="537" height="473" alt="image" src="https://github.com/user-attachments/assets/22dbafcc-6658-456f-a912-a026b343d45a" />
