#  📖 Anexo - Aplicación de Patrón de Diseño Creacional - Singleton #

Los patrones de diseño creacionales se enfocan en cómo se crean los objetos. Ayudan a separar el proceso de creación de objetos de su uso, lo que permite mayor flexibilidad y reutilización.

Para este caso seleccionamos el patrón Singleton, que asegura que una clase tenga una única instancia y proporciona un punto global de acceso a ella.

En este sistema, la clase RepositorioTurnos debe tener una única instancia para garantizar la integridad de los datos al gestionar múltiples operaciones sobre los turnos (crear, eliminar, modificar, buscar).

## Motivación ##

En el sistema de gestión de turnos, la clase RepositorioTurnos es responsable de almacenar y recuperar todos los turnos registrados, actuando como una base de datos en memoria o una interfaz hacia un backend persistente.

Durante el desarrollo se detectó que distintas partes del sistema accedían a este repositorio para consultar o modificar turnos: clases como ServiciosTurnos, Administrador, Paciente, etc. Sin un mecanismo centralizado, podían crearse múltiples instancias del repositorio, llevando a datos inconsistentes y duplicación de turnos, especialmente en operaciones concurrentes o en ambientes simulados de prueba.

Para resolver este problema, se implementó el patrón Singleton sobre la clase RepositorioTurnos, garantizando que:

+ Solo exista una única instancia del repositorio durante toda la ejecución del sistema.

+ Todas las clases que necesitan acceder a los turnos trabajen sobre la misma instancia compartida.

+ Se asegure la integridad de los datos y la sincronización del estado del sistema.

 ## Estructura de Clases ##
+ [Diagrama Clases Singleton](https://drive.google.com/file/d/1AwOgeWKY0YhElN4xBLfdtAIYHlGg2Wri/view?usp=sharing)
<img width="511" height="794" alt="image" src="https://github.com/user-attachments/assets/b1e0d31f-1989-40d3-a81f-38e80a5c5205" />

