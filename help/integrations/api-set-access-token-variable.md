---
title: 'Vídeo de API de Marketo: Cómo establecer el token de acceso en una variable'
description: Obtenga información sobre cómo configurar la aplicación de Postman y cómo aprovechar las variables para guardar datos en la variable con fines de reutilización.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
source-git-commit: 3243c3047efa1bcb92581a58aafe17689ff945fd
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 24%

---

# Ayuda de la API: cómo establecer el token de acceso en una variable

Obtenga información sobre la configuración de la aplicación de Postman y aprovechamiento de las variables para guardar datos en la variable con fines de reutilización. También aprenderá a realizar su primera llamada a la API de REST de Marketo Engage para obtener el token de acceso.

>[!PREREQUISITES]
>
>Antes de iniciar este vídeo, cree un nombre de usuario de solo API con una función de AOI y un servicio de Launchpad. Siga los pasos de los artículos siguientes:
>
>* [Crear un rol de usuario solo de API](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"}
>
>* [Crear un usuario solo de API](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"}
>
>* [Crear un servicio personalizado para utilizarlo con la API de REST](https://experienceleague.adobe.com/es/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"}

**Referencias utilizadas en este vídeo:**

* Extremo de autenticación de Marketo: `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* Script JS para obtener access_token del cuerpo de respuesta (se coloca en la pestaña Scripts: ):

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* [Documentación para desarrolladores Marketo Engage](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3429275/?learn=on)
