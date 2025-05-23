---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Tipos de mecanismos de votación'
weight: 45_000
---

La votación es la base de la gobernanza descentralizada, ya que permite a las partes interesadas influir en las decisiones, asignar recursos y moldear el futuro de una DAO. Sin embargo, los diferentes mecanismos de votación presentan distintos niveles de imparcialidad, seguridad y resistencia a la manipulación.

---

## **Votación basada en tokens**

### **Cómo funciona**
- Cada token representa un voto (1 token = 1 voto).
- Cuantos más tokens posea un participante, mayor será su poder de voto.
- Se utiliza en la mayoría de las DAOs debido a su simplicidad y su alineación directa con la propiedad de tokens.

### **Ventajas**
- Simple y ampliamente adoptado: fácil de implementar mediante tokens de gobernanza ERC-20.
- Incentivos alineados: los poseedores de tokens tienen participación en el éxito de la DAO.
- Eficiente para decisiones de alto riesgo: la votación ponderada refleja el compromiso financiero.

### **Desventajas**
- Riesgo plutocrático: los grandes poseedores (ballenas) pueden dominar las decisiones. 
- Baja participación electoral: los titulares pueden no participar en la gobernanza.
- Vulnerabilidad a la compra de votos: los tokens se pueden tomar prestados o delegar para influir.

### **Mejores casos de uso**
- Gobernanza de protocolos (p. ej., Uniswap, Compound).
- DAOs donde la propiedad de tokens se alinea estrechamente con los incentivos para la toma de decisiones.

---

## **Voto cuadrático**

### **Cómo funciona**
- Los votos no son lineales: el costo de emitir varios votos aumenta cuadráticamente.
- Evita que una sola entidad domine las decisiones con grandes tenencias. 
- **Ejemplo de costo de votos:**
  - 1 voto cuesta 1 token
  - 2 votos cuestan 4 tokens (2²)
  - 3 votos cuestan 9 tokens (3²)
  - 4 votos cuestan 16 tokens (4²)
  - Y así sucesivamente...

### **Ventajas**
- Equilibra la influencia: los grandes tenedores conservan poder, pero con rendimientos decrecientes.
- Fomenta la participación diversa: los pequeños accionistas tienen una voz significativa.
- Resultados más democráticos: ayuda a prevenir el dominio de las ballenas.

### **Desventajas**
- Requiere verificación de identidad: sin la resistencia de Sybil, se puede manipular.
- Implementación compleja: requiere contratos inteligentes e infraestructura adicionales.
- Podría no funcionar bien para todas las DAOs: si los contribuyentes tienen diferentes niveles de experiencia, igualar el poder de voto puede ser contraproducente.

### **Mejores casos de uso**
- DAO centradas en la gobernanza comunitaria.
- Asignación de fondos (p. ej., subvenciones de Gitcoin).
- Financiación de bienes públicos donde se necesita una representación más justa.

---

## **Voto por convicción**

### **Cómo funciona**
- El poder de voto se acumula con el tiempo según el tiempo que un participante apoya una propuesta.
- Fomenta el compromiso a largo plazo en lugar de picos repentinos de votación.
- **Ejemplo de fórmula de convicción:**
  - Convicción = Convicción Previa × Factor de Decaimiento + Nueva Participación

### **Ventajas**
- Disuade la manipulación a corto plazo. Evita los votos de ballena de última hora.
- Gobernanza continua. Los miembros pueden expresar sus preferencias dinámicamente.
- Resistente a la compra de votos. Requiere compromiso a largo plazo, lo que reduce la influencia repentina.

### **Desventajas**
- Toma de decisiones lenta. Requiere tiempo para que los votos acumulen influencia.
- Los nuevos participantes tienen menos poder inmediato. Puede perjudicar a los recién llegados.
- Podría no ser ideal para decisiones urgentes. Algunas DAOs necesitan ciclos de gobernanza más rápidos.

### **Mejores casos de uso**
- Decisiones de asignación de fondos. 
- DAOs impulsadas por la comunidad con incentivos a largo plazo.
- Ecosistemas que requieren la formación gradual de consenso (p. ej., Commons Stack).

---

## **Consenso holográfico**

### **Cómo funciona**
- Se utiliza un mecanismo de mercado predictivo junto con la votación tradicional.
- Los participantes apuestan tokens para indicar qué propuestas merecen atención.
- Si una propuesta supera un umbral de atención, se acelera su votación completa en la DAO.
- Al igual que un holograma recrea una representación 3D a partir de un medio 2D, este mecanismo de votación intenta proyectar la voluntad de toda la DAO a través de las acciones de un grupo más pequeño.

### **Ventajas**
- Gobernanza escalable: prioriza las propuestas importantes sin abrumar a los votantes.
- Filtra las propuestas de baja calidad: evita el spam o los elementos de gobernanza sin importancia.
- Toma de decisiones eficiente: solo las decisiones de alto impacto llegan a la votación completa de la DAO.

### **Desventajas**
- Requiere participación en staking: una baja participación puede reducir la eficiencia.
- Puede ser complejo de entender: requiere la formación de los participantes de la DAO.
- Depende de buenos incentivos económicos: un diseño deficiente de los incentivos puede llevar a la manipulación.

### **Mejores casos de uso**
- Grandes DAOs que requieren una gobernanza escalable (p. ej., DAOstack).
- DAOs donde no todas las propuestas deben someterse a votación.
- Proyectos que utilizan modelos de gobernanza basados ​​en predicciones.

---

## **Voto delegado (democracia líquida)**

### **Cómo funciona**
- Los participantes delegan su poder de voto a representantes de confianza.
- Los delegados pueden votar directamente o delegar la delegación.
- Los poseedores de tokens pueden revocar o cambiar la delegación en cualquier momento.

### **Ventajas**
- Fomenta una gobernanza basada en la experiencia: los delegados suelen estar mejor informados.
- Flexible: los participantes pueden votar directamente o delegar selectivamente.
- Mejora la participación: una forma sencilla de participación para los miembros pasivos.

### **Desventajas**
- Riesgo de centralización: la delegación podría dar lugar a oligarquías en la gobernanza.
- Posible desalineación: los delegados podrían no siempre representar los intereses de los votantes.
- Requiere confianza en los delegados: la gobernanza podría depender demasiado de unas pocas figuras clave.

### **Mejores casos de uso**
- DAOs con grandes bases de tenedores pasivos de tokens (p. ej., Compound, Aave).
- Sistemas de gobernanza complejos que requieren supervisión experta.
- Modelos híbridos que combinan votación directa y delegada.

---

## **Voto por orden de preferencia**

### **Cómo funciona**
- Los votantes clasifican múltiples opciones por orden de preferencia.
- Si ninguna opción obtiene la mayoría, se elimina la opción con menor puntuación y los votos se redistribuyen hasta que surge un ganador.

- **Ejemplo de voto por orden de preferencia**

| **Opción candidata** | **Ronda 1** | **Ronda 2** | **Ronda 3** | **Ronda 4** |
|------------|------------|---------|---------|---------|
| Estrategia de rendimiento DeFi | 28% | 30% | 38% | **52%** |
| Inversión en proyectos NFT | 15% | 15% | ~~X~~ | ~~X~~ |
| Mejora del Protocolo | 22% | 24% | 28% | ~~X~~ |
| Subvenciones Comunitarias | 25% | 31% | 34% | 48% |
| Reserva DAO | 10% | ~~X~~ | ~~X~~ | ~~X~~ |

### **Ventajas**
- Fomenta la toma de decisiones por consenso.
- Reduce la polarización: se considera una gama más amplia de opiniones.
- Útil para seleccionar candidatos o propuestas con múltiples opciones.

### **Desventajas**
- Más complejo que la votación simple: requiere cálculos adicionales.
- Puede no ser ideal para decisiones binarias: funciona mejor con votaciones con múltiples opciones.
- Potencial para la votación estratégica: los votantes pueden manipular las clasificaciones.

### **Mejores casos de uso**
- Elecciones de representantes o miembros del consejo de la DAO.
- Decisiones con múltiples resultados viables.
- Situaciones donde la construcción de consenso es importante.

---

## **Elegir el mecanismo de votación adecuado para su DAO**

Cada DAO requiere diferentes modelos de votación según su tamaño, necesidades de gobernanza y participación de la comunidad.

| **Mecanismo** | **Ideal para** | **Principal desventaja** |
|----------------------|----------------------|--------------------|
| **Voto basado en tokens** | Gobernanza simple | Susceptible al dominio de las ballenas |
| **Voto cuadrático** | Toma de decisiones más justa | Requiere resistencia Sybil |
| **Voto por convicción** | Compromiso a largo plazo | Ciclos de decisión lentos |
| **Consenso holográfico** | Priorización de propuestas | Implementación compleja |
| **Voto delegado** | Participación pasiva en la gobernanza | Riesgos de centralización |
| **Voto por orden de preferencia** | Decisiones con múltiples opciones | Complejidad computacional |

