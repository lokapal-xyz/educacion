---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Quorums, Umbrales de Votación y Mecanismos de Ejecución'
weight: 50_000
---

Para garantizar que las decisiones de gobernanza reflejen la voluntad de la comunidad, se requieren quórums y umbrales de votación bien definidos. Estos parámetros determinan cuántos participantes deben participar y qué nivel de apoyo se necesita para que una propuesta se apruebe.

---

## **Requisitos de quórum**

### **¿Qué es un quórum?**
El quórum es el nivel mínimo de participación requerido para que una votación se considere válida. Sin quórum, un pequeño grupo de votantes podría aprobar propuestas sin una participación más amplia de la comunidad.

### **Tipos de quórums en las DAO**

- **Quórum absoluto**: un número mínimo fijo de votos (p. ej., se necesitan 1000 votos independientemente de la participación total de los votantes).
- **Quórum relativo**: un porcentaje del suministro total de tokens o del poder de gobernanza (p. ej., debe participar el 10 % de los tokens en circulación). - **Cuórum Dinámico** – Se ajusta en función de factores como la participación electoral o el tipo de propuesta, reduciendo los requisitos de cuórum cuando la participación es baja.

### **Equilibrio de los Niveles de Cuórum**

- **Demasiado Alto →** La baja participación puede provocar un estancamiento en la gobernanza.
- **Demasiado Bajo →** Los grupos pequeños de votantes podrían manipular las decisiones.

- **Solución →** Los modelos de cuórum dinámicos o escalonados garantizan la participación y mantienen la seguridad.

---

## **Umbrales de Votación**

### **¿Qué es un Umbral de Votación?**
Un umbral de votación es el porcentaje de votos necesario para que una propuesta se apruebe. Evita la regla de la minoría y garantiza que las decisiones reflejen el apoyo de la mayoría.

### **Modelos Comunes de Umbrales de Votación**

- **Mayoría Simple (50%+1)** – El método más común, donde una propuesta se aprueba si obtiene más de la mitad de los votos. - **Supermayoría (p. ej., 60%-75%)**: Se utiliza para propuestas de alto impacto (p. ej., actualizaciones de protocolo, gasto de tesorería).

- **Mayoría relativa**: La opción con más votos gana, incluso si es inferior al 50% (común en la votación multiopción).

- **Votación cuadrática o ponderada**: Ajusta el poder de voto en función de la participación para evitar el dominio de las grandes partes interesadas.

### **Elegir el umbral adecuado**

- **Los umbrales más bajos (p. ej., 50%)** fomentan la participación, pero corren el riesgo de que decisiones controvertidas se aprueben con demasiada facilidad.

- **Los umbrales más altos (p. ej., 66%)** garantizan el consenso, pero pueden causar bloqueos en la gobernanza.

- Los **modelos escalonados** permiten diferentes umbrales para distintos tipos de propuestas (p. ej., más bajos para iniciativas comunitarias, más altos para cambios constitucionales).

---

## **Mecánica de Ejecución de Propuestas**

Una vez aprobada una propuesta, debe ejecutarse de forma eficiente y segura. La ejecución puede ser:

### **Ejecución Manual (Fuera de la Cadena)**
- Una entidad de confianza (por ejemplo, una billetera multifirma o un consejo de gobernanza) ejecuta los cambios aprobados.

- Riesgos: Requiere confianza en los ejecutores; posibilidad de retrasos o censura.

### **Ejecución Automatizada (En la Cadena)**
- Los contratos inteligentes ejecutan la propuesta una vez que se cumplen las condiciones.

- Ejemplo: Una propuesta aprobada activa automáticamente una transferencia de tesorería.

- Beneficios: Reduce la dependencia de la intervención humana; mejora la transparencia.

### **Ejecución Híbrida**
- Una combinación de ejecución dentro y fuera de la cadena, donde algunas decisiones (p. ej., la aprobación de financiación) se toman dentro de la cadena, mientras que otras (p. ej., el cumplimiento legal) requieren acciones fuera de la cadena.

---

## **Reflexiones finales**

- Un buen diseño de quórums previene la manipulación de la gobernanza y fomenta la participación.
- Unos umbrales de votación adecuados equilibran la eficiencia con la legitimidad de las decisiones.
- La mecánica de ejecución determina la fluidez con la que se implementan las decisiones de gobernanza.

Establecer parámetros de gobernanza flexibles y bien calibrados garantiza que las DAO se mantengan eficientes, resilientes y basadas en la comunidad.