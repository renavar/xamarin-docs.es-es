---
title: 'Xamarin.Essentials: Portapapeles'
description: Este documento describe la clase del Portapapeles en Xamarin.Essentials, que le permite copiar y pegar texto en el Portapapeles del sistema entre aplicaciones.
ms.assetid: C52AE99A-0FB3-425D-9106-3DA5777FEFA0
author: jamesmontemagno
ms.author: jamont
ms.date: 05/04/2018
ms.openlocfilehash: 41b15b480fa23bd49667b68e904043e4f1a95732
ms.sourcegitcommit: 632955f8cdb80712abd8dcc30e046cb9c435b922
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2018
ms.locfileid: "38842620"
---
# <a name="xamarinessentials-clipboard"></a>Xamarin.Essentials: Portapapeles

![La versión preliminar de NuGet](~/media/shared/pre-release.png)

El **Portapapeles** clase le permite copiar y pegar texto en el Portapapeles del sistema entre aplicaciones.

## <a name="using-clipboard"></a>Usar el Portapapeles

Agregue una referencia a Xamarin.Essentials en su clase:

```csharp
using Xamarin.Essentials;
```

Para comprobar si el **Portapapeles** tiene actualmente listo para pegar texto:

```csharp
var hasText = Clipboard.HasText;
```

Para establecer el texto en el **Portapapeles**:

```csharp
Clipboard.SetText("Hello World");
```

Leer texto desde el **Portapapeles**:

```csharp
var text = await Clipboard.GetTextAsync();
```

## <a name="api"></a>API

- [Código fuente de Portapapeles](https://github.com/xamarin/Essentials/tree/master/Xamarin.Essentials/Clipboard)
- [Documentación de API de Portapapeles](xref:Xamarin.Essentials.Clipboard)
