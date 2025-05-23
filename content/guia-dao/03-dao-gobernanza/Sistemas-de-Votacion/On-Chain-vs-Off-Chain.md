---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Votación on-chain vs off-chain'
weight: 46_000
---

La votación es un mecanismo fundamental de gobernanza DAO que determina mucho, desde las actualizaciones de protocolo hasta la gestión de la tesorería. Sin embargo, las DAOs deben elegir entre la votación on-chain y off-chain; cada una con sus propias desventajas en términos de seguridad, transparencia, costo y escalabilidad.

---

## **¿Qué es la votación on-chain?**

### **Cómo funciona**
- Los votos se registran directamente en la blockchain como transacciones.
- Requiere que los participantes firmen las transacciones con su billetera.
- El contrato inteligente ejecuta automáticamente el resultado una vez finalizada la votación.

### **Ventajas**
- A prueba de manipulaciones: los resultados se almacenan permanentemente en la blockchain, lo que garantiza la transparencia.
- Ejecución sin requisitos de confianza: los contratos inteligentes ejecutan las decisiones sin intermediarios.
- Registro inmutable: evita disputas sobre el historial de votaciones o la manipulación.

### **Desventajas**
- Costoso: cada voto requiere una transacción en la blockchain, lo que genera tarifas de gas. 
- Lenta: La votación depende de la congestión de la red y los tiempos de bloque.
- Menor participación: Los usuarios pueden evitar votar debido a costos y barreras técnicas.

### **Mejores casos de uso**
- Decisiones críticas de gobernanza (p. ej., asignación de tesorería, actualizaciones de protocolo).
- Cuando la transparencia y la seguridad superan las preocupaciones por el costo.
- DAOs maduras con participantes activos con inversión financiera.

---

## **¿Qué es la votación off-chain?**

### **Cómo funciona**
- Las votaciones no se registran en la blockchain, sino que se realizan a través de plataformas externas (p. ej., Snapshot, encuestas de Discord, Formularios de Google).
- Los participantes pueden firmar los mensajes criptográficamente, pero las votaciones no requieren tarifas de gas.
- Un mecanismo de ejecución independiente (a menudo multifirmas) aplica los resultados.

### **Ventajas**
- Votación sin gas: Fomenta una mayor participación.
- Más rápida: No es necesario esperar la confirmación de la cadena de bloques. 
- Flexible: Permite estructuras de votación complejas sin las limitaciones de los contratos inteligentes.

### **Desventajas**
- Necesita confianza: Los resultados dependen de plataformas externas o facilitadores de gobernanza.
- Potencial de manipulación: Sin la aplicación on-chain, los votos podrían ignorarse o manipularse.
- Menor transparencia: La integridad de los datos depende del proveedor de servicios off-chain.

### **Mejores casos de uso**
- DAOs que priorizan la inclusión y la participación.
- DAOs en fase inicial que prueban modelos de gobernanza.
- Votos de señalización no vinculantes (por ejemplo, para evaluar la opinión de la comunidad).

---

## **Comparación de la votación on-chain y off-chain**

| **Característica** | **Votación on-chain** | **Votación off-chain** |
|--------------------|--------------------|--------------------|
| **Seguridad** | Alta (ejecución inmutable y confiable) | Media (depende de la integridad de la plataforma) |
| **Transparencia** | Completa (resultados visibles en la blockchain) | Parcial (depende de verificación externa) |
| **Costo** | Caro (tarifas de gas por cada voto) | Gratuito o mínimo (sin costos de gas) |
| **Velocidad** | Más lento (tiempo de confirmación en la blockchain) | Más rápido (sin retrasos en las transacciones) |
| **Escalabilidad** | Limitado (costo de gas elevado para votaciones numerosas) | Alto (admite amplia participación) |
| **Flexibilidad** | Bajo (las reglas deben estar predefinidas) | Alto (fácil de ajustar) |

Ambos tipos de votación tienen sus ventajas y desventajas. Muchas DAOs los combinan para equilibrar la seguridad y la participación. ---

## **Enfoques híbridos: combinando votación on-chain y off-chain**

Dado que ningún sistema es perfecto, muchas DAOs utilizan modelos de gobernanza híbridos:

### **Ejemplos de enfoques**
- **Señalización off-chain → ejecución on-chain**
  - Paso 1: Los miembros de la DAO votan off-chain (p. ej., Snapshot).
  - Paso 2: Si una propuesta se aprueba, una multifirma o consejo la ejecuta on-chain.
  - Ejemplo: MakerDAO, Gobernanza de Gitcoin.

- **Modelos híbridos basados ​​en umbrales**
  - Las decisiones pequeñas (p. ej., subvenciones menores) se toman off-chain para mayor rapidez.
  - Las decisiones importantes (p. ej., retiros de tesorería) requieren ejecución on-chain.
  - Ejemplo: Optimism DAO, Gobernanza de ENS.

**Delegación de votos**
  - Los participantes votan off-chain, pero delegan la ejecución final a actores on-chain confiables.
  - Reduce los costos, manteniendo cierto grado de cumplimiento sin requisitos de confianza.

---

## **Cómo elegir el enfoque adecuado para su DAO**

- Si la seguridad es la prioridad, utiliza el voto on-chain para decisiones clave.
- Si la participación es más importante, utiliza el voto off-chain para fomentar la interacción.
- Si buscas un equilibrio entre ambos, considera un modelo híbrido donde los votos off-chain guíen la ejecución on-chain.