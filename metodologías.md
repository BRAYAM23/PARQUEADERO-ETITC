# Diseño de Solución para el Sistema de Parqueadero Automatizado ETITC

## 1. Metodología Tradicional: Cascada (Waterfall)

**Descripción:**  
La metodología en cascada es secuencial y lineal. Cada fase depende de la finalización de la anterior. Es adecuada para proyectos con requisitos bien definidos desde el principio.

### Fases y Descripción:

1. **Requisitos:**
   - El sistema debe permitir la entrada y salida automatizada de vehículos.
   - Utilizar reconocimiento de placas y tarjetas electrónicas.
   - Integración con el carnet estudiantil para acceso de estudiantes.
   - Monitoreo de la ocupación en tiempo real.
   - Generación de reportes sobre el uso del parqueadero.

2. **Diseño:**
   - **Diseño del Sistema:** Diagrama de arquitectura del software que incluye módulos para reconocimiento de placas, control de acceso, registro de usuarios y monitoreo de ocupación.
   - **Diseño de Base de Datos:** Tablas para almacenar datos de usuarios, vehículos, accesos y ocupación del parqueadero.

3. **Implementación:**
   - Desarrollar el sistema con un lenguaje como Java o Python para la parte del software.
   - Integrar hardware con cámaras de reconocimiento de placas y lectores de tarjetas RFID.

4. **Pruebas:**
   - Pruebas unitarias para cada módulo del sistema.
   - Pruebas de integración para asegurar que los módulos interactúan correctamente.
   - Pruebas de estrés para verificar el rendimiento bajo alta carga.

5. **Mantenimiento:**
   - Monitoreo continuo y corrección de errores.
   - Actualizaciones para mejorar funcionalidades según sea necesario.

### Roles:
- **Analista de Negocios:** Define requisitos.
- **Arquitecto de Software:** Diseña la solución.
- **Desarrolladores:** Implementan el sistema.
- **Ingenieros de Pruebas:** Realizan las pruebas.
- **Administrador del Sistema:** Mantenimiento.

---

## 2. Metodologías Ágiles

### a. Scrum

**Descripción:**  
Scrum es una metodología ágil que se enfoca en entregas incrementales, con el trabajo dividido en sprints (ciclos cortos). Ideal para proyectos con requisitos cambiantes.

### Proceso Scrum:

1. **Requisitos:**
   - El sistema debe ser flexible y permitir modificaciones según las necesidades del parqueadero.
   - Inicialmente, se enfocará en el acceso automatizado por placa y carnet estudiantil.

2. **Sprint 1:**
   - **Objetivo:** Implementar el acceso automatizado usando reconocimiento de placas.
   - **Tareas:**
     - Desarrollar el módulo de reconocimiento de placas.
     - Probar el acceso con una base de datos de usuarios.

3. **Sprint 2:**
   - **Objetivo:** Integrar el carnet estudiantil y tarjetas RFID para el control de acceso.
   - **Tareas:**
     - Programar la integración con el carnet estudiantil.
     - Desarrollar pruebas para validar el flujo de entrada/salida.

4. **Sprint 3:**
   - **Objetivo:** Monitorear la ocupación en tiempo real.
   - **Tareas:**
     - Crear un sistema de monitoreo visual para el personal de seguridad.
     - Probar la precisión del monitoreo.

### Roles en Scrum:
- **Product Owner:** Define los requisitos y prioridades (Director de Parqueadero).
- **Scrum Master:** Facilita el trabajo del equipo y elimina impedimentos (Jefe de Proyectos).
- **Equipo de Desarrollo:** Desarrolla y prueba el sistema (Desarrolladores, QA).

---

### b. Kanban

**Descripción:**  
Kanban es una metodología visual que gestiona el flujo de trabajo de manera continua. Se centra en limitar el trabajo en curso y mejorar la eficiencia.

### Proceso Kanban:

1. **Columnas del tablero Kanban:**
   - **Backlog:** Acceso automatizado, integración con tarjetas, monitoreo de ocupación.
   - **En Progreso:** Implementación del reconocimiento de placas.
   - **En Revisión:** Pruebas de integración del sistema con RFID.
   - **Finalizado:** Monitoreo de ocupación en tiempo real.

2. **Mejora Continua:**
   - Se revisa el flujo de trabajo en reuniones diarias y se ajusta según los bloqueos o cuellos de botella.
   - Se agregan nuevas funcionalidades al **Backlog** cuando surgen nuevas necesidades, por ejemplo, generación de reportes.

### Roles en Kanban:
- **Product Manager:** Define las prioridades.
- **Desarrolladores:** Implementan y mueven las tareas a través del tablero.
- **QA:** Se encarga de probar las funcionalidades completadas.

---

### c. Extreme Programming (XP)

**Descripción:**  
XP es una metodología ágil que enfatiza la colaboración cercana con el cliente, ciclos de retroalimentación rápidos y técnicas como la programación en pareja y pruebas automatizadas.

### Proceso XP:

1. **Planificación:**
   - Se definen historias de usuario para cada funcionalidad: "Como estudiante, quiero ingresar al parqueadero usando mi carnet."

2. **Desarrollo:**
   - **Programación en Pareja:** Dos desarrolladores trabajan juntos para asegurar calidad y compartir conocimientos.
   - **Pruebas Automatizadas:** Cada funcionalidad se prueba de forma continua a medida que se desarrolla.
   - **Iteraciones Cortas:** Entregas frecuentes cada 1-2 semanas.

3. **Retroalimentación:**
   - El cliente (administrador del parqueadero) revisa las entregas y proporciona retroalimentación inmediata para ajustar el sistema.

### Roles en XP:
- **Cliente:** Proporciona retroalimentación constante.
- **Desarrolladores:** Implementan el sistema en parejas.
- **QA:** Se encargan de las pruebas automatizadas y la calidad del código.

---

## Conclusión

- **Metodología Tradicional (Cascada):** Adecuada si los requisitos están completamente definidos desde el inicio y no se espera que cambien.
- **Metodologías Ágiles (Scrum, Kanban, XP):** son buenos si el proyecto requiere flexibilidad y evolución continua, permitiendo entregas rápidas y ajustes basados en retroalimentación.
