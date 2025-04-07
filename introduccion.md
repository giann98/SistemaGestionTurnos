:card_index_dividers:	# Anexo - Introducción al Diseño Orientado a Objetos #

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


## 🗂 Casos de Uso

---

### ✅ Solicitar Turno
- **Actor:** Paciente  
- **Descripción:** Un paciente solicita un turno con un profesional disponible.

**Flujo Principal:**
1. El paciente ingresa al sistema.  
2. Selecciona un profesional y verifica la fecha de disponibilidad.  
3. Confirma el turno.  
4. El sistema envía una notificación de confirmación.

**Precondiciones:**  
El paciente debe estar registrado.

**Postcondiciones:**  
El turno queda registrado y notificado.

---

### ✅ Registrar Profesional de la Salud
- **Actor:** Administrador del sistema  
- **Descripción:** Se agrega un nuevo profesional al sistema.

**Flujo Principal:**
1. El administrador ingresa al sistema.  
2. Ingresa los datos del profesional en un formulario.  
3. Establece su especialidad con fecha y horarios de atención.  
4. Guarda la información.

**Precondiciones:**  
El profesional debe contar con matrícula válida y el administrador con credenciales adecuadas.

**Postcondiciones:**  
El profesional queda registrado en el sistema.

---

### ✅ Notificar Cambio de Turno
- **Actor:** Administrador / Profesional / Paciente  
- **Descripción:** Se notifica a los usuarios cuando un turno es modificado.

**Flujo Principal:**
1. El profesional o el administrador entra al sistema.  
2. Registra un cambio en un turno.  
3. El sistema genera y envía una notificación a los afectados.

**Precondiciones:**  
Debe existir un turno activo.

**Postcondiciones:**  
El paciente y el profesional reciben la notificación.

---

### ✅ Cancelar Turno
- **Actor:** Paciente o Profesional  
- **Descripción:** Un turno es cancelado.

**Flujo Principal:**
1. El usuario ingresa al sistema.  
2. Selecciona un turno existente.  
3. Solicita la cancelación.  
4. El sistema actualiza el estado y envía una notificación.

**Precondiciones:**  
Debe existir un turno registrado para el usuario seleccionado.

**Postcondiciones:**  
El turno queda cancelado y se libera el horario, notificando a los usuarios.

---

### ✅ Consultar Historial de Turnos
- **Actor:** Paciente o Profesional  
- **Descripción:** Se consulta el historial de turnos asignados.

**Flujo Principal:**
1. El usuario ingresa al sistema.  
2. Selecciona la opción "Historial".  
3. Visualiza la lista de turnos anteriores.

**Precondiciones:**  
Debe existir al menos un turno registrado para el usuario consultado.

**Postcondiciones:**  
Se muestra el historial de turnos.
## Boceto inicial del Diseño de Clases ##

![Diseño clases](https://github.com/user-attachments/assets/76bc70c0-c786-494e-b282-fc937b5b1472)
