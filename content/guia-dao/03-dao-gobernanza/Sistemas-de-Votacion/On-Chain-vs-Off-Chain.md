---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Votación On-Chain vs Off-Chain'
weight: 46_000
---

La votación es un mecanismo fundamental de gobernanza para las DAO, que determina todo, desde las actualizaciones de protocolo hasta la gestión de la tesorería. Sin embargo, las DAO deben elegir entre la votación en cadena y fuera de ella, cada una con sus propias desventajas en términos de seguridad, transparencia, costo y escalabilidad.

---

## **¿Qué es la votación en cadena?**

### **Cómo funciona**
- Los votos se registran directamente en la blockchain como transacciones.
- Requiere que los participantes firmen las transacciones con su billetera.
- El contrato inteligente ejecuta automáticamente el resultado una vez finalizada la votación.

### **Ventajas**
- A prueba de manipulaciones: los resultados se almacenan permanentemente en la blockchain, lo que garantiza la transparencia.
- Ejecución sin confianza: los contratos inteligentes ejecutan las decisiones sin intermediarios.
- Registro inmutable: evita disputas sobre el historial de votaciones o la manipulación.

### **Desventajas**
- Costoso: cada voto requiere una transacción en la blockchain, lo que genera comisiones de gas. - Lenta: La votación depende de la congestión de la red y los tiempos de bloque.

- Menor participación: Los usuarios pueden evitar votar debido a costos y barreras técnicas.

### **Mejores casos de uso**
- Decisiones críticas de gobernanza (p. ej., asignación de tesorería, actualizaciones de protocolo).

- Cuando la transparencia y la seguridad superan las preocupaciones por el costo.

- DAOs maduras con participantes activos con inversión financiera.

- ---

## **¿Qué es la votación fuera de la cadena?**

### **Cómo funciona**
- Las votaciones no se registran en la cadena de bloques, sino que se realizan a través de plataformas externas (p. ej., Snapshot, encuestas de Discord, Formularios de Google).

- Los participantes pueden firmar los mensajes criptográficamente, pero las votaciones no requieren comisiones de gas.

- Un mecanismo de ejecución independiente (a menudo multifirmas) aplica los resultados.

### **Ventajas**
- Votación sin gas: Fomenta una mayor participación.

- Más rápida: No es necesario esperar la confirmación de la cadena de bloques. - Flexible: Permite estructuras de votación complejas sin las limitaciones de los contratos inteligentes.

### **Desventajas**
- No es confiable: Los resultados dependen de plataformas externas o facilitadores de gobernanza.

- Potencial de manipulación: Sin la aplicación en cadena, los votos podrían ignorarse o manipularse.

- Menor transparencia: La integridad de los datos depende del proveedor de servicios fuera de la cadena.

### **Mejores casos de uso**
- DAO que priorizan la inclusión y la participación.

- DAO en fase inicial que prueban modelos de gobernanza.

- Votos de señalización no vinculantes (por ejemplo, para evaluar la opinión de la comunidad).

---

## **Comparación de la votación en cadena y fuera de cadena**

| **Característica** | **Votación en cadena** | **Votación fuera de cadena** |
|--------------------|--------------------|--------------------|
| **Seguridad** | Alta (ejecución inmutable y confiable) | Media (depende de la integridad de la plataforma) |
| **Transparencia** | Completa (resultados visibles en la blockchain) | Parcial (depende de verificación externa) |
| **Costo** | Caro (comisiones de gas por cada voto) | Gratuito o mínimo (sin costes de gas) |
| **Velocidad** | Más lento (tiempo de confirmación en la blockchain) | Más rápido (sin retrasos en las transacciones) |
| **Escalabilidad** | Limitado (costo de gas elevado para votaciones numerosas) | Alto (admite amplia participación) |
| **Flexibilidad** | Bajo (las reglas deben estar predefinidas) | Alto (fácil de ajustar) |

Ambos tipos de votación tienen sus ventajas y desventajas. Muchas DAO los combinan para equilibrar la seguridad y la participación. ---

## **Enfoques Híbridos: Combinando Votación On-Chain y Off-Chain**

Dado que ningún sistema es perfecto, muchas DAO utilizan modelos de gobernanza híbridos:

### **Ejemplos de Enfoques**
- **Señalización Off-Chain → Ejecución On-Chain**
- Paso 1: Los miembros de la DAO votan off-chain (p. ej., Snapshot).
- Paso 2: Si una propuesta se aprueba, una multifirma o consejo la ejecuta on-chain.
- Ejemplo: MakerDAO, Gobernanza de Gitcoin.

- **Modelos Híbridos Basados ​​en Umbrales**
- Las decisiones pequeñas (p. ej., subvenciones menores) se toman off-chain para mayor rapidez.
- Las decisiones importantes (p. ej., retiros de tesorería) requieren ejecución on-chain.
- Ejemplo: Optimism DAO, Gobernanza de ENS.

**Delegación de Votos**

- Los participantes votan fuera de la cadena, pero delegan la ejecución final a actores confiables dentro de la cadena.

- Reduce los costos dentro de la cadena, manteniendo cierto grado de cumplimiento sin necesidad de confianza.

---

## **Cómo Elegir el Enfoque Adecuado para tu DAO**

- Si la seguridad es la prioridad, utiliza el voto dentro de la cadena para decisiones clave.

- Si la participación es más importante, utiliza el voto fuera de la cadena para fomentar la interacción.

- Si buscas un equilibrio entre ambos, considera un modelo híbrido donde los votos fuera de la cadena guíen la ejecución dentro de la cadena.