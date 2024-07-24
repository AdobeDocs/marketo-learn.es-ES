---
title: Migración a Identity Management de Adobe
description: Descripción próximamente.
role: User
level: Beginner
hide: true
hidefromtoc: true
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: fe760c2fc53b96d5c176de377730bce2e89dbc74
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# Migración a Identity Management de Adobe

El Adobe está mejorando la forma de administrar las suscripciones y los usuarios de Adobe Marketo Engage. Estamos mejorando la productividad para usted y su organización mediante la migración de sus suscripciones de Marketo Engage y usuarios a Adobe Admin Console.

Este tutorial le permite desplazarse por la migración para poder administrar Adobe Marketo Engage junto con otras cuentas de Adobe y productos para los usuarios en una ubicación central. La migración es necesaria y no afectará al flujo de trabajo, el contenido, las integraciones ni los recursos de marketing.

## Lista de comprobación previa a la migración para administradores de Marketo Engage {#pre-migration-checklist-for-marketo-engage-administrators}

Para garantizar que su organización pueda migrar Adobe Marketo Engage a Adobe Admin Console, le recomendamos que siga la lista de comprobación siguiente para administrar los próximos cambios.

### 1. Identifique a los administradores del sistema y comente las acciones que pueden tener que realizar {#identify-your-system-administrators}

* Si no está seguro de quiénes son los administradores del sistema de su organización, póngase en contacto con el equipo de cuenta de Adobe o póngase en contacto con el soporte técnico de Adobe `marketocares@marketo.com`.

* Confirme la Adobe Admin Console (u organización de Adobe) a la que se migrarán las suscripciones de Marketo Engage.  Las suscripciones de Marketo Engage deben implementarse en la misma organización que Dynamic Chat, una herramienta nativa de automatización de conversaciones integrada con Marketo Engage.
  `TBD LINK TO https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete`

* Obtenga más información acerca de cómo comunicarse con los administradores del sistema en la [Sección de correo electrónico de ejemplo](#announce-the-migration-timeline).

### 2. Familiarícese con los cambios y el impacto de migrar a Identidad de Adobe {#familiarize-yourself-with-the-changes}

En el siguiente vídeo, el equipo de administración de productos Marketo Engage le explica el recorrido de migración y qué esperar.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?quality=12&learn=on){transcript=true}

Encontrará más ayuda sobre este tema para los administradores de Marketo Engage en los siguientes artículos de ayuda:

* [Lista de comprobación de configuración de usuario](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Información general de Identity Management de Adobe](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migrando a la identidad de Adobe con la consola de migración](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Entender cómo usar Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html){target="_blank"}

### 3. Anuncie a sus equipos internos el calendario y la preparación de la migración necesarios {#announce-the-migration-timeline}

* Marque la fecha de migración en los calendarios de los administradores del Marketo Engage y los usuarios una vez que se haya programado.

Puede modificar la fecha de migración en **Administración** > **Consola de migración** > **Premigración** para que se ajuste mejor a la cronología interna. Obtenga más información acerca de la reprogramación y las limitaciones de [modificar la fecha de migración](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* Envíe un correo electrónico para comunicarse con los administradores del sistema.

A continuación se muestra un ejemplo de correo electrónico que puede enviar a los administradores del sistema. Normalmente, el departamento de TI gestiona todas las licencias de Adobe.

`---------------------------------------------------`

**Asunto: Se necesita asistencia—Migración de suscripciones de Marketo Engage a Adobe Admin Console**

Estimado `[IT Administrator/NAME]`:

Nuestra suscripción de Marketo Engage se migrará pronto al sistema Identity Management de Adobe. `[Marketing Operation team]` necesita su ayuda para completar algunos pasos necesarios antes de que comience la migración de usuarios, a fin de minimizar el impacto en los usuarios de Marketo Engage.

`1.` Confirme si la organización ya administra otros productos de Adobe en Adobe Admin Console y si Marketo Engage se migrará a la misma consola.

* Tenga en cuenta que las suscripciones de Marketo Engage deben estar en la misma organización que Dynamic Chat, una herramienta nativa de automatización de conversaciones integrada con Marketo Engage.

* Si tiene dudas o preguntas acerca del Admin Console al que se agregará un Marketo Engage, comuníquese con el equipo de atención al cliente en `marketocares@marketo.com` e inclúyanos en su comunicación.

`2.` Esté atento a un correo electrónico de Adobe con la línea de asunto &quot;Acción necesaria para administrar el acceso de los usuarios a Adobe Marketo Engage `[Package Tier]`&quot;. Este correo electrónico se ha enviado después de aprovisionar las licencias de Marketo Engage en nuestro Admin Console. Solo los administradores del sistema recibirán este correo electrónico. Por favor, infórmenos de inmediato cuando lo reciba.

* El Adobe puede solicitar su consentimiento, que es el administrador del sistema del Admin Console, para migrar automáticamente a los usuarios a la consola existente de su organización. En el mensaje de correo electrónico con la línea de asunto &quot;Acción necesaria para administrar el acceso de los usuarios a Adobe Marketo Engage `[Package Tier]`&quot;, haga clic en el botón &quot;Comenzar&quot; para ir a la página de consentimiento.

`3.` **Opcional:** Configuración de SSO (inicio de sesión único) en Adobe Admin Console.

* Para que nuestros usuarios puedan iniciar sesión con SSO en su identidad de Adobe a partir de ahora, le pedimos que nos ayude con la configuración de SSO en Adobe Admin Console antes de que se produzca la migración de usuarios.
Agradecemos su cooperación durante esta transición. Avíseme cuando haya completado estos pasos para poder continuar con la migración de usuarios con Marketo Engage.
Un saludo,

`[Your Name]`

`---------------------------------------------------`

* Envíe un correo electrónico a los usuarios de Marketo Engage.

A continuación se muestra un ejemplo de correo electrónico que puede utilizar para anunciar la próxima migración a los usuarios de Marketo Engage que no tienen privilegios de administrador.

`---------------------------------------------------`

**Asunto: Actualización importante: migración de suscripciones de Marketo Engage a Adobe Admin Console**

Estimados usuarios de Marketo Engage:

Tenemos un anuncio importante sobre la instancia de Marketo Engage y cómo iniciará sesión. El Adobe consiste en trasladar las suscripciones de Marketo Engage y los usuarios a Adobe Admin Console para permitir a sus clientes centralizar toda la administración de productos en un solo lugar. Esto no afectará a los flujos de trabajo, el contenido, las integraciones ni los recursos de marketing.

Detalles clave:

* Fecha de migración: [Especifique la fecha programada; busque esta información en el Marketo Engage en **Administración** > **Consola de migración** > **Premigración**]

* Horario: la migración comienza alrededor de la medianoche (hora local) para nuestra suscripción.

* Impacto: no se perderá el acceso al producto durante la migración de usuarios. Si ha iniciado sesión cuando se migra su cuenta, se cerrará la sesión y se le pedirá que vuelva a iniciarla en cuestión de minutos mediante el servicio de identidad de Adobe después de la migración.

* Ventajas: Autentique el Marketo Engage y otros productos de Adobe mediante una sola identidad de Adobe, ya sea un Federated ID de Adobe ID o de Adobe (SSO).

Qué debe hacer:

`1.` Prepararse: se requiere la verificación por correo electrónico para que pueda migrarse a una identidad de Adobe.

i. Ha recibido un correo electrónico de solicitud de verificación por correo electrónico con un vínculo (permanece válido durante 3 días). Si el vínculo ha caducado, puedes volver a enviar el correo electrónico de verificación yendo a **Administración** > **Mi cuenta** > **Configuración de la cuenta** y haciendo clic en **Volver a enviar verificación**.
ii. Se requiere una sesión de usuario activa para que la verificación del correo electrónico se realice correctamente. Inicie sesión en la suscripción de Marketo Engage usando primero la URL del proveedor de identidad (IdP).

`2.` integrada: una vez que se haya migrado su cuenta de usuario, recibirá un correo electrónico del Adobe con respecto a los cambios en el método de inicio de sesión.

i. Acepte la nueva invitación haciendo clic en el botón &quot;Aceptar invitación&quot; e iniciando sesión con el Adobe Identidad.
ii. En la página de inicio de sesión de Adobe, inicie sesión con un Adobe ID existente.

`3.` Contacto: si tiene alguna pregunta o necesita ayuda después de migrar su cuenta o si no se ha migrado su cuenta y ha perdido el acceso a Marketo Engage, póngase en contacto con el equipo de migración de Marketo Engage en `[your internal contact email/phone]`.

Agradecemos su cooperación durante esta transición. Gracias por su comprensión y compromiso para mantener nuestros sistemas seguros.

Mejor,

`[Your Name]`

`---------------------------------------------------`
