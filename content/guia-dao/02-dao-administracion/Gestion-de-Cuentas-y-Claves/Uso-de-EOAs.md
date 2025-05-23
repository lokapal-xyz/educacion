---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Uso de EOAs, multisigs y billeteras de contratos inteligentes'
weight: 33_000
---

La gestión eficaz de cuentas y claves es crucial para la seguridad y la gobernanza de las DAOs. Esta sección explora los tres tipos principales de billeteras utilizados en las DAO:

- **Cuentas de propiedad externa (EOA)**: Billeteras simples controlados por una clave privada.
- **Billeteras multifirma**: Requieren múltiples aprobaciones para las transacciones.
- **Billeteras de contratos inteligentes**: Billeteras programables con funciones de seguridad avanzadas.

Cada tipo de billetera ofrece distintas ventajas en cuanto a seguridad, descentralización y usabilidad.

---

## **Cuentas de propiedad externa (EOA)**

Una EOA es una billetera estándar controlada por una única clave privada, que generalmente se gestiona a través de billeteras como MetaMask, Ledger o Trezor.

### **Ventajas**
- **Simplicidad**: Fácil de configurar y usar.
- **Bajos costos de gas**: Sin interacciones on-chain adicionales.
- **Control total**: Solo el titular de la clave puede firmar las transacciones.

### **Desafíos**
- **Punto único de fallo**: si la clave privada se pierde o se ve comprometida, el acceso se pierde permanentemente.
- **Sin recuperación integrada**: a diferencia de las billeteras de contratos inteligentes, las EOAs carecen de opciones de recuperación de cuentas.
- **Riesgo de centralización**: en un entorno DAO, una única EOA que controle las funciones clave socava la descentralización.

### **Casos de uso en DAOs**
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

### **Casos de uso en DAOs**
- Se utiliza comúnmente para la gestión de tesorería.
- Ayuda a los comités de gobernanza a controlar las acciones administrativas con altos privilegios.
- Se utiliza para la financiación de subvenciones y garantizar una distribución justa. 

---

## **Billeteras de contratos inteligentes**

Una billetera de contratos inteligentes es una cuenta programable que puede aplicar reglas de seguridad. Algunos ejemplos son Safe Modules, Argent y los billeteras Inteligentes Kernel.

### **Características de las billeteras de contratos inteligentes**
- **Permisos personalizables**: Define quién puede ejecutar ciertas acciones.
- **Mecanismos de recuperación de cuenta**: Habilita la recuperación social o configuraciones multiclave.
- **Abstracción de gas**: Algunos billeteras permiten el pago de comisiones en tokens en lugar de ETH.

### **Ventajas**
- **Seguridad avanzada**: Puede incluir timelocks, límites de retiro o lógica multifirma.
- **Programabilidad**: Se puede implementar una lógica de gobernanza personalizada.
- **Recuperación fácil de usar**: Reduce el riesgo de pérdida permanente debido a la mala gestión de la clave privada.

### **Desafíos**
- **Mayores costos de gas**: La ejecución de contratos inteligentes requiere más gas que las EOAs. 
- **Complejidad**: Requiere una configuración y auditorías de seguridad adecuadas.
- **Riesgos en la actualización**: Las actualizaciones mal diseñadas pueden introducir vulnerabilidades.

### **Casos de uso en DAOs**
- Ideal para contratos controlados por la gobernanza (p. ej., desembolso automatizado de tesorería).
- Se utiliza para el control de identidad y acceso basado en DAOs.
- Facilita la descentralización progresiva al pasar de una gobernanza multifirma a una gobernanza de contratos inteligentes.

---

## **Comparación: EOAs vs. multifirmas vs. billeteras de contratos inteligentes**

| **Característica** | **EOA** | **Billetera multifirma** | **Billetera de contratos inteligentes** |
|-------------------|------|----------------|----------------------|
| **Seguridad** | Baja | Alta | Muy Alta |
| **Descentralización** | Ninguna | Moderada | Alta |
| **Facilidad de uso** | Alta | Moderada | Baja |
| **Costo de gas** | Bajo | Moderado | Alta |
| **Personalización** | Ninguna | Baja | Alta |
| **Ideal para** | Particulares | Tesorería, Control Administrativo | Gobernanza Automatizada |

Las DAOs deben elegir el tipo de billetera adecuado según sus necesidades de gobernanza, buscando un equilibrio entre seguridad, descentralización y usabilidad.