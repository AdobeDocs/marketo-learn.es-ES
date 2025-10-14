---
title: Migración a Adobe Identity Management
description: Este tutorial le ayudará a navegar por la migración de sus suscripciones de Marketo Engage y usuarios a Adobe Admin Console.
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: dcfffa299cbcfef489f5b618fae29f745b878d26
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Migración a Adobe Identity Management

Adobe está mejorando la forma de administrar las suscripciones y los usuarios de Adobe Marketo Engage. Estamos aumentando la productividad de su organización mediante la migración de sus suscripciones y usuarios de Marketo Engage a Adobe Admin Console.

Este tutorial le ayudará a navegar por la migración para que pueda empezar a administrar Adobe Marketo Engage junto con otras cuentas y productos de Adobe para sus usuarios en una ubicación central. La migración es necesaria y no afectará al flujo de trabajo, el contenido, las integraciones ni los recursos de marketing.

## Lista de comprobación previa a la migración para administradores de Marketo Engage {#pre-migration-checklist-for-marketo-engage-administrators}

Para garantizar que su organización pueda migrar Adobe Marketo Engage a Adobe Admin Console, le recomendamos que siga la lista de comprobación siguiente para administrar los próximos cambios.

### 1. Identifique a los administradores del sistema y al equipo de TI y comente las acciones que pueden tener que realizar {#identify-your-system-administrators}

* Si no está seguro de qué administradores del sistema pertenecen a su organización, póngase en contacto con el equipo de cuenta de Adobe o póngase en contacto con el soporte técnico de Adobe `marketocares@marketo.com`.

* Confirme la Adobe Admin Console (o la organización de Adobe) a la que se migrarán las suscripciones de Marketo Engage. Es probable que tengas un Adobe Admin Console para [Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, una herramienta nativa de automatización de conversaciones en Marketo Engage. Las suscripciones de Marketo Engage deben implementarse en la misma organización que Dynamic Chat.

* Trabaje con su equipo de TI para realizar la lista de permitidos de todos los dominios de Adobe enumerados [&#x200B; en la parte superior de este artículo](https://experienceleague.adobe.com/es/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} para evitar la interrupción del acceso a Marketo Engage después de la migración a Adobe Identity.

* **Opcional:** [Implementar el inicio de sesión único (SSO)](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} antes de la migración de usuarios.

  >[!NOTE]
  >
  >Existen diferencias entre el SSO compatible con Marketo Engage y el SSO de Adobe Admin Console. Por lo tanto, es posible que sea necesario implementar cambios en la configuración.

* **Opcional:** Personalice la [duración máxima de sesión deseada](https://helpx.adobe.com/es/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} antes de la migración de usuarios para que los usuarios de Marketo Engage permanezcan autenticados.

* Aprenda qué debe comunicarse con los administradores del sistema en la [Sección de correo electrónico de ejemplo](#announce-the-migration-timeline).

### 2. Familiarícese con los cambios y el impacto de la migración a Adobe Identity {#familiarize-yourself-with-the-changes}

En el siguiente vídeo, el equipo de administración de productos de Marketo Engage le explica el recorrido de migración y qué esperar.

>[!VIDEO](https://video.tv.adobe.com/v/3432370/?t=170/?quality=12&learn=on&captions=spa){transcript=true}

Encontrará más ayuda sobre este tema para los administradores de Marketo Engage en los siguientes artículos de ayuda:

* [Lista de comprobación de configuración de usuario](https://experienceleague.adobe.com/es/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Información general sobre Adobe Identity Management](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Explicación de la suscripción de Marketo y la migración de usuarios a Adobe Admin Console](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migración a la identidad de Adobe con la consola de migración](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Entender cómo usar Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html){target="_blank"}

### 3. Anuncie a sus equipos internos el calendario y la preparación de la migración necesarios {#announce-the-migration-timeline}

* Marque la fecha de migración en los calendarios de los administradores y usuarios de Marketo Engage una vez programada.

   * Puede modificar la fecha de migración en **Administración** > **Consola de migración** > **Premigración** para que se ajuste mejor a su cronograma interno. Obtenga más información acerca de la reprogramación y las limitaciones de [modificar la fecha de migración](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **Envíe un correo electrónico a los administradores del sistema**

A continuación se muestra un ejemplo de correo electrónico para enviar a sus administradores. Normalmente, el departamento de TI administra todas las licencias de Adobe.

+++ Correo electrónico de ejemplo para enviar a los administradores del sistema

**Asunto: Se necesita asistencia—Migración de suscripciones de Marketo Engage a Adobe Admin Console**

Estimado `[IT Administrator/NAME]`:

Nuestra suscripción a Marketo Engage se migrará pronto al sistema Identity Management de Adobe. `[Marketing Operation team]` necesita su ayuda para completar algunos pasos necesarios antes de que comience la migración de usuarios, a fin de minimizar el impacto en los usuarios de Marketo Engage.

`1.`: confirme si la organización ya administra otros productos de Adobe en Adobe Admin Console y si Marketo Engage se migrará a la misma consola.

* Las suscripciones a Marketo Engage deben estar en la misma organización que Dynamic Chat, una herramienta nativa de automatización de conversaciones integrada con Marketo Engage.

* Si tiene alguna pregunta o duda con respecto a Admin Console, póngase en contacto con el Soporte técnico de Adobe en `marketocares@marketo.com` y comuníquese con CC.

`2.` Esté atento a un correo electrónico de Adobe con la línea de asunto &quot;Acción necesaria para administrar el acceso de los usuarios a Adobe Marketo Engage `[Package Tier]`&quot;. Este correo electrónico se ha enviado después de aprovisionar las licencias de Marketo Engage en nuestro Admin Console. Solo los administradores del sistema recibirán este correo electrónico. Por favor, infórmenos de inmediato cuando lo reciba.

* Adobe puede solicitar su consentimiento, como administrador del sistema de Admin Console, para migrar automáticamente a los usuarios a la consola existente de su organización. En el mensaje de correo electrónico con la línea de asunto &quot;Acción necesaria para administrar el acceso de los usuarios a Adobe Marketo Engage `[Package Tier]`&quot;, haga clic en el botón &quot;Comenzar&quot; para ir a la página de consentimiento.

`3.` Después de la migración, Marketo Engage pasará de estar disponible desde experience.adobe.com a Adobe Experience Cloud. Realice una lista de permitidos de todos los dominios de Adobe enumerados [&#x200B; en la parte superior de este artículo](https://experienceleague.adobe.com/es/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} para evitar interrupciones en el acceso a Marketo Engage.

`4.` **Opcional:** Configurar SSO (inicio de sesión único) en Adobe Admin Console.

* Para beneficiar a los usuarios que inician sesión con SSO en su servicio de identidad de Adobe a partir de ahora, ayuden a configurar el SSO en Adobe Admin Console antes de que se produzca la migración de usuarios.

`5.` **Opcional:** Establezca una [duración máxima de sesión](https://helpx.adobe.com/es/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} más larga en Adobe Admin Console.

* Para evitar que los usuarios tengan que iniciar sesión con frecuencia, personalice la duración de la sesión en la Configuración avanzada con una duración más larga.

Agradecemos su cooperación durante esta transición. Avíseme cuando haya completado estos pasos para que pueda continuar con la migración.

Un saludo,

`[Your Name]`

+++

* **Enviar un correo electrónico a los usuarios de Marketo Engage**

A continuación se muestra un ejemplo de correo electrónico para usuarios de Marketo Engage que **no** tienen privilegios de administrador.

+++ Ejemplo de correo electrónico que anuncia la próxima migración

**Asunto: Actualización importante: migración de suscripciones de Marketo Engage a Adobe Admin Console**

Estimados usuarios de Marketo Engage:

Tenemos un anuncio importante sobre nuestra instancia de Marketo Engage y cómo iniciará sesión. Adobe está trasladando suscripciones y usuarios de Marketo Engage a Adobe Admin Console para permitirnos centralizar toda la administración de productos en una ubicación. Esto no afectará a los flujos de trabajo, el contenido, las integraciones ni los recursos de marketing.

**Detalles de clave:**

* **Fecha de migración**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Horario**: la migración comienza alrededor de la medianoche (hora local) para nuestra suscripción.

* **Impacto**: no habrá pérdida de acceso al producto durante la migración de usuarios. Si inicia sesión cuando migran su cuenta, se cerrará la sesión y se le pedirá que vuelva a iniciarla en cuestión de minutos mediante Adobe Identity después de la migración.

* **Ventajas**: Autentique Marketo Engage y otros productos de Adobe con una sola identidad de Adobe: Adobe ID o Adobe Federated ID (SSO).

**Lo que necesita hacer:**

`1.` **Preparar**: se requiere la verificación por correo electrónico para migrar a una identidad de Adobe.

i. Ha recibido un correo electrónico de solicitud de verificación por correo electrónico con un vínculo (permanece válido durante 3 días). Si el vínculo ha caducado, puede volver a enviar el correo electrónico de verificación desde Marketo Engage haciendo clic en el icono &quot;Mi perfil&quot; y, a continuación, ir a **Mi cuenta** > **Configuración de la cuenta** > **Volver a enviar la verificación**.

ii. Se requiere una sesión de usuario activa para que la verificación del correo electrónico se realice correctamente. Inicie sesión en la suscripción de Marketo Engage usando primero la URL del proveedor de identidad (IdP).

`2.` **Incorporado**: Una vez migrada su cuenta de usuario, recibirá un mensaje de correo electrónico de Adobe con respecto a los cambios en el método de inicio de sesión.

i. Acepte la nueva invitación haciendo clic en el botón &quot;Aceptar invitación&quot; e iniciando sesión con Adobe Identity.

ii. En la página de inicio de sesión de Adobe, inicie sesión con un Adobe ID existente.

iii. Primero debe iniciar sesión en la instancia de Marketo Engage para cualquier dirección URL previamente marcada en el dominio engage-xx.marketo.com al que vaya a navegar.

`3.` **Contacto**: Si tiene alguna pregunta o necesita ayuda después de migrar su cuenta, o si su cuenta no se ha migrado y ha perdido el acceso a Marketo Engage, póngase en contacto con el equipo de migración de Marketo Engage en `[your internal contact email/phone]`.

Agradecemos su cooperación durante esta transición. Gracias por su comprensión y compromiso para mantener nuestros sistemas seguros.

Un saludo,

`[Your Name]`

+++
