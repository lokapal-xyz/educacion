---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Mecanismos de Recuperación de la Gobernanza'
weight: 102_000
---

El sistema de gobernanza de una DAO debe ser lo suficientemente resiliente como para recuperarse de brechas de seguridad, adquisiciones hostiles o propuestas maliciosas. Sin mecanismos de recuperación, un solo ataque podría desestabilizar permanentemente la gobernanza o causar la pérdida de fondos de tesorería.

---

## **¿Por qué es crucial la recuperación de la gobernanza?**

Las vulnerabilidades de gobernanza se pueden explotar de diversas maneras:

- **Propuestas maliciosas** que drenan la tesorería o alteran las reglas de gobernanza.
- **Ataques del 51%** en los que una entidad hostil obtiene el control mayoritario.
- **Claves multifirma robadas** que conducen a acciones no autorizadas.
- **Soborno o manipulación de votos** que distorsiona la toma de decisiones.

Sin mecanismos de recuperación, las DAO pueden tener dificultades para deshacer acciones perjudiciales o restaurar la confianza.

---

## **Revertir propuestas perjudiciales**

Las DAO deben equilibrar la descentralización con la seguridad, garantizando que las propuestas maliciosas se puedan revertir sin permitir una centralización excesiva.

### **Medidas de Protección Preventivas**
- **Retrasos** en acciones críticas de gobernanza (p. ej., 48 horas de retraso en la ejecución).
- **Aprobación en varios pasos** para propuestas de alto impacto.
- **Derecho de veto de la comunidad** para detener propuestas sospechosas antes de su ejecución.

### **Estrategias de Reversión**
- **Mecanismos de Veto de Emergencia**
- Permite a las multifirmas de gobernanza o a un consejo de seguridad pausar o cancelar propuestas maliciosas.
- Ejemplo: GovernorBravo de Compound incluye un rol de "Guardián" que puede vetar cambios perjudiciales.

- **Reversión de Propuestas mediante Votación de Gobernanza**
- Una votación a nivel de la DAO para invalidar una propuesta ejecutada (si se detecta a tiempo).
- Si se implementa esta funcionalidad, debe sopesar el riesgo de que se utilice para revertir propuestas válidas.

- **Bifurcación o Reversión de la Red**
- En casos extremos, las DAO pueden bifurcar el protocolo para crear una nueva versión sin cambios maliciosos. Ejemplo: La bifurcación dura de Ethereum tras el hackeo de TheDAO (2016) restauró los fondos robados.

---

## **Recuperando el control tras un ataque de gobernanza**

Si una DAO pierde el control ante un actor malicioso o una multifirma comprometida, debe contar con mecanismos de escape a nivel de protocolo para recuperar la gobernanza. Las siguientes son algunas estrategias clave de recuperación:

### **Toma de emergencia de multifirma**
- Si la gobernanza se ve comprometida, una multifirma de respaldo puede anular las acciones dañinas.
- Requiere firmantes de seguridad confiables con poderes limitados.

### **Ajustes de quórum y ponderación de votos**
- Reducir el poder de voto de las billeteras sospechosas para prevenir futuros ataques.
- Cambios temporales en el quórum para permitir acciones de recuperación rápidas.
- Algunas DAO permiten una "votación instantánea" de emergencia para ajustar la configuración de gobernanza.

### **Mecanismos de protección de la tesorería**
- Retiros de emergencia controlados por multifirma para transferir fondos a un contrato seguro. - Retiros con bloqueo temporal que permiten acciones de recuperación antes de que se agoten los activos.

---

## **Post-Recuperación: Fortalecimiento de la Gobernanza**

Tras un evento de seguridad, las DAO deben revisar las vulnerabilidades e implementar nuevas protecciones para prevenir futuros incidentes.

- **Mejores Prácticas Post-Recuperación:**
- Realizar un análisis post-mortem para comprender qué falló.
- Fortalecer la seguridad multifirma y revisar los permisos de los titulares de claves.
- Ajustar los marcos de gobernanza para reducir el riesgo de ataques.
- Considerar actualizaciones de protocolo para añadir más capas de seguridad.