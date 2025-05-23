---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Diseño de contratos modulares vs. monolíticos'
weight: 15_000
---

Al diseñar la arquitectura de contratos inteligentes de una DAO, una de las decisiones fundamentales es elegir entre una estructura modular o monolítica. Esta elección afecta la flexibilidad, el mantenimiento, la seguridad y la capacidad de actualización de la DAO.

---

## Entendiendo los dos enfoques

### **Diseño monolítico de contratos**
Una estructura monolítica de contratos integra todas las funcionalidades principales de una DAO en un único contrato inteligente o en un conjunto de contratos estrechamente acoplados.

#### **Beneficios:**
- **Simplicidad**: Más fácil de entender y auditar, ya que toda la lógica se encuentra en un único marco.
- **Menor sobrecarga**: Menos interacciones entre contratos implican menores costos de gas y complejidad.
- **Predictibilidad**: La lógica de gobernanza está codificada, lo que la hace más resistente a interacciones imprevistas.

#### **Desventajas:**
- **Flexibilidad limitada**: Cambiar o actualizar la lógica de gobernanza a menudo requiere reimplementar todo el contrato. 
- **Mayor exposición al riesgo**: Una sola vulnerabilidad en el contrato puede comprometer todo el sistema.
- **Problemas de escalabilidad**: A medida que la DAO crece, una estructura monolítica puede resultar difícil de mantener o ampliar.

---

### **Diseño de contrato modular**
Un enfoque modular divide la lógica de gobernanza en múltiples contratos inteligentes independientes o semi-independientes que interactúan entre sí. Estos módulos pueden incluir contratos centrales, capas de control de acceso, mecanismos de votación, gestión de tesorería y extensiones de gobernanza.

#### **Beneficios:**
- **Flexibilidad**: Los componentes individuales se pueden actualizar o reemplazar sin afectar a todo el sistema.

- **Compartimentación de seguridad**: Es menos probable que los errores o exploits en un módulo comprometan toda la DAO.

- **Personalización**: Diferentes DAOs pueden combinar módulos para adaptarse a sus necesidades de gobernanza.

#### **Desventajas:**
- **Mayor complejidad**: Un mayor número de contratos interactuando implica un mayor riesgo de comportamientos no deseados. 
- **Mayores costos de gas**: Múltiples llamadas a contratos pueden aumentar los costos de ejecución.
- **Riesgos de interdependencia**: Si los módulos dependen demasiado unos de otros, los cambios en uno pueden generar problemas inesperados en otros.

---

## Eligiendo el enfoque adecuado

### Cuándo elegir un diseño monolítico:
- Si la DAO tiene necesidades de gobernanza simples que no requieren cambios frecuentes.
- Si minimizar las tarifas de gas es una prioridad.
- Si la organización prefiere una estructura altamente determinista y fácil de auditar.

### Cuándo elegir un diseño modular:
- Si la DAO prevé que los mecanismos de gobernanza evolucionen con el tiempo.
- Si el aislamiento de seguridad es una prioridad para reducir el riesgo sistémico.
- Si la DAO necesita componibilidad con otros marcos de gobernanza o integraciones externas.

---

## Enfoques híbridos
Muchas DAOs modernas utilizan un enfoque híbrido, donde las funcionalidades centrales permanecen monolíticas para simplificar, mientras que las extensiones de gobernanza y las funciones avanzadas siguen una estructura modular. Algunos ejemplos incluyen:
- Mantener la gestión de votación y tesorería separada para facilitar las actualizaciones.
- Usar contratos proxy para facilitar la actualización, manteniendo un núcleo simple.
- Implementar extensiones de gobernanza que añadan nuevos mecanismos de toma de decisiones sin alterar el contrato central.

---

## Reflexiones finales
La elección entre un diseño de contrato modular y monolítico depende de las necesidades de gobernanza de una DAO, su tolerancia al riesgo y su adaptabilidad a largo plazo. Mientras que las estructuras monolíticas ofrecen simplicidad y menores costos, los diseños modulares brindan flexibilidad y compartimentación de la seguridad. En la práctica, muchas DAOs consideran que un enfoque híbrido funciona mejor, ya que equilibra las fortalezas de ambos modelos.