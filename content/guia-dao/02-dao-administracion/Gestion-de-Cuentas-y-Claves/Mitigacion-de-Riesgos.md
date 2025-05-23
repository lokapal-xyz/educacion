---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Mitigación de riesgos por compromiso de claves'
weight: 35_000
---

Una clave comprometida puede poner en riesgo los fondos, la gobernanza y las operaciones de una DAO. Exploremos estrategias para minimizar, detectar y recuperarse de incidentes de seguridad relacionados con claves.

---

## **Detección temprana de vulnerabilidades de clave**

### **Mejores prácticas**
- Habilitar el monitoreo en tiempo real para detectar cualquier actividad inusual.
- Configurar alertas para transacciones grandes o inesperadas.
- Utilizar mecanismos de protección (por ejemplo, retrasos en las transacciones o límites de retiro).
- Realizar auditorías de seguridad periódicas de las prácticas de gestión de claves.

### **Errores comunes que se deben evitar**
- Ignorar pequeñas transacciones no autorizadas (posibles ataques de prueba).
- Falta de herramientas de análisis o monitoreo on-chain.
- No revisar los registros de acceso y los patrones de actividad.

---

## **Estrategias de recuperación ante vulnerabilidades de clave**

### **Mejores prácticas**
- Implementar multifirmas de emergencia para anular las claves comprometidas. 
- Utilizar transacciones con timelock para permitir la reversión en caso de ataque.
- Almacenar las claves de respaldo de forma segura y separadas de las claves principales.
- Utilizar mecanismos de recuperación social para la restauración de claves.

### **Errores comunes que se deben evitar**
- Falta de un plan de contingencia para claves perdidas o robadas.
- Depender de un único método de recuperación (p. ej., un único titular de la clave de respaldo).
- Tiempo de respuesta lento tras detectar una vulnerabilidad.

---

## **Minimizar el impacto de una clave comprometida**

### **Mejores prácticas**
- Implementar niveles de acceso escalonados (limitar el uso de claves con altos privilegios).
- Utilizar claves que caduquen tras un periodo determinado.
- Establecer una gobernanza modular para aislar los riesgos (p. ej., SubDAOs con control independiente).
- Habilitar interruptores automáticos de seguridad para revocar los permisos comprometidos.

### **Errores comunes que se deben evitar**
- Otorgar todos los permisos a una única clave o entidad. 
- No revocar el acceso rápidamente tras una vulneración.
- Utilizar un sistema de gobernanza rígido que carece de flexibilidad para responder ante emergencias.

---

## **Reflexiones finales**
- **Prevenir** la vulneración de claves con almacenamiento seguro y control de acceso (véase el artículo anterior).
- **Detectar** problemas a tiempo mediante monitoreo y alertas.
- **Recuperarse** rápidamente con copias de seguridad multifirma y procedimientos de emergencia.
- **Minimizar** el impacto mediante acceso por niveles y desconexión automática.