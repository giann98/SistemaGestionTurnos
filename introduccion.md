# Anexo - Introducción al Diseño Orientado a Objetos #

### **Programación Orientada a Objetos (POO)** ###

La Programación Orientada a Objetos (POO) es un paradigma de programación que organiza el código en torno a "objetos" en lugar de funciones y procedimientos. Cada objeto es una instancia de una clase y puede contener datos (atributos) y comportamientos (métodos). Este enfoque facilita la reutilización de código, la modularidad y el mantenimiento del software.

### **Importancia de la POO** ###

La POO permite modelar problemas del mundo real de manera intuitiva, dividiendo el sistema en entidades que interactúan entre sí. Esto hace que el código sea más comprensible, reutilizable y fácil de mantener.

## Los cuatro fundamentos de la POO  ##

1. **Encapsulamiento:** Protege los datos dentro de un objeto, permitiendo el acceso solo a través de métodos definidos.<br> Ejemplo: Un cajero automático, te permite consultar tu saldo y/o retirar efectivo siempre y caundo sepas la clave de tu cuenta.

2. **Herencia:** Permite que una clase derive de otra, reutilizando atributos y métodos.<br> Ejemplo: La clase "Médico" hereda propiedades de la clase "Persona", todo Médico es una persona y comparte sus características.

3. **Polimorfismo:** Permite que un mismo método tenga diferentes comportamientos según el objeto que lo usa.<br> Ejemplo: La clase "Médico" y la clase "Enfermera" pueden tener un método "atenderPacientes" con diferentes implementaciones, la enfermera lo tiende de cierta forma y el Médico puede aplicar otros tratamientos dentro del mismo método.

4. **Abstracción:** Permite centrarse en los aspectos esenciales de un objeto sin preocuparse por los detalles internos.<br> Ejemplo: Un cliente usa un "sistema de turnos" sin conocer cómo funciona internamente.

## Requisitos Iniciales del Sistema ##

+ **Registrar pacientes con datos personales y de contacto.** <br>

+ **Registrar profesionales de la salud con su información y horarios de atención.** <br>

+ **Asignar turnos evitando sobreasignaciones.** <br>

+ **Enviar notificaciones automáticas a pacientes y profesionales según el estado de los turnos.** <br>

+ **Permitir la consulta y gestión del historial de turnos.** <br>

+ **Aplicar seguridad y control de acceso a la información.** <br>

## Casos de Uso ## 

## Boceto inicial del Diseño de Clases ##
