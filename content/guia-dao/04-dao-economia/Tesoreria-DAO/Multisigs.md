---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Tesorerías multisig y controladas por contratos inteligentes'
weight: 62_000
---

La seguridad de la tesorería es un aspecto fundamental de la gobernanza de las DAOs, ya que garantiza la protección de los fondos contra el uso indebido, los ataques informáticos o los riesgos de centralización. Dos de las soluciones de gestión de tesorería más utilizadas en las DAOs son:

- **Billeteras multifirma (multisigs)**: Requieren múltiples aprobaciones antes de ejecutar transacciones.
- **Tesorerías controladas por contratos inteligentes**: Automatizan la gestión de fondos según las reglas de gobernanza.

---

## **Billeteras multisig: un enfoque seguro y colaborativo**

### **¿Qué es una billetera multisig?**
Una multisig requiere múltiples aprobaciones antes de ejecutar una transacción. En lugar de que una sola persona controle los fondos, un grupo de firmantes aprueba las transacciones colectivamente.

- **Ejemplo:** Un multi-sig 5/9 significa que, de los 9 firmantes designados, al menos 5 deben aprobar una transacción antes de su ejecución.

### **Ventajas de las multifirmas para las tesorerías de las DAO**
- **Evita el control unilateral**: Ningún firmante puede retirar fondos por sí solo.
- **Mejora la seguridad**: Incluso si una clave se ve comprometida, un atacante no puede vaciar los fondos.
- **Gobernanza descentralizada**: Requiere la colaboración entre múltiples partes interesadas.
- **Seguridad personalizable**: Las DAOs pueden ajustar el número de firmantes necesarios para mayor flexibilidad.

### **Desafíos y consideraciones**
- **Retrasos en la coordinación**: Las transacciones requieren múltiples aprobaciones, lo que ralentiza la ejecución.
- **Confianza en los firmantes**: Si la mayoría de los firmantes se confabulan, aún pueden actuar maliciosamente.
- **Riesgos de pérdida de claves**: Si suficientes firmantes pierden el acceso, los fondos podrían quedar bloqueados permanentemente.

- **Estrategia de mitigación:**
  - Utilizar un conjunto diverso de firmantes con diferentes perfiles.
  - Implementar mecanismos de timelock para transacciones de alto valor. 
  - Mantener procesos de recuperación de emergencia en caso de pérdida de claves.

### **Billeteras multifirma populares para las DAOs**
- **Gnosis Safe**: La billetera multifirma en cadena más utilizado.
- **SafeSnap**: Integra Gnosis Safe con Snapshot para una ejecución controlada por gobernanza.
- **Squads (en Solana)**: Solución multifirma diseñada para DAOs basadas en Solana.

---

## **Tesorerías controladas por contratos inteligentes: automatización de las finanzas de las DAOs**

### **¿Qué es una tesorería controlada por contratos inteligentes?**
Una tesorería controlada por contratos inteligentes ejecuta transacciones automáticamente según reglas predefinidas, sin intervención humana.

- **Ejemplo:** Una DAO puede crear un contrato de adquisición de derechos que libera fondos a los contribuyentes con el tiempo, evitando el uso indebido.

### **Beneficios de las tesorerías controladas por contratos inteligentes**
- **Ejecución totalmente sin requisitos de confianza**: Las reglas de gobernanza aplican directamente las políticas de gasto.
- **Distribución programable de fondos**: Automatiza subvenciones, salarios y pagos.
- **Elimina errores humanos y retrasos**: No requiere aprobaciones manuales para transacciones rutinarias.
- **Transparente y auditable**: Cualquiera puede inspeccionar la lógica del contrato inteligente en la blockchain.

### **Desafíos y riesgos**
- **Vulnerabilidades de los contratos inteligentes**: Los errores o exploits podrían provocar pérdidas irreversibles de fondos.
- **Ejecución rígida**: Una vez implementados, los contratos inteligentes no se adaptan a menos que se actualicen.
- **Tarifas de gas y congestión de la red**: La ejecución on-chain puede resultar costosa durante un uso intensivo de la red.

- **Estrategia de mitigación:**
  - Realizar auditorías de seguridad periódicas y recompensas por errores.
  - Utilizar contratos inteligentes actualizables (por ejemplo, el patrón proxy de OpenZeppelin) para mayor flexibilidad.
  - Implementar mecanismos de seguridad como actualizaciones controladas por multifirma.

### **Ejemplos de sistemas de tesorería con contratos inteligentes**
- **Compound Governance**: Utiliza contratos inteligentes para automatizar los flujos de fondos de tesorería.
- **Tesorería de Aragon DAO**: Los contratos inteligentes gestionan todas las decisiones relacionadas con la tesorería on-chain. 
- **Sablier y Superfluid** – Habilita la transmisión de tokens en tiempo real para nóminas y pagos.

---

## **Combinación de billeteras multisig y contratos inteligentes para máxima seguridad**

Un enfoque híbrido que aprovecha tanto los billeteras multi-firma como los contratos inteligentes puede ofrecer el mejor equilibrio entre seguridad, flexibilidad y automatización.

| **Enfoque** | **Caso de uso** | **Ventajas** | **Desventajas** |
|-------------|------------|---------|---------|
| **Solo multisig** | Gestión manual de tesorería | Alta seguridad, adaptable | Requiere ejecución manual |
| **Solo contratos inteligentes** | Tesorería totalmente automatizada | Ejecución sin requisitos de confianza | Menor flexibilidad, posibles riesgos para los contratos inteligentes |
| **Híbrido (multisig + contratos inteligentes)** | Automatización controlada por la gobernanza | Combina seguridad y automatización | Configuración más compleja |

- **Ejemplo de modelo híbrido:**
  - Usar una billetera multifirma para aprobar actualizaciones de los contratos inteligentes de tesorería.
  - Automatizar pagos rutinarios mediante contratos inteligentes (p. ej., salarios de contribuyentes).
  - Exigir aprobaciones multifirma para transferencias de alto valor para evitar vulnerabilidades.

---

## **Reflexiones finales**

La elección del sistema de gestión de tesorería adecuado depende del tamaño de una DAO, su tolerancia al riesgo y su modelo de gobernanza.

- Las DAOs pequeñas pueden empezar con billeteras multifirma para simplificar.
- Las DAOs más grandes suelen integrar contratos inteligentes para la automatización, manteniendo las protecciones multifirma.
- Un enfoque híbrido puede ofrecer lo mejor de ambos mundos: seguridad y automatización.