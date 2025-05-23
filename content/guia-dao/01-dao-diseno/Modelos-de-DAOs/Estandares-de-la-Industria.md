---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Estándares de la industria'
weight: 20_000
---

A medida que las DAOs han evolucionado, ciertos marcos, plataformas y herramientas se han adoptado ampliamente gracias a su fiabilidad, seguridad y apoyo comunitario. Estos estándares del sector ofrecen soluciones de eficacia comprobada para la gobernanza, la gestión de tesorería y la toma de decisiones, lo que reduce la necesidad de que las DAOs creen sistemas desde cero.

---

## **¿Por qué son importantes los estándares de la industria?**

Usar marcos de DAO consolidados ofrece varias ventajas:

- **Seguridad**: Los contratos auditados y probados en campo reducen el riesgo de vulnerabilidades.
- **Eficiencia**: El uso de soluciones predefinidas acelera la implementación y los procesos de gobernanza de las DAOs.
- **Interoperabilidad**: Muchos marcos estándar se integran bien con herramientas externas y extensiones de gobernanza.
- **Comunidad y soporte**: Los marcos más utilizados cuentan con sólidas comunidades de desarrolladores, lo que facilita la búsqueda de recursos y asistencia.

Sin embargo, basarse en los estándares del sector también implica heredar las desventajas de sus decisiones de diseño, que pueden no adaptarse a las necesidades específicas de cada DAO.

---

## **Selección de marcos y plataformas DAO**

### **Marco MolochDAO**

Las DAOs de estilo Moloch se centran en la simplicidad y la eficiencia del capital, utilizando principalmente "rage quitting" (o mecanismo de salida anticipada) como mecanismo principal. Los miembros aportan a un fondo compartido y pueden salir (rage quit) con su parte proporcional si no están de acuerdo con las decisiones de gobernanza.

- **Fortalezas**: Asignación de capital simple y eficiente, fuerte resistencia a ataques Sybil.
- **Debilidades**: Flexibilidad limitada, falta de funcionalidades de gobernanza modular.
- **Usado por**: MetaCartel, DAOhaus.

### **Compound Governor**

El sistema de gobernanza de Compound se basa en la creación off-chain de propuestas con ejecución on-chain mediante un modelo de votación ponderada por tokens. Se ha convertido en un estándar de gobernanza ampliamente utilizado, que impulsa muchas DAOs que requieren una toma de decisiones on-chain transparente.

- **Fortalezas**: Totalmente on-chain, modular y bien auditado. 
- **Debilidades**: Alta carga de gobernanza, potencial de captura de gobernanza.
- **Usado por**: Compound, Uniswap, Aave, OpenZeppelin Governor.

### **Gnosis Safe y Zodiac**

Gnosis Safe es la billetera multifirma más utilizada en el ecosistema DAO, actuando como una capa de gestión y ejecución de tesorería. Zodiac, un framework de extensión, permite a las DAOs crear mecanismos de gobernanza modulares y componibles sobre Gnosis Safe.

- **Fortalezas**: Alta flexibilidad, seguridad multifirma, expansión modular.
- **Debilidades**: Requiere integraciones externas para una funcionalidad de gobernanza completa.
- **Usado por**: Gnosis DAO, ENS DAO, SafeDAO.

### **Aragon**

Aragon ofrece una suite completa para la creación de DAOs, que les permite implementar estructuras de gobernanza con permisos personalizados, mecanismos de votación y resolución de disputas. Aragon OS y Aragon DAO satisfacen diferentes necesidades de gobernanza, desde DAOs simples hasta organizaciones complejas.

- **Fortalezas**: Configuración de gobernanza "No-code" (sin creación de código), diseño modular, sólido ecosistema de desarrolladores.
- **Debilidades**: Mayor complejidad en comparación con marcos ligeros, dependencia de la infraestructura de Aragon.
- **Usado por**: Decentraland, API3.

### **Tally**

Tally es una interfaz de gobernanza compatible con DAOs basadas en el Gobernador de Compound, que proporciona una interfaz intuitiva para la creación de propuestas, la votación y el seguimiento de la ejecución.

- **Fortalezas**: Mejora la accesibilidad de las DAOs y se integra con los frameworks de gobernanza existentes.
- **Debilidades**: Limitado a DAOs basadas en Compound Governor, depende de capas de ejecución externas.
- **Usado por**: Compound, Gitcoin, Uniswap.

---

## **Elegir el estándar adecuado para su DAO**

El mejor marco depende de las necesidades de la DAO, su estructura de gobernanza y su nivel de descentralización. Algunas consideraciones:

- **Para una gobernanza y gestión de tesorería sencillas** → MolochDAO, Gnosis Safe.
- **Para una gobernanza completamente on-chain** → Compound Governor, Aragon.
- **Para una gobernanza modular e híbrida** → Gnosis Safe + Zodiac, Aragon OS.
- **Para una interfaz de usuario de gobernanza intuitiva** → Tally.

Algunas DAO utilizan una combinación de estas herramientas, combinando una tesorería de Gnosis Safe con la votación de Compound Governor o el sistema de permisos de Aragon con extensiones de gobernanza externas.

---

## **Reflexiones finales**

Los estándares de la industria proporcionan a las DAOs modelos de gobernanza fiables y probados que pueden adoptarse tal cual o personalizarse para adaptarse a necesidades específicas. Si bien estos marcos simplifican la creación y gobernanza de las DAOs, cada uno tiene sus propias compensaciones, y elegir el correcto depende de los objetivos de la DAO, sus necesidades de seguridad y su filosofía de gobernanza.