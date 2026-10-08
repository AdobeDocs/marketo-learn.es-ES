---
title: 'Vídeo de API de Marketo: Cómo establecer el token de acceso en una variable'
description: Obtenga información sobre cómo configurar la aplicación de Postman y cómo aprovechar las variables para guardar datos en la variable con fines de reutilización.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00.000Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: dca84292-69e9-4116-a575-667d31fa060d
    internal-label: APIs
subfeature_v2:
  - id: cf1396d8-ab85-4e93-b35d-d9b573024abf
    internal-label: REST APIs
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 4768ecb20d4d9c70452ae084256928261f3a80eb
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 27%
---
# Ayuda sobre la API: cómo establecer el token de acceso en una variable

Obtenga información sobre la configuración de la aplicación de Postman y aprovechamiento de las variables para guardar datos en la variable con fines de reutilización. Además, aprenda a realizar su primera llamada a la API de REST de Marketo Engage para obtener el token de acceso.

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

* [Documentación para desarrolladores de Marketo Engage](https://experienceleague.adobe.com/es/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3453986/?captions=spa&learn=on)
