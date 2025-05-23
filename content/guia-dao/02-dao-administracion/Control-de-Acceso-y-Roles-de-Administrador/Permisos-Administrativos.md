---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Asignación, gestión y revocación de permisos administrativos'
weight: 29_000
---

Garantizar una gestión segura y eficiente de los roles administrativos es fundamental para mantener la integridad de una DAO. Esta sección explora:

- **Asignación de roles**: Definición y distribución de permisos.
- **Gestión de permisos**: Supervisión y ajuste del acceso según sea necesario.
- **Mecanismos de revocación**: Protección contra el uso indebido y minimización de riesgos.

---

## **Asignación de roles administrativos**

Las estructuras de gobernanza de las DAOs suelen requerir diferentes niveles de control administrativo para gestionar las operaciones del protocolo, las decisiones de tesorería y la ejecución de la gobernanza.

### **Tipos de roles comunes**
- **Administradores de gobernanza**: Supervisan las actualizaciones de los contratos inteligentes y las configuraciones críticas.
- **Gerentes de tesorería**: Gestionan la asignación de fondos y las operaciones financieras.
- **Ejecutores de propuestas**: Ejecutan las votaciones de gobernanza exitosas.

### **Mejores prácticas para la asignación de roles**
- **Principio de privilegios mínimos**: Asignar solo los permisos mínimos necesarios.
- **Roles temporales**: Usar privilegios de administrador temporales siempre que sea posible.
- **Verificación multicapa**: Exigir votación on-chain o aprobaciones multifirma para roles críticos.

### **Ejemplo: OpenZeppelin AccessControl**
- El módulo AccessControl facilita permisos basados ​​en roles con asignación granular.
- Los roles se pueden restringir, delegar o revocar mediante votaciones de gobernanza.

---

## **Administración de permisos y consideraciones de seguridad**

Una vez asignados, los permisos deben supervisarse y actualizarse a medida que la DAO evoluciona. Una gestión incorrecta de los roles puede provocar violaciones de seguridad, ataques a la gobernanza o incentivos desalineados.

### **Estrategias de gestión continua de roles**
- **Auditorías periódicas de roles**: Revisar periódicamente los roles de administrador y su necesidad. 
- **Transparencia on-chain**: Utiliza contratos inteligentes para rastrear los cambios de roles.
- **Gobernanza multifirma**: Requiere aprobación colectiva para cambios administrativos.

### **Caso práctico: el ataque de gobernanza a Tornado Cash**
- En 2023, un atacante obtuvo el control de los contratos de gobernanza al explotar los permisos de administrador.
- La falta de mecanismos de revocación y seguridad multicapa permitió la toma de control.

---

## **Revocación de acceso y gestión de la caducidad de roles**

Revocar permisos es tan importante como otorgarlos. Los administradores obsoletos, comprometidos o inactivos deben ser removidos de inmediato para minimizar los riesgos de seguridad.

### **Métodos para revocar permisos**
- **Revocación on-chain**: Elimina roles directamente mediante votaciones de gobernanza.
- **Permisos con límite de tiempo**: Establece fechas de caducidad para roles de administrador críticos.
- **Intervención multifirma**: Requiere consenso grupal antes de ejecutar revocaciones.

### **Mecanismos de revocación de emergencia**
- **Contratos de Guardián**: Direcciones de emergencia que pueden anular permisos.
- **Administradores a prueba de fallos**: Cuentas preaprobadas que pueden eliminar actores maliciosos.

### **Ejemplo: sistema de gestión de roles de Aragon**
- Las DAOs de Aragon utilizan permisos modulares para permitir ajustes dinámicos de roles.
- Se pueden otorgar o revocar permisos de administrador mediante propuestas de la DAO.

---

## **Reflexiones finales**

La seguridad de una DAO depende en gran medida de quién controla los permisos administrativos. Al implementar mecanismos robustos de asignación, monitoreo y revocación, las DAOs pueden prevenir vulnerabilidades de gobernanza, riesgos internos y fallas operativas.