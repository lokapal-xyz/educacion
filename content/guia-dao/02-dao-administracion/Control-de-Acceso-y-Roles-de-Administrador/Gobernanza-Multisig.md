---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Estructuras de gobernanza multisig'
weight: 30_000
---

Las billeteras multifirma (multisig) desempeñan un papel fundamental en la gobernanza de las DAOs, ya que garantizan que ninguna parte tenga control unilateral sobre acciones críticas. 

---

## **Entendiendo las billeteras multifirma en las DAOs**

Una billetera multifirma requiere varias claves privadas para firmar transacciones antes de su ejecución.

### **Configuraciones comunes de multifirma**
- **M de N firmas**: Un número determinado (M) de firmantes debe aprobar una acción del total (N) asignado (por ejemplo, 3 de 5 firmantes, 6 de 9, 11 de 19). 
- **Umbrales de aprobación**: Algunas DAOs implementan requisitos de firma dinámicos según el tipo de transacción.
- **Aprobaciones con timelocks**: Ciertas transacciones requieren una ejecución retrasada por motivos de seguridad.

### **Herramientas multifirma populares para DAOs**
- **Gnosis Safe**: La solución multifirma on-chain más utilizada.
- **SafeSnap**: Integra Gnosis Safe con Snapshot para la ejecución de votaciones off-chain.
- **Aragon Agent**: Permite DAOs controladas por multifirma dentro del marco de Aragon.

---

## **Beneficios de seguridad y descentralización**

La gobernanza multifirma mitiga los riesgos clave en la toma de decisiones de las DAO:

- **Evita el control unilateral**: Ninguna entidad puede realizar cambios críticos por sí sola.
- **Reduce los puntos únicos de fallo**: Protege contra claves privadas comprometidas.
- **Mejora la transparencia**: Todas las aprobaciones son visibles en la blockchain. 
- **Impulsa la toma de decisiones colectiva** – Garantiza que varios miembros de confianza validen las transacciones.

### **Caso práctico: el incidente de la multifirma de Optimism**
- En 2022, Optimism envió por error 20 millones de dólares en tokens OP a una multifirma incorrecta.
- **Consideraciones de seguridad**: La verificación adecuada del firmante y las simulaciones de transacciones son cruciales.

---

## **Consideraciones de implementación para las DAO**

Las DAOs deben diseñar cuidadosamente sus estructuras de gobernanza multifirma para equilibrar la seguridad, la eficiencia y la descentralización.

### **Factores clave a considerar**
- **¿Quiénes deberían ser firmantes?** – Los miembros de la multifirma deben ser confiables, diversos y responsables.
- **¿Cuál es el umbral óptimo?** – Un umbral demasiado bajo (2 de 5) aumenta el riesgo; un umbral demasiado alto (4 de 5) puede causar retrasos. 
- **¿Debería ser temporal el control multifirma?** – Algunas DAOs utilizan multifirma solo en las etapas iniciales y posteriormente pasan a una gobernanza totalmente descentralizada.
- **¿Cómo gestionar emergencias?** – Se deben implementar mecanismos de recuperación de respaldo y mecanismos de seguridad.

### **Ejemplo: transición a multifirma de Compound**
- Inicialmente protegido por una multifirma, Compound transfirió gradualmente el control de gobernanza a la votación basada en tokens.

---

## **Reflexiones finales**

La gobernanza multifirma mejora la seguridad, la descentralización y la rendición de cuentas dentro de las DAOs. Sin embargo, un diseño deficiente o una mala gestión pueden generar cuellos de botella, ineficiencias y vulnerabilidades.