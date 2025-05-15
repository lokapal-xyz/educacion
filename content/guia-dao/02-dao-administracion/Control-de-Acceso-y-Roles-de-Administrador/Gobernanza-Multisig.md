---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Estructuras de Gobernanza Multisig'
weight: 30_000
---

Las billeteras multifirma (multisig) desempeñan un papel fundamental en la gobernanza de las DAO, ya que garantizan que ninguna parte tenga control unilateral sobre acciones críticas. Esta sección abarca:

- **Cómo funciona la multifirma**: Fundamentos de la configuración de billeteras multifirma.
- **Beneficios de seguridad y descentralización**: Por qué las DAO dependen de la gobernanza multifirma.
- **Consideraciones de implementación**: Factores clave al diseñar un sistema multifirma.

---

## **Entendiendo las billeteras multifirma en las DAO**

Una billetera multifirma requiere varias claves privadas para firmar transacciones antes de su ejecución.

### **Configuraciones comunes de multifirma**
- **M de N firmas**: Un número determinado (M) de firmantes debe aprobar una acción del total (N) asignado (por ejemplo, 3 de 5 firmantes, 6 de 9, 11 de 19). - **Esquemas de Umbral**: Algunas DAO implementan requisitos de firma dinámicos según el tipo de transacción.
- **Aprobaciones con Bloqueo de Tiempo**: Ciertas transacciones requieren una ejecución retrasada por motivos de seguridad.

### **Herramientas Multifirma Populares para DAO**
- **Gnosis Safe**: La solución multifirma en cadena más utilizada.
- **SafeSnap**: Integra Gnosis Safe con Snapshot para la ejecución de votaciones fuera de cadena.
- **Aragon Agent**: Permite DAOs controladas por multifirma dentro del marco de Aragon.

---

## **Beneficios de Seguridad y Descentralización**

La gobernanza multifirma mitiga los riesgos clave en la toma de decisiones de las DAO:

- **Evita el control unilateral**: Ninguna entidad puede realizar cambios críticos por sí sola.
- **Reduce los puntos únicos de fallo**: Protege contra claves privadas comprometidas.
- **Mejora la transparencia**: Todas las aprobaciones son visibles en cadena. **Impulsa la toma de decisiones colectiva** – Garantiza que varios miembros de confianza validen las transacciones.

### **Caso práctico: El incidente de la multifirma Optimism**
- En 2022, Optimism envió por error 20 millones de dólares en tokens OP a una multifirma incorrecta.

**Consideraciones de seguridad**: La verificación adecuada del firmante y las simulaciones de transacciones son cruciales.

---

## **Consideraciones de implementación para las DAO**

Las DAO deben diseñar cuidadosamente sus estructuras de gobernanza multifirma para equilibrar la seguridad, la eficiencia y la descentralización.

### **Factores clave a considerar**
- **¿Quiénes deberían ser firmantes?** – Los miembros de la multifirma deben ser confiables, diversos y responsables.

- **¿Cuál es el umbral óptimo?** – Un umbral demasiado bajo (2 de 5) aumenta el riesgo; un umbral demasiado alto (4 de 5) puede causar retrasos. - **¿Debería ser temporal el control multifirma?** – Algunas DAO utilizan multifirma solo en las etapas iniciales y posteriormente pasan a una gobernanza totalmente descentralizada.

- **¿Cómo gestionar emergencias?** – Se deben implementar mecanismos de recuperación de respaldo y mecanismos de seguridad.

### **Ejemplo: Transición a Multifirma de Compound**
- Inicialmente protegido por una multifirma, Compound transfirió gradualmente el control de gobernanza a la votación basada en tokens.

---

## **Reflexiones finales**

La gobernanza multifirma mejora la seguridad, la descentralización y la rendición de cuentas dentro de las DAO. Sin embargo, un diseño deficiente o una mala gestión pueden generar cuellos de botella, ineficiencias y vulnerabilidades.