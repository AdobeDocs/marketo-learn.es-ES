---
title: Desarrollar una guía de gobernanza de instancias con documentación
description: Aprenda a establecer un procedimiento sólido para crear y mantener la documentación y el registro de cambios para la instancia de Marketo Engage. Esto no solo ahorrará tiempo para el intercambio de conocimientos de su equipo, sino que también mejorará la salud y la eficacia de su instancia.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
exl-id: 4313b54a-1848-4684-b037-7a7795dd01ec
source-git-commit: 681d390ce5ab336a7e24cc63256659a492288517
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# Desarrollar una guía de gobernanza de instancias con documentación

A medida que avanza hacia una instancia heredada de [!DNL Marketo Engage], a menudo se presenta con el desafío de carecer de documentación funcional y técnica actualizada. Como administrador, establecer directrices para garantizar un control adecuado de las instancias es una responsabilidad central que no se puede pasar por alto. Es una de las estrategias críticas para [aumentar la eficacia mientras trabaja en una instancia de Marketo Engage establecida](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

Este tutorial paso a paso originado en [!DNL Adobe Marketo Champion] (2018), Nick Hajdin, lo guiará a través de este proceso para esbozar la configuración de la instancia, documentar los programas operativos principales y mantener un [!DNL changelog] para aplicar una directiva de gobernanza estricta.

## ¿Por qué desarrollar una guía y documentación de gobernanza de instancias para su instancia heredada?

La documentación detallada y un [!DNL changelog] son vitales para una administración eficiente y la transferencia de conocimientos dentro de su instancia de [!DNL Marketo Engage]. Realizar un seguimiento de los cambios y las decisiones que ha realizado durante la configuración de la instancia puede ayudarle a lo siguiente:

1. Capacite a los usuarios internos de forma más sencilla y escalable.
2. Genere de manera más eficiente en [!DNL Marketo Engage] a largo plazo.
3. Mantenga el estado y la higiene de su instancia en adelante para evitar que dedique horas a explorar correos electrónicos, [pista de auditoría](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html) y [registro de actividad](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) para obtener contexto.
4. Ahorre tiempo al transferir conocimientos de [!DNL Marketo Engage] a un nuevo administrador de [!DNL Marketo Engage] si su equipo experimenta algún cambio.

## [!DNL Marketo Engage] guía de gobernanza 101

Una guía de gobernanza sirve como fuente fiable para la configuración de la instancia y los requisitos de diseño del sistema. La información clave que se recomienda incluir en este documento es:

* Estructuras de programa/carpeta
* Permiso de usuario y función
* Límites de comunicación
* Normas de gobernanza
* Formación interna del usuario antes de concederle acceso a la plataforma

## Cómo desarrollar y mantener una guía de gobernanza para su instancia de [!DNL Marketo Engage]

### Paso 1: Identifique el estado actual de la guía y documentación de gobernanza

* **No puedo encontrar ninguna documentación para mi instancia heredada:** Si recientemente inició una función nueva y no puede encontrar ninguna documentación para su instancia heredada, **vaya al paso 2** y comience con una plantilla descargable que proporcionamos.
* **Tengo documentación en el archivo:** ¡Felicitaciones, es una buena señal! Asegúrese de revisar su relevancia para ver cuándo se realiza el último cambio. Si los integrantes del equipo no la mantienen activamente, se recomienda actualizarla e informar a los usuarios internos sobre cómo mantenerla actualizada.

### Paso 2: Identificar los elementos que se incluirán en la documentación de [!DNL Marketo Engage] y [!DNL Changelogs]

El formato varía de una plataforma basada en la nube a un documento compartido. Puede diseñar el formato que se adapte a las necesidades de su organización. [Aquí tiene una sencilla documentación y una sencilla plantilla de excel changelog](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx) que cubre los elementos importantes con los que puede empezar. Estos incluyen:

* Documentación
   * Nombre de plantilla de programa
   * Canal
   * Fecha de creación
   * Creado por
   * Finalidad del programa
   * Estado
   * Vínculo a plantilla de programa
   * Nota
* Changelog
   * Nombre de plantilla de programa
   * Fecha del cambio
   * Actualizado por
   * Propósito de la actualización
   * Experiencia antes del cambio (incluir vínculos/capturas de pantalla)
   * Experiencia tras el cambio (incluir vínculos/capturas de pantalla)
   * URL del programa

### Paso 3: Identificar y documentar el estado actual de los programas operativos primarios

Comience por identificar los programas operativos clave con impactos en el nivel de suscripción. Algunos ejemplos son Campañas de administración de datos, Ciclo de vida del posible cliente, Puntuación de posibles clientes, Sincronización de [!DNL CRM] y Capacidad de entrega.

Para cada programa operativo identificado, documente su estado actual. Esto incluye detalles sobre el propósito del programa, la configuración, las campañas inteligentes asociadas y la integración con otras herramientas (si corresponde).

### Paso 4: Aplicar mantenimiento de [!DNL Changelog]

El siguiente paso es establecer una directiva de gobernanza estricta para la instancia de [!DNL Marketo Engage] que requiera el mantenimiento de [!DNL Changelog]. Esta política garantiza que cualquier actualización realizada en los programas operativos en toda la instancia esté documentada exhaustivamente.

Informe a su equipo de la importancia de estos documentos y de cómo acceder a ellos y actualizarlos correctamente. Podría resultar útil asignar responsabilidades para mantener el registro de cambios, por lo que algunos miembros o administradores designados del equipo de operaciones de marketing registran los cambios de forma coherente y proporcionan firmas.

### Paso 5: Centralización de la documentación

Establezca una ubicación central o un repositorio para almacenar toda la documentación relacionada con su instancia de [!DNL Marketo Engage]. Podría ser una unidad compartida, una carpeta dedicada o un sistema basado en la nube.

### Paso 6: Revisión y actualización periódicas

Programe revisiones periódicas de la documentación para asegurarse de que es precisa y está actualizada. Se puede pasar por alto fácilmente durante las horas de mayor afluencia. Configure recordatorios de forma proactiva en el calendario para asegurarse de que su equipo realiza actualizaciones con regularidad y reflejen los cambios o las optimizaciones en los programas operativos.

## ¿Qué sigue?

Empiece descargando esta [plantilla simple](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx).

Siga los pasos anteriores para desarrollar la guía y la documentación de gobernanza. A medida que avance en el proceso, tenga en cuenta las siguientes reglas:

**Actualice la documentación existente:**
Es crucial mantener la documentación actualizada. Si no se ha modificado en los últimos 3 años, dedique tiempo a revisar la documentación a medida que audite la instancia.

**Compartir y entrenar:**
Comparta su documentación y [!DNL changelog] con los integrantes relevantes del equipo y edúquelos sobre cómo actualizar estos registros.

**Revisión periódica:** programar con antelación el tiempo necesario para revisarlas y mantenerlas durante todo el año, a fin de incluir cambios, optimizaciones o ajustes nuevos a medida que se produzcan.

El mantenimiento de una documentación completa y actualizada para la instancia de Marketo Engage le ahorrará tiempo y esfuerzo a largo plazo y le facilitará una administración eficaz de instancias.

### Autores

**Nick Hajdin**
[!DNL Adobe Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**Amy Chiu**
*Administrador de marketing de adopción y retención, Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
