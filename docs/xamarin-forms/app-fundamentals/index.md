---
title: Principios de la aplicación de Xamarin.Forms
description: Exploración de los fundamentos de desarrollo de aplicaciones de Xamarin.Forms, incluidos todos los conceptos principales necesarios, a través de toques finales, como la localización y accesibilidad.
ms.prod: xamarin
ms.assetid: 7B516BBC-F7E1-4387-9779-7754E2E69723
ms.technology: xamarin-forms
author: davidbritch
ms.author: dabritch
ms.date: 02/28/2017
ms.openlocfilehash: 515dbd2683619cfcfb7a6c8ecac6bc147265ef7d
ms.sourcegitcommit: 6e955f6851794d58334d41f7a550d93a47e834d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/12/2018
ms.locfileid: "38995617"
---
# <a name="xamarinforms-application-fundamentals"></a>Principios de la aplicación de Xamarin.Forms

## <a name="accessibilityaccessibilityindexmd"></a>[Accesibilidad](accessibility/index.md)

Sugerencias para incorporar características accesibles (por ejemplo, la compatibilidad con herramientas de lectura de pantalla) con Xamarin.Forms.

## <a name="app-classapplication-classmd"></a>[Clase de aplicación](application-class.md)

La clase `Application` es el punto de partida de Xamarin.Forms: todas las aplicaciones deben implementar una subclase `App`para establecer la página inicial. También proporciona la colección `Properties` para el almacenamiento simple de datos. Se puede definir en C# o XAML.

## <a name="app-lifecycleapp-lifecyclemd"></a>[Ciclo de vida de la aplicación](app-lifecycle.md)

Los métodos `OnStart`, `OnSleep` y `OnResume` de la clase `Application`, así como los eventos de navegación modal, le permiten controlar los eventos de ciclo de vida de las aplicaciones con código personalizado.

## <a name="behaviorsbehaviorsindexmd"></a>[Comportamientos](behaviors/index.md)

Los controles de interfaz de usuario se pueden ampliar fácilmente sin subclases mediante comportamientos para agregar funcionalidad.

## <a name="custom-rendererscustom-rendererindexmd"></a>[Representadores personalizados](custom-renderer/index.md)

Los representadores personalizados permiten a los desarrolladores "invalidar" la representación predeterminada de los controles de Xamarin.Forms para personalizar su apariencia y comportamiento en cada plataforma (mediante SDK nativos si quiere).

## <a name="data-bindingdata-bindingindexmd"></a>[Enlace de datos](data-binding/index.md)

El enlace de datos vincula las propiedades de dos objetos, de forma que permite que los cambios en una propiedad se reflejen automáticamente en la otra propiedad. El enlace de datos es una parte integral de la arquitectura de aplicación Model-View-ViewModel ([MVVM](~/xamarin-forms/enterprise-application-patterns/mvvm.md)).

## <a name="dependency-servicedependency-serviceindexmd"></a>[Servicio de dependencia](dependency-service/index.md)

`DependencyService` proporciona un localizador simple para que pueda programar en interfaces de su código compartido y proporcionar implementaciones específicas de la plataforma que se resuelven automáticamente, de forma que es fácil hacer referencia a la funcionalidad específica de la plataforma en Xamarin.Forms.

## <a name="effectseffectsindexmd"></a>[Efectos](effects/index.md)

Los efectos permiten personalizar los controles nativos de cada plataforma y se suelen usar para pequeños cambios de estilo.

## <a name="filesfilesmd"></a>[Archivos](files.md)

Archivo de control con Xamarin.Forms puede lograrse mediante código en una biblioteca .NET Standard, o mediante el uso de recursos incrustados.

## <a name="gesturesgesturesindexmd"></a>[Gestos](gestures/index.md)

La clase [`GestureRecognizer`](xref:Xamarin.Forms.GestureRecognizer) de Xamarin.Forms admite gestos de tocar, reducir y movimiento panorámico en controles de interfaz de usuario.

## <a name="localizationlocalizationindexmd"></a>[Localización](localization/index.md)

El marco de trabajo de localización integrada de .NET puede utilizarse para generar aplicaciones multilingües multiplataforma con Xamarin.Forms.

## <a name="local-databasesdatabasesmd"></a>[Bases de datos locales](databases.md)

Xamarin.Forms es compatible con aplicaciones basadas en la base de datos con el motor de base de datos de SQLite, lo que permite cargar y guardar los objetos en código compartido.

## <a name="messaging-centermessaging-centermd"></a>[Centro de mensajería](messaging-center.md)

Xamarin.Forms `MessagingCenter` permite ver los modelos y otros componentes se comuniquen sin tener que saber nada acerca de sí además de un contrato de mensaje simple.

## <a name="navigationnavigationindexmd"></a>[Navegación](navigation/index.md)

Xamarin.Forms proporciona una serie de experiencias de navegación de página diferentes, en función del tipo `Page` que se use.

## <a name="templatestemplatesindexmd"></a>[Templates](templates/index.md) (Plantillas [C++])

Las plantillas de control proporcionan la capacidad de aplicar y volver a aplicar fácilmente un tema a las páginas de aplicación en tiempo de ejecución, mientras que las plantillas de datos proporcionan la capacidad de definir la presentación de datos en controles compatibles.

## <a name="triggerstriggersmd"></a>[Desencadenadores](triggers.md)

Actualice los controles al responder a cambios de las propiedades y eventos en XAML.


## <a name="related-links"></a>Vínculos relacionados

- [Introducción a Xamarin.Forms](~/xamarin-forms/get-started/introduction-to-xamarin-forms.md)
