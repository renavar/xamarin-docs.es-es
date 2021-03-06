---
title: Uso de SkiaSharp en Xamarin.Forms
description: SkiaSharp es un sistema de gráficos 2D para .NET y C# funciona con el motor de gráficos de Skia de código abierto que se usa habitualmente en productos de Google. Esta guía explica cómo usar SkiaSharp para gráficos 2D en las aplicaciones de Xamarin.Forms.
ms.prod: xamarin
ms.assetid: 2C348BEA-81DF-4794-8857-EB1DFF5E11DB
ms.technology: xamarin-forms
author: charlespetzold
ms.author: chape
ms.date: 09/11/2017
ms.openlocfilehash: bdc0603c6ae406adac42533e251106ccccf2cb7c
ms.sourcegitcommit: 7f2e44e6f628753e06a5fe2a3076fc2ec5baa081
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/18/2018
ms.locfileid: "39130951"
---
# <a name="using-skiasharp-in-xamarinforms"></a>Uso de SkiaSharp en Xamarin.Forms

_Uso SkiaSharp para gráficos 2D en las aplicaciones de Xamarin.Forms_

SkiaSharp es un sistema de gráficos 2D para .NET y C# funciona con el motor de gráficos de Skia de código abierto que se usa habitualmente en productos de Google. Puede usar SkiaSharp en sus aplicaciones de Xamarin.Forms para dibujar texto, mapas de bits y gráficos vectoriales en 2D. Consulte la [plano 2D](~/graphics-games/skiasharp/index.md) guía para obtener información general sobre la biblioteca de SkiaSharp y algunos otros tutoriales.

Esta guía se da por supuesto que está familiarizado con la programación de Xamarin.Forms.

> [!VIDEO https://channel9.msdn.com/Events/Xamarin/Xamarin-University-Presents-Webinar-Series/SkiaSharp-Graphics-for-XamarinForms/player]

**Seminario Web: SkiaSharp para Xamarin.Forms**

## <a name="skiasharp-preliminaries"></a>Pasos preliminares de SkiaSharp

SkiaSharp para Xamarin.Forms está empaquetado como un paquete de NuGet. Después de crear una solución de Xamarin.Forms en Visual Studio o Visual Studio para Mac, puede usar el Administrador de paquetes de NuGet para buscar el **SkiaSharp.Views.Forms** empaquetar y agregarlo a la solución. Si activa la **referencias** sección de cada proyecto después de agregar SkiaSharp, puede ver que varios **SkiaSharp** bibliotecas se han agregado a cada uno de los proyectos de la solución.

Si la aplicación de Xamarin.Forms tiene como destino iOS, use la página de propiedades de proyecto para cambiar el destino de implementación mínimo IOS 8.0.

En cualquier página de C# que utiliza SkiaSharp desea incluir un `using` la directiva para el [ `SkiaSharp` ](https://developer.xamarin.com/api/namespace/SkiaSharp/) espacio de nombres, que abarca todas las SkiaSharp clases, estructuras y enumeraciones que va a usar en los gráficos la programación. También conviene un `using` la directiva para el [ `SkiaSharp.Views.Forms` ](https://developer.xamarin.com/api/namespace/SkiaSharp.Views.Forms/) espacio de nombres para las clases específicas de Xamarin.Forms. Esto es una cantidad menor espacio de nombres, con la clase más importante que es [ `SKCanvasView` ](https://developer.xamarin.com/api/type/SkiaSharp.Views.Forms.SKCanvasView/). Esta clase se deriva de Xamarin.Forms `View` clase y hospede su salida gráfica de SkiaSharp.

> [!IMPORTANT]
> El `SkiaSharp.Views.Forms` espacio de nombres también contiene un `SKGLView` clase que derive de `View` pero usa OpenGL para representar gráficos. Para fines de simplicidad, esta guía restringe a sí mismo a `SKCanvasView`, pero al usar `SKGLView` en su lugar, es bastante similar.

## <a name="skiasharp-drawing-basicsbasicsindexmd"></a>[Conceptos básicos de dibujo de SkiaSharp](basics/index.md)

Algunas de las cifras más sencillas de gráficos que puede dibujar con SkiaSharp son círculos, elipses y rectángulos. Mostrar estas cifras, aprenderá acerca de las coordenadas de SkiaSharp, tamaños y colores.

## <a name="skiasharp-lines-and-pathspathsindexmd"></a>[Trazados y líneas de SkiaSharp](paths/index.md)

Una ruta de acceso de gráficos es una serie de líneas rectas conectadas y curvas. Se trazan las rutas de acceso, rellenado, o ambos. En este tema abarca muchos aspectos del dibujo de líneas, incluidos los extremos de trazo y uniones y guiones y las líneas de puntos, pero no permite las geometrías de curva.

## <a name="skiasharp-transformstransformsindexmd"></a>[Transformaciones de SkiaSharp](transforms/index.md)

Las transformaciones permiten que los objetos gráficos uniformemente traducido, escalar, girar, o sesgar. En este artículo también muestra cómo puede utilizar una matriz de transformación de 3 por 3 estándar para crear transformaciones no afines y aplicar transformaciones a rutas de acceso.

## <a name="skiasharp-curves-and-pathscurvesindexmd"></a>[Trazados y curvas de SkiaSharp](curves/index.md)

La exploración de las rutas de acceso se continúa con la adición de curvas para los objetos de una ruta de acceso y aprovechando otras características eficaces de la ruta de acceso. Verá cómo puede especificar una ruta de acceso completa en una cadena de texto conciso, cómo usar los efectos de la ruta de acceso y cómo profundizar en los aspectos internos de ruta de acceso.

## <a name="skiasharp-bitmapsbitmapsindexmd"></a>[Mapas de bits de SkiaSharp](bitmaps/index.md)

Los mapas de bits son matrices rectangulares de bits que corresponden a los píxeles de un dispositivo de pantalla. Esta serie de artículos muestra cómo cargar, guardar, mostrar, crear, dibuje en, animar y tener acceso a los bits de SkiaSharp mapas de bits.

## <a name="related-links"></a>Vínculos relacionados

- [API de SkiaSharp](https://developer.xamarin.com/api/root/SkiaSharp/)
- [SkiaSharpFormsDemos (ejemplo)](https://developer.xamarin.com/samples/xamarin-forms/SkiaSharpForms/Demos/)
- [SkiaSharp con Xamarin.Forms seminario Web (vídeo)](https://channel9.msdn.com/Events/Xamarin/Xamarin-University-Presents-Webinar-Series/SkiaSharp-Graphics-for-XamarinForms)
