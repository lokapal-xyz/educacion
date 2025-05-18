---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Uso de EOAs, Multisigs y Billeteras de Contratos Inteligentes'
weight: 33_000
---

Externally Owned Accounts (EOA, cuentas de propiedad externa)


La gestión eficaz de cuentas y claves es crucial para la seguridad y la gobernanza de las DAO. Esta sección explora los tres tipos principales de billeteras utilizados en las DAO:

- **Cuentas de Propiedad Externa (EOA)**: billeteras simples controlados por una clave privada.
- **billeteras Multifirma**: Requieren múltiples aprobaciones para las transacciones.
- **billeteras de Contratos Inteligentes**: billeteras programables con funciones de seguridad avanzadas.

Cada tipo de monedero ofrece distintas ventajas en cuanto a seguridad, descentralización y usabilidad.

- ---

## **Cuentas de Propiedad Externa (EOA)**

Un EOA es un monedero estándar controlado por una única clave privada, que generalmente se gestiona a través de billeteras como MetaMask, Ledger o Trezor.

### **Ventajas**
- **Simplicidad**: Fácil de configurar y usar.
- **Bajos Costos de Gas**: Sin interacciones contractuales adicionales.
- **Control Total**: Solo el titular de la clave puede firmar las transacciones.

### **Desafíos**
- **Punto único de fallo**: si la clave privada se pierde o se ve comprometida, el acceso se pierde permanentemente.
- **Sin recuperación integrada**: a diferencia de las billeteras de contratos inteligentes, las EOA carecen de opciones de recuperación de cuentas.
- **Riesgo de centralización**: en un entorno DAO, una única EOA que controle las funciones clave socava la descentralización.

### **Casos de uso de DAO**
- Adecuado para contribuyentes individuales que reciben pagos.
- Se utiliza para roles DAO con privilegios bajos donde la descentralización no es una preocupación.

---

## **Billeteras multifirma**

Una billetera multifirma (multisig) requiere que varios firmantes aprueben las transacciones. Las soluciones multifirma más populares incluyen Gnosis Safe y TotalSig.

### **Cómo funcionan las multifirmas**
- Requieren M de N firmas (por ejemplo, 3 de 5 firmantes).
- Las transacciones solo se ejecutan si se alcanza el umbral requerido.

### **Ventajas**
- **Seguridad mejorada**: evita que una sola clave comprometida ejecute transacciones.
- **Control compartido**: garantiza que las decisiones involucren a múltiples partes de confianza.
- **Gobernanza integrada**: se alinea con la toma de decisiones descentralizada.

### **Desafíos**
- **Ejecución más lenta**: las transacciones requieren múltiples aprobaciones, lo que puede retrasar las operaciones.
- **Complejidad de coordinación**: requiere la participación continua de los firmantes.
- **Vulnerabilidad a la colusión**: si la mayoría de los firmantes coluden, pueden eludir las medidas de seguridad.

### **Casos de uso de DAO**
- Se utiliza comúnmente para la gestión de tesorería.
- Ayuda a los comités de gobernanza a controlar las acciones administrativas con altos privilegios.
- Se utiliza para la financiación de subvenciones y garantizar una distribución justa. ---

## **billeteras de Contratos Inteligentes**

Un monedero de contratos inteligentes es una cuenta programable que puede aplicar reglas de seguridad. Algunos ejemplos son Safe Modules, Argent y los billeteras Inteligentes Kernel.

### **Características de los billeteras de Contratos Inteligentes**
- **Permisos Personalizables**: Define quién puede ejecutar ciertas acciones.
- **Mecanismos de Recuperación de Cuenta**: Habilita la recuperación social o configuraciones multiclave.
- **Abstracción de Gas**: Algunos billeteras permiten el pago de comisiones en tokens en lugar de ETH.

### **Ventajas**
- **Seguridad Avanzada**: Puede incluir bloqueos de tiempo, límites de retiro o lógica multifirma.

- **Programabilidad**: Se puede implementar una lógica de gobernanza personalizada.

- **Recuperación Fácil de Usar**: Reduce el riesgo de pérdida permanente debido a la mala gestión de la clave privada.

### **Desafíos**
- **Mayores Costos de Gas**: La ejecución de contratos inteligentes requiere más gas que los EOA. - **Complejidad**: Requiere una configuración y auditorías de seguridad adecuadas.
- **Riesgos de actualizabilidad**: Las actualizaciones mal diseñadas pueden introducir vulnerabilidades.

### **Casos de uso de DAO**
- Ideal para contratos controlados por la gobernanza (p. ej., desembolso automatizado de tesorería).
- Se utiliza para el control de identidad y acceso basado en DAO.
- Facilita la descentralización progresiva al pasar de una gobernanza multifirma a una gobernanza de contratos inteligentes.

---

## **Comparación: EOA vs. Multifirmas vs. billeteras de Contratos Inteligentes**

| Característica | EOA | Monedero Multifirma | Monedero de Contratos Inteligentes |
|-------------------|------|----------------|----------------------|
| **Seguridad** | Baja | Alta | Muy Alta |
| **Descentralización** | Ninguna | Moderada | Alta |
| **Facilidad de uso** | Alta | Moderada | Baja |
| **Costo de gas** | Bajo | Moderado | Alta |
| **Personalización** | Ninguna | Baja | Alta |
| **Ideal para** | Particulares | Tesorería, Control Administrativo | Gobernanza Automatizada |

Las DAO deben elegir el tipo de billetera adecuado según sus necesidades de gobernanza, buscando un equilibrio entre seguridad, descentralización y usabilidad.