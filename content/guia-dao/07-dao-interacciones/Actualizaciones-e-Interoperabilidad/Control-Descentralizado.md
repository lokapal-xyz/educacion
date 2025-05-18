---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Garantías de Control Descentralizado de las Actualizaciones'
weight: 117_000
---

La capacidad de una DAO para actualizar sus contratos e infraestructura debe equilibrarse con la descentralización para evitar puntos críticos de fallo o tomas de control de la gobernanza. Exploremos los mecanismos, herramientas y estrategias que las DAO pueden utilizar para mantener un control descentralizado sobre las actualizaciones, garantizando al mismo tiempo la seguridad y la eficiencia.

---

## **¿Por qué es importante el control descentralizado sobre las actualizaciones?**

Si bien las actualizaciones de los contratos inteligentes y los cambios de gobernanza son necesarios para la adaptabilidad, los mecanismos de actualización mal diseñados pueden:

- **Introducir riesgos de centralización** → Si un grupo pequeño controla las actualizaciones, puede anular las decisiones de la comunidad.

- **Permitir tomas de control maliciosas** → Los atacantes podrían explotar los mecanismos de actualización para tomar el control de la DAO.

- **Reducir la transparencia y la confianza** → Las actualizaciones unilaterales pueden erosionar la confianza de la comunidad en la gobernanza.

Para prevenir estos riesgos, las DAO deben diseñar procesos de actualización que permanezcan descentralizados y alineados con la gobernanza de la comunidad.

---

## **Estrategias Clave para el Control Descentralizado de Actualizaciones**

### **Aprobaciones de Actualizaciones Impulsadas por la Gobernanza**
- Exigir la votación en cadena para las actualizaciones, garantizando que la comunidad controle los cambios de protocolo.
- Utilizar la votación instantánea para la señalización fuera de la cadena antes de comprometerse con la ejecución en cadena.
- Establecer umbrales mínimos de quorum y aprobación para evitar que grupos pequeños se apropien de la gobernanza.

- ---

### **Ejecución de Actualizaciones Controlada por Multifirma**
- Utilizar billeteras multifirma (p. ej., Gnosis Safe) para ejecutar actualizaciones solo si varios firmantes de confianza las aprueban.
- Asegurarse de que la multifirma se distribuya entre un grupo diverso de miembros de la comunidad.
- Considerar la rotación de firmantes para evitar la centralización a largo plazo.

- ---

### **Bloqueos de Tiempo para Evitar Actualizaciones Instantáneas**
- Implementar bloqueos de tiempo en las actualizaciones para proporcionar un período de espera antes de que los cambios surtan efecto. Esto permite a la comunidad revisar y reaccionar si se propone un cambio malicioso o imprevisto.

---

### **Mecanismos de Gobernanza de Emergencia**
--- Establecer poderes de veto de emergencia que permitan a la DAO detener las actualizaciones en caso de un ataque.
--- Utilizar consejos de seguridad elegidos por la comunidad para evaluar los riesgos de seguridad urgentes.

---

### **Contratos Actualizables con Supervisión Comunitaria**
--- Utilizar patrones UUPS o Proxy Transparente, pero requerir la aprobación de la gobernanza para nuevas implementaciones.
--- Evitar mecanismos de actualización controlados por administradores que eludan la gobernanza de la comunidad.
--- Publicar las propuestas de actualización con antelación para permitir el escrutinio público.

---

## **Transparencia y Participación Comunitaria**

Incluso con las medidas de seguridad técnicas, las DAO deben garantizar la transparencia y una amplia participación en las decisiones de actualización:

--- **Discusiones Públicas de Gobernanza** → Utilizar foros como Discourse para debatir las actualizaciones antes de la votación formal. - **Código abierto y auditorías** → Las propuestas de actualización se pueden revisar públicamente y se someten a auditorías de seguridad.

- **Descentralización progresiva** → Transición gradual del control de los equipos centrales a la comunidad en general.

---

## **Desafíos y desventajas**

- **Demasiada centralización** → Actualizaciones rápidas, pero con riesgo de captura de la gobernanza.

- **Demasiada descentralización** → Actualizaciones más lentas, pero con mayor seguridad y alineación con la comunidad.

- **Complejidad de los contratos inteligentes** → Los mecanismos de gobernanza excesivamente complejos pueden generar problemas de usabilidad.