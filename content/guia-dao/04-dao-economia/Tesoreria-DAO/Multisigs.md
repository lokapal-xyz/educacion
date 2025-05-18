---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Tesorerías Controladas por Multisigs y Contratos Inteligentes'
weight: 62_000
---

La seguridad de la tesorería es un aspecto fundamental de la gobernanza de las DAO, ya que garantiza la protección de los fondos contra el uso indebido, los ataques informáticos o los riesgos de centralización. Dos de las soluciones de gestión de tesorería más utilizadas en las DAO son:

- **billeteras Multi-Firma (Multi-Sigs)**: Requieren múltiples aprobaciones antes de ejecutar transacciones.
- **Tesorerías Controladas por Contratos Inteligentes**: Automatizan la gestión de fondos según las reglas de gobernanza.

---

## **billeteras Multi-Firma: Un Enfoque Seguro y Colaborativo**

### **¿Qué es un Monedero Multi-Firma?**
Un monedero multi-firma (multi-sig) requiere múltiples aprobaciones antes de ejecutar una transacción. En lugar de que una sola persona controle los fondos, un grupo de firmantes aprueba las transacciones colectivamente.

- **Ejemplo:** Un multi-sig 5/9 significa que, de los 9 firmantes designados, al menos 5 deben aprobar una transacción antes de su ejecución.

### **Ventajas de las multifirmas para las tesorerías de las DAO**
- **Evita el control unilateral**: Ningún firmante puede retirar fondos por sí solo.
- **Mejora la seguridad**: Incluso si una clave se ve comprometida, un atacante no puede vaciar los fondos.
- **Gobernanza descentralizada**: Requiere la colaboración entre múltiples partes interesadas.
- **Seguridad personalizable**: Las DAO pueden ajustar el número de firmantes necesarios para mayor flexibilidad.

### **Desafíos y consideraciones**
- **Retrasos en la coordinación**: Las transacciones requieren múltiples aprobaciones, lo que ralentiza la ejecución.

- **Confianza en los firmantes**: Si la mayoría de los firmantes se confabulan, aún pueden actuar maliciosamente.

- **Riesgos de pérdida de claves**: Si suficientes firmantes pierden el acceso, los fondos podrían quedar bloqueados permanentemente.

- **Estrategia de mitigación:**
- Utilizar un conjunto diverso de firmantes con diferentes perfiles.
- Implementar mecanismos de bloqueo temporal para transacciones de alto valor. - Mantiene procesos de recuperación de emergencia en caso de pérdida de claves.

### **billeteras multifirma populares para DAO**
- **Gnosis Safe**: El monedero multifirma en cadena más utilizado.
- **SafeSnap**: Integra Gnosis Safe con Snapshot para una ejecución controlada por gobernanza.
- **Squads (en Solana)**: Solución multifirma diseñada para DAO basadas en Solana.

---

## **Tesorerías Controladas por Contratos Inteligentes: Automatización de las Finanzas de las DAO**

### **¿Qué es una Tesorería Controlada por Contratos Inteligentes?**
Una tesorería controlada por contratos inteligentes ejecuta transacciones automáticamente según reglas predefinidas, sin intervención humana.

- **Ejemplo:** Una DAO puede crear un contrato de adquisición de derechos que libera fondos a los contribuyentes con el tiempo, evitando el uso indebido.

### **Beneficios de las Tesorerías Controladas por Contratos Inteligentes**
- **Ejecución totalmente sin necesidad de confianza**: Las reglas de gobernanza aplican directamente las políticas de gasto.

- **Distribución programable de fondos**: Automatiza subvenciones, salarios y pagos.

- **Elimina errores humanos y retrasos**: No requiere aprobaciones manuales para transacciones rutinarias.

- **Transparente y auditable**: Cualquiera puede inspeccionar la lógica del contrato inteligente en cadena.

### **Desafíos y riesgos**
- **Vulnerabilidades de los contratos inteligentes**: Los errores o exploits podrían provocar pérdidas irreversibles de fondos.
- **Ejecución rígida**: Una vez implementados, los contratos inteligentes no se adaptan a menos que se actualicen.
- **Comisiones de gas y congestión de la red**: La ejecución en cadena puede resultar costosa durante un uso intensivo de la red.

- **Estrategia de mitigación:**
- Realizar auditorías de seguridad periódicas y recompensas por errores.
- Utilizar contratos inteligentes actualizables (por ejemplo, el patrón proxy de OpenZeppelin) para mayor flexibilidad.
- Implementar mecanismos de seguridad como actualizaciones controladas por multifirma.

### **Ejemplos de sistemas de tesorería con contratos inteligentes**
- **Gobernanza compuesta**: Utiliza contratos inteligentes para automatizar los flujos de fondos de tesorería.
- **Tesorería de Aragon DAO**: Los contratos inteligentes gestionan todas las decisiones relacionadas con la tesorería en cadena. - **Sablier y Superfluid** – Habilita la transmisión de tokens en tiempo real para nóminas y pagos.

---

## **Combinación de billeteras Multi-Firma y Contratos Inteligentes para Máxima Seguridad**

Un enfoque híbrido que aprovecha tanto los billeteras multi-firma como los contratos inteligentes puede ofrecer el mejor equilibrio entre seguridad, flexibilidad y automatización.

| **Enfoque** | **Caso de Uso** | **Ventajas** | **Desventajas** |
|-------------|------------|---------|---------|
| **Solo Multi-Firma** | Gestión manual de tesorería | Alta seguridad, adaptable | Requiere ejecución manual |
| **Solo Contratos Inteligentes** | Tesorería totalmente automatizada | Ejecución sin necesidad de confianza | Menor flexibilidad, posibles riesgos para los contratos inteligentes |
| **Híbrido (Multi-Firma + Contratos Inteligentes)** | Automatización controlada por la gobernanza | Combina seguridad y automatización | Configuración más compleja |

**Ejemplo de modelo híbrido:**
- Usar una billetera multifirma para aprobar actualizaciones de los contratos inteligentes de tesorería.
- Automatizar pagos rutinarios mediante contratos inteligentes (p. ej., salarios de contribuyentes).
- Exigir aprobaciones multifirma para transferencias de alto valor para evitar vulnerabilidades.

---

## **Reflexiones Finales**

La elección del sistema de gestión de tesorería adecuado depende del tamaño de una DAO, su tolerancia al riesgo y su modelo de gobernanza.

- Las DAO pequeñas pueden empezar con billeteras multifirma para simplificar.
- Las DAO más grandes suelen integrar contratos inteligentes para la automatización, manteniendo las protecciones multifirma.
- Un enfoque híbrido puede ofrecer lo mejor de ambos mundos: seguridad y automatización.