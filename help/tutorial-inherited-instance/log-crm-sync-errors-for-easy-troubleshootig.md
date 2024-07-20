---
title: Registrar errores de sincronización de CRM para facilitar la resolución de problemas
description: Aprenda a utilizar un registro de errores de sincronización de CRM para investigar los problemas de sincronización de CRM y mantenerla en funcionamiento sin problemas.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 3b7e6127-28fd-4dce-915d-5af9bcce984b
source-git-commit: 681d390ce5ab336a7e24cc63256659a492288517
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Registrar errores de sincronización de CRM para facilitar la resolución de problemas

Como Marketo Engage, comprobar si tu instancia está sincronizada con tu CRM debería ser una parte clave de tu [rutina diaria](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. Aunque la sección [Notificaciones](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (que se encuentra en la esquina superior derecha de la interfaz de Marketo Engage) es donde empezará a buscar e investigar los problemas de sincronización frecuentes, hay una sugerencia profesional que puede ayudarle a administrar el estado de la instancia de forma organizada. Campeona del Adobe de Marketo (2019-2022), Amy Goldfine recomienda a los usuarios administradores que mantengan un registro de los errores de sincronización de CRM para facilitar la resolución de problemas.

![Captura de pantalla de la ficha Errores de sincronización](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## ¿Por qué mantener un registro de los errores de sincronización de CRM?

Al registrar los errores de sincronización de CRM, los administradores de Marketo Engage pueden revisar los problemas y tendencias con los administradores de CRM para corregir la causa raíz. Siga los pasos a continuación para documentar los problemas de sincronización de CRM para su instancia.

## Cómo mantener un registro de los errores de sincronización de CRM

Antes de comenzar, descargue la [plantilla Registro de errores de sincronización con CRM](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Paso 1:** Vaya a la sección *[!UICONTROL Administrador]* del Marketo Engage. En *[!UICONTROL Integración]*, haga clic en *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]* o *[!DNL Veeva]*, dependiendo de qué [!DNL CRM] utilice, y luego en la ficha *[!UICONTROL Errores de sincronización]*.

**Paso 2:** Puede elegir [exportar los registros de errores como  [!DNL CSV] archivo a través del panel [!UICONTROL Filtro]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Si solo tiene unas pocas horas, copiar y pegar directamente desde la ficha *[!UICONTROL Errores de sincronización]* sería la mejor opción.

**Paso 3:** Tenga en cuenta la fecha en la que se produjo el error.

**Paso 4:** Escriba el número de registros de persona afectados por ese error. (A veces, su CRM solo generará un error para una persona. A veces habrá muchas personas con el mismo error a la vez).

**Paso 5:** Tenga en cuenta la dirección de correo electrónico de una persona afectada por el error. Esto facilita la referencia y la conversación de los errores con el administrador de CRM.

**Paso 6:** Pegue vínculos al registro de persona en [!DNL Marketo Engage] y al registro de [!UICONTROL contacto o posible cliente de CRM] de esa persona.

**Paso 7:** En la última columna, pegue el texto real del error.

## ¿Qué sigue?

**Identificar códigos de error:** Para comprender los códigos de error, busque las descripciones en la documentación de desarrolladores [Tabla de códigos de error de nivel de respuesta](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} y busque los pasos siguientes típicos para resolver los errores.

## Autores

**Amy Goldfine**\
Adobe Marketo Champion(2019-2022)
*Fundador, MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Administrador de marketing de adopción y retención en el Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
