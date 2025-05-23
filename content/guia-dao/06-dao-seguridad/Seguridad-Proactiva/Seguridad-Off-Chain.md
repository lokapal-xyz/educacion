---
date: '2025-03-09T16:55:34-03:00'
draft: false
title: 'Preocupaciones de Seguridad Off-Chain'
weight: 98_000
---

Si bien las DAOs operan principalmente en la infraestructura blockchain, las amenazas de seguridad off-chain plantean riesgos significativos que pueden afectar la gobernanza, la seguridad de los miembros y la integridad general. Exploremos las principales vulnerabilidades off-chain que enfrentan las DAOs y cómo mitigarlas eficazmente.

---

## **¿Por Qué es Importante la Seguridad Off-Chain?**

- **Más allá de los contratos inteligentes**
  - Las herramientas de gobernanza de las DAOs, las comunicaciones y las interacciones de los miembros a menudo dependen de plataformas off-chain, lo que genera riesgos de seguridad particulares.
  - Los sistemas off-chain comprometidos pueden manipular las decisiones de las DAOs, filtrar información confidencial o interrumpir las operaciones de gobernanza.
  - Un enfoque de seguridad integral requiere proteger tanto los elementos dentro como fuera de la cadena.

---

## **Principales Amenazas de Seguridad Off-Chain**

- **Herramientas de gobernanza comprometidas**
  - La gobernanza de las DAOs a menudo se basa en Snapshot, Tally o Discourse, no directamente on-chain. 
  - Agentes maliciosos podrían comprometer estas plataformas para alterar las propuestas de gobernanza, falsificar votos o manipular las discusiones.

- **Mitigación:**
  - Implementar autenticación multifactor (MFA) y controles de acceso seguros.
  - Auditar periódicamente los privilegios de administrador y rotar las claves.

---

- ​​**Ataques de phishing e ingeniería social**
  - Los miembros y participantes de la gobernanza suelen ser blanco de ataques de phishing en Discord, Telegram y Twitter.
  - Los atacantes pueden hacerse pasar por colaboradores principales, engañando a los usuarios para que revelen información confidencial.

- **Mitigación:**
  - Informar a los miembros de la DAO sobre los riesgos del phishing y verificar las identidades antes de interactuar.
  - Utilizar dominios oficiales de la DAO y mensajes firmados para las comunicaciones importantes.

---

- ​​**Canales de comunicación explotados**
  - Muchas DAOs se coordinan a través de Discord, Telegram y foros, que son vulnerables a la toma de control de la administración y la manipulación de mensajes.
  - Los atacantes pueden difundir desinformación, eliminar discusiones de gobernanza o manipular narrativas.

- **Mitigación:**
  - Restringir el acceso de administrador y usar MFA para los moderadores de Discord/Telegram.
  - Mantener las discusiones de gobernanza archivadas públicamente para evitar la manipulación de datos.

---

- ​​**Vulnerabilidades de la nube y las claves API**
  - Muchas DAOs utilizan API off-chain para herramientas de gobernanza, seguimiento de tesorería o agregación de datos.
  - Si se filtran las claves API o las credenciales de la nube, los atacantes pueden modificar los paneles de la DAO, bloquear votos o secuestrar multifirmas.

- **Mitigación:**
  - Usar herramientas de gestión de secretos (p. ej., HashiCorp Vault, AWS Secrets Manager).
  - Rotar las claves API regularmente y usar el acceso con privilegios mínimos para los servicios en la nube.

---

- ​​**Riesgos regulatorios y legales**
  - Las DAOs suelen interactuar con entidades off-chain, como bancos, estructuras legales o asociaciones. 
  - El incumplimiento legal puede provocar cierres, congelación de activos o demandas.

- **Mitigación:**
  - Establecer marcos legales claros y consideraciones jurisdiccionales.
  - Utilizar la descentralización progresiva para reducir las responsabilidades centralizadas.

---

## **Mejores Prácticas Para la Seguridad DAO Off-Chain**

- **Herramientas de gobernanza segura**: Utilizar MFA, acceso basado en roles y auditorías de seguridad periódicas.
- **Proteger las comunicaciones de los miembros**: Implementar canales de confianza, mensajería cifrada y moderación de bots.
- **Reforzar la infraestructura off-chain**: Proteger las claves API, los servicios en la nube y las integraciones externas.
- **Educar a los miembros de las DAOs**: Concientizar sobre la ingeniería social, el phishing y la verificación de identidad.