---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Preocupaciones de Seguridad Off-Chain'
weight: 98_000
---

Si bien las DAO operan principalmente en la infraestructura blockchain, las amenazas de seguridad fuera de la cadena plantean riesgos significativos que pueden afectar la gobernanza, la seguridad de los miembros y la integridad general. Exploremos las principales vulnerabilidades fuera de la cadena que enfrentan las DAO y cómo mitigarlas eficazmente.

---

## **¿Por qué es importante la seguridad fuera de la cadena?**

---

**Más allá de los contratos inteligentes**

---

Las herramientas de gobernanza de las DAO, las comunicaciones y las interacciones de los miembros a menudo dependen de plataformas fuera de la cadena, lo que genera riesgos de seguridad fuera de la cadena.

---

Los sistemas fuera de la cadena comprometidos pueden manipular las decisiones de las DAO, filtrar información confidencial o interrumpir las operaciones de gobernanza.

---

Un enfoque de seguridad integral requiere proteger tanto los elementos dentro como fuera de la cadena.

---

## **Principales amenazas de seguridad fuera de la cadena**

---

**Herramientas de gobernanza comprometidas**

---

La gobernanza de las DAO a menudo se basa en Snapshot, Tally o Discourse, no directamente en la cadena. Agentes maliciosos podrían comprometer estas plataformas para alterar las propuestas de gobernanza, falsificar votos o manipular las discusiones.

- **Mitigación:**
- Implementar autenticación multifactor (MFA) y controles de acceso seguros.
- Auditar periódicamente los privilegios de administrador y rotar las claves.

- ---

- ​​**Ataques de phishing e ingeniería social**
- Los miembros y participantes de la gobernanza suelen ser blanco de ataques de phishing en Discord, Telegram y Twitter.
- Los atacantes pueden hacerse pasar por colaboradores principales, engañando a los usuarios para que revelen información confidencial.

- **Mitigación:**
- Informar a los miembros de la DAO sobre los riesgos del phishing y verificar las identidades antes de interactuar.
- Utilizar dominios oficiales de la DAO y mensajes firmados para las comunicaciones importantes.

- ---

- ​​**Canales de comunicación explotados**
- Muchas DAO se coordinan a través de Discord, Telegram y foros, que son vulnerables a la toma de control de la administración y la manipulación de mensajes.
- Los atacantes pueden difundir desinformación, eliminar discusiones de gobernanza o manipular narrativas.

- **Mitigación:**
- Restringir el acceso de administrador y usar MFA para los moderadores de Discord/Telegram.
- Mantener las discusiones de gobernanza archivadas públicamente para evitar la manipulación de datos.

- ---

- ​​**Vulnerabilidades de la nube y las claves API**
- Muchas DAO utilizan API fuera de la cadena para herramientas de gobernanza, seguimiento de tesorería o agregación de datos.
- Si se filtran las claves API o las credenciales de la nube, los atacantes pueden modificar los paneles de la DAO, bloquear votos o secuestrar multifirmas.

- **Mitigación:**
- Usar herramientas de gestión de secretos (p. ej., HashiCorp Vault, AWS Secrets Manager).
- Rotar las claves API regularmente y usar el acceso con privilegios mínimos para los servicios en la nube.

- ---

- ​​**Riesgos regulatorios y legales**
- Las DAO suelen interactuar con entidades fuera de la cadena, como bancos, estructuras legales o asociaciones. - El incumplimiento legal puede provocar cierres, congelación de activos o demandas.

- **Mitigación:**
- Establecer marcos legales claros y consideraciones jurisdiccionales.
- Utilizar la descentralización progresiva para reducir las responsabilidades centralizadas.

---

## **Mejores prácticas para la seguridad fuera de la cadena en DAO**

- **Herramientas de gobernanza segura**: Utilizar MFA, acceso basado en roles y auditorías de seguridad periódicas.
- **Proteger las comunicaciones de los miembros**: Implementar canales de confianza, mensajería cifrada y moderación de bots.
- **Reforzar la infraestructura fuera de la cadena**: Proteger las claves API, los servicios en la nube y las integraciones externas.
- **Educar a los miembros de las DAO**: Concientizar sobre la ingeniería social, el phishing y la verificación de identidad.