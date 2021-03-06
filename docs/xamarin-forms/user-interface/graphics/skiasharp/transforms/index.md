---
title: Transformaciones de SkiaSharp
description: Este artículo explora las transformaciones para mostrar gráficos de SkiaSharp en Xamarin.Forms y esto muestra con código de ejemplo.
ms.prod: xamarin
ms.technology: xamarin-forms
ms.assetid: E9BE322E-ECB3-4395-AFE4-4474A0F25551
author: charlespetzold
ms.author: chape
ms.date: 03/10/2017
ms.openlocfilehash: e2f83e3de574d11052b5301f1832988b7f4166bf
ms.sourcegitcommit: 6e955f6851794d58334d41f7a550d93a47e834d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/12/2018
ms.locfileid: "38998652"
---
# <a name="skiasharp-transforms"></a>Transformaciones de SkiaSharp

_Obtenga información acerca de las transformaciones para mostrar gráficos de SkiaSharp_

SkiaSharp admite transformaciones tradicional de gráficos que se implementan como métodos de la [ `SKCanvas` ](https://developer.xamarin.com/api/type/SkiaSharp.SKCanvas/) objeto. Matemáticamente, transformaciones alteran las coordenadas y los tamaños que se especifican en `SKCanvas` funciones de dibujo se representan los objetos gráficos. Las transformaciones a menudo resultan prácticos para dibujar gráficos repetitivos o para ver la animación. Algunas técnicas &mdash; como girar texto o mapas de bits &mdash; no son posibles sin el uso de transformaciones.

Transformaciones de SkiaSharp admiten las siguientes operaciones:

- *Traducir* a coordenadas de desplazamiento de una ubicación a otra
- *Escala* para aumentar o disminuir las coordenadas y tamaños
- *Girar* para girar las coordenadas en torno a un punto
- *Sesgar* desplazar las coordenadas horizontal o verticalmente para que un rectángulo se convierte en un paralelogramo

Estos se conocen como *afín* transforma. Transformaciones afines siempre conservar líneas paralelas y nunca producen una coordenada o tamaño para convertirse en infinito. Un cuadrado nunca se transforma en un paralelogramo distinto, y un círculo nunca se transforma en algo distinto de una elipse.

SkiaSharp también admite transformaciones no afines (también denominada *proyectiva* o *perspectiva* transforma) basándose en una matriz de transformación de 3 por 3 estándar. Una transformación no afín permite un cuadrado se transforman en cualquier cuadrilátero convexo (una cuatro lados figura con todos los ángulos interior inferior a 180 grados). Transformaciones no afines pueden provocar coordenadas o tamaños para convertirse en infinito, pero son vitales para los efectos 3D.

## <a name="differences-between-skiasharp-and-xamarinforms-transforms"></a>Diferencias entre las transformaciones de Xamarin.Forms y SkiaSharp

Xamarin.Forms también admite las transformaciones que son similares a los de SkiaSharp. Xamarin.Forms [ `VisualElement` ](xref:Xamarin.Forms.VisualElement) clase define las siguientes propiedades de transformación:

- `TranslationX` y `TranslationY`
- `Scale`
- `Rotation`, `RotationX` y `RotationY`

El `RotationX` y `RotationY` propiedades son las transformaciones de perspectiva que creación efectos casi 3D.

Hay varias diferencias fundamentales entre las transformaciones de SkiaSharp y transformaciones de Xamarin.Forms:

La primera diferencia es que las transformaciones de SkiaSharp se aplican a toda la `SKCanvas` objeto mientras se aplican las transformaciones de Xamarin.Forms a persona `VisualElement` derivados. (Puede aplicar las transformaciones de Xamarin.Forms para la `SKCanvasView` objeto, porque `SKCanvasView` deriva `VisualElement`, pero dentro de ese `SKCanvasView`, se aplican las transformaciones SkiaSkarp.)

Las transformaciones de SkiaSharp son relativas a la esquina superior izquierda de la `SKCanvas` mientras Xamarin.Forms transformaciones son relativas a la esquina superior izquierda de la `VisualElement` al que se aplican. Esta diferencia es importante al aplicar la escala y giro transforma porque estas transformaciones son siempre con respecto a un momento determinado.

La realidad la gran diferencia es que son transformaciones de SKiaSharp *métodos* mientras que las transformaciones de Xamarin.Forms son *propiedades*. Se trata de una diferencia semántica más allá de la diferencia sintáctica: transformaciones de SkiaSharp realizan una operación, mientras que las transformaciones de Xamarin.Forms establecen un estado. Transformaciones de SkiaSharp se aplican a objetos gráficos dibujados a continuación, pero no a los objetos de gráficos que se dibujan antes de aplicar la transformación. En cambio, una transformación de Xamarin.Forms se aplica a un elemento previamente representado tan pronto como se establece la propiedad. Transformaciones de SkiaSharp son acumulativas, como los métodos se llaman; Transformaciones de Xamarin.Forms se sustituyen cuando se establece la propiedad con otro valor.

Todos los programas de ejemplo en esta sección aparecen bajo el encabezado **transforma** en la página principal de la [ **SkiaSharpFormsDemos** ](https://developer.xamarin.com/samples/xamarin-forms/SkiaSharpForms/Demos/) programa y en el [ **Transforma** ](https://github.com/xamarin/xamarin-forms-samples/tree/master/SkiaSharpForms/Demos/Demos/SkiaSharpFormsDemos/Transforms) carpeta de la solución.

## <a name="the-translate-transformtranslatemd"></a>[Transformación de traslación](translate.md)

Obtenga información sobre cómo usar la transformación de traslación de SkiaSharp gráficos de desplazamiento.

## <a name="the-scale-transformscalemd"></a>[Transformación de escala](scale.md)

Descubra la transformación de escala de SkiaSharp para el escalado de objetos para distintos tamaños.

## <a name="the-rotate-transformrotatemd"></a>[Transformación de rotación](rotate.md)

Explore los efectos y animaciones posibles con la transformación de giro de SkiaSharp.

## <a name="the-skew-transformskewmd"></a>[Transformación de sesgo](skew.md)

Vea cómo la transformación de sesgo puede crear objetos gráficos superpuestos de SkiaSharp.

## <a name="matrix-transformsmatrixmd"></a>[Transformaciones de matriz](matrix.md)

Profundice en las transformaciones de SkiaSharp con la matriz de transformación versátil.

## <a name="touch-manipulationstouchmd"></a>[Manipulaciones táctiles](touch.md)

Matriz de uso se transforma para implementar las manipulaciones táctiles para arrastrar, escala y giro.

## <a name="non-affine-transformsnon-affinemd"></a>[Transformaciones no afines](non-affine.md)

Vaya más allá de la oridinary con efectos de la transformación no afín.

## <a name="3d-rotation3d-rotationmd"></a>[Giro 3D](3d-rotation.md)

Utilizar las transformaciones no afines girar objetos 2D en el espacio 3D.


## <a name="related-links"></a>Vínculos relacionados

- [API de SkiaSharp](https://developer.xamarin.com/api/root/SkiaSharp/)
- [SkiaSharpFormsDemos (ejemplo)](https://developer.xamarin.com/samples/xamarin-forms/SkiaSharpForms/Demos/)
