---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Vulnerabilidades en Contratos Inteligentes'
weight: 95_000
---

Los contratos inteligentes constituyen la columna vertebral de las DAOs, automatizando la gobernanza, la gestión de tesorería y la toma de decisiones. Sin embargo, su naturaleza inmutable y sin permisos los convierte en blancos atractivos para los atacantes.

---

## **Vulnerabilidades Comunes de los Contratos Inteligentes**

- **Ataques de Reentrada**
  - Ocurren cuando un contrato externo llama repetidamente a una función antes de que se complete la ejecución original.
  - Permite a los atacantes drenar fondos antes de que se actualicen los saldos.
  - Prevención: Utilizar el patrón Controles-Efectos-Interacciones, guardias de reentrada y pagos basados ​​en retiros.

---

- ​​**Exploits de Front-Running y MEV**
  - Agentes maliciosos monitorean el mempool y ejecutan transacciones antes que otros.
  - Pueden utilizarse para ataques sándwich, manipulación de arbitraje o ataques de gobernanza.
  - Prevención: Utilizar esquemas de compromiso-revelación, timelocks y relays de transacciones privadas (p. ej., Flashbots Protect).

---

- ​​**Desbordamientos y subdesbordamientos de enteros**
  - Se producen cuando los números superan los valores máximo o mínimo, lo que provoca un comportamiento no deseado.
  - Prevención: Utilice las librerías SafeMath (integradas en Solidity 0.8+).

---

- **Manipulación de Oráculos**
  - Si una DAO depende de un único oráculo de precios, los atacantes pueden manipular los precios para drenar las tesorerías o liquidar posiciones.
  - Prevención: Utilizar oráculos descentralizados (Chainlink, Pyth) y precios TWAP para mitigar la manipulación.

---

- ​​**Ataques de Denegación de Servicio (DoS)**
  - Los atacantes pueden bloquear la ejecución de contratos, enviar spam con propuestas de gobernanza o impedir retiros.
  - Prevención: Utilizar límites de gas, umbrales de propuesta y mecanismos de limitación de tasa.

---

- ​​**Ataques de Préstamos Flash**
  - Implican el préstamo de grandes cantidades de activos sin garantía para manipular los mercados.
  - Permitir a los atacantes explotar las disparidades de precios entre los DEX o manipular la gobernanza.
  - Prevención: Implementar precios promedio ponderados en el tiempo, utilizar múltiples oráculos de precios y añadir retrasos en las transacciones.

---

- ​​**Fallas de Control de Acceso**
  - Ocurren cuando las funciones críticas carecen de las comprobaciones de autorización adecuadas.
  - Permiten que usuarios no autorizados ejecuten operaciones privilegiadas, como retiros de fondos.
  - Prevención: Implementar un control de acceso integral basado en roles, usar modificadores de forma consistente y auditar permisos.

---

- ​​**Errores Lógicos y Gestión Incorrecta del Estado**
  - Resultan de una lógica defectuosa o un seguimiento de estado inadecuado.
  - Provocan que los contratos se comporten de forma diferente a la prevista, a menudo con consecuencias financieras.
  - Prevención: Pruebas exhaustivas, verificación formal y documentación clara de las transiciones de estado.

---

- ​​**Ataques de Repetición de Firmas**
  - Implican la reutilización de firmas válidas para ejecutar transacciones varias veces.
  - Permiten a los atacantes repetir operaciones, como retiros o aprobaciones.
  - Prevención: Incluir nonces, marcas de tiempo o identificadores únicos en las firmas y mantener el seguimiento de las firmas utilizadas.

---

- ​​**Problemas de límite de gas en bloque**
  - Se producen cuando las funciones usan bucles con iteraciones ilimitadas.
  - Pueden imposibilitar la ejecución de funciones cuando los arrays crecen demasiado.
  - Prevención: Implementar paginación, evitar bucles ilimitados y diseñar para la eficiencia del gas.

---

- ​​**Llamadas externas sin control**
  - Fallos en llamadas de contratos externos que no se validan correctamente.
  - Pueden provocar estados inesperados cuando las llamadas fallan silenciosamente.
  - Prevención: Verificar los valores de retorno, usar patrones try/catch e implementar una gestión de fallos adecuada.

---

- ​​**Colisión de almacenamiento**
  - Se produce en patrones de proxy cuando los slots de almacenamiento se sobrescriben accidentalmente.
  - Provoca corrupción de datos y un comportamiento impredecible.
  - Prevención: Usar patrones de almacenamiento estandarizados, una planificación cuidadosa de las actualizaciones y variables de brecha de almacenamiento.

---

- ​​**Vulnerabilidades de puente entre cadenas**
  - Fallos de seguridad en los protocolos de comunicación entre cadenas. 
  - Permitir el robo de fondos bloqueados o la acuñación no autorizada de tokens encapsulados.
  - Prevención: Validación multifirma, mecanismos de consenso robustos y limitación de tasa.

---

- ​​**Dependencia de la marca de tiempo**
  - Ocurre cuando los contratos dependen de las marcas de tiempo de los bloques para operaciones críticas.
  - Los mineros pueden manipular las marcas de tiempo por varios segundos, lo que afecta la lógica sensible al tiempo.
  - Prevención: Evitar dependencias precisas de las marcas de tiempo, usar números de bloque para la temporización e implementar periodos de búfer.

---

- ​​**Aleatoriedad insegura**
  - Resulta del uso de fuentes de datos predecibles en la cadena para generar números aleatorios.
  - Permite a los mineros u observadores predecir o manipular resultados aleatorios.
  - Prevención: Usar esquemas de compromiso-revelación, funciones aleatorias verificables (VRF) o aleatoriedad proporcionada por el oráculo.

---

- ​​**Falta de validación de entrada**
  - Ocurre cuando los contratos no validan correctamente las entradas externas. 
  - Permite la manipulación mediante valores inesperados, lo que provoca fallos lógicos o desbordamientos.
  - Prevención: Implementar comprobaciones exhaustivas de límites, validar todas las entradas con los rangos esperados y utilizar sentencias "require".

---

## **Reflexiones Finales**

Las DAOs deben proteger proactivamente los contratos inteligentes para evitar fallos catastróficos. La reentrada, el front-running, los problemas de control de acceso y las vulnerabilidades de oráculos siguen siendo amenazas clave. Mediante prácticas de codificación segura, la implementación de auditorías y el uso de la verificación formal, las DAOs pueden minimizar las vulnerabilidades y mantener la confianza en sus sistemas de gobernanza.