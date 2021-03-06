---
title: Ensamblados disponibles
description: Este documento enumera los ensamblados disponibles para su uso en Xamarin.iOS, Xamarin.Android y Xamarin.Mac. También incluye vínculos a documentación sobre bibliotecas de .NET Standard y bibliotecas de clases portables.
ms.prod: xamarin
ms.assetid: AEF4ED0E-391F-4FA4-9F18-842BC24C272D
author: asb3993
ms.author: amburns
ms.date: 03/13/2018
ms.openlocfilehash: d005d6c5e1dcfe7e9bcff44b308cea0ce7ab73e9
ms.sourcegitcommit: 6e955f6851794d58334d41f7a550d93a47e834d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/12/2018
ms.locfileid: "38998659"
---
# <a name="available-assemblies"></a>Ensamblados disponibles

Xamarin.iOS, Xamarin.Android y Xamarin.Mac todos se distribuyen con más de una docena de ensamblados. Como Silverlight es un subconjunto de los ensamblados de .NET de escritorio extendido, las plataformas Xamarin también es un subconjunto de las distintas Silverlight y ensamblados de .NET de escritorio extendido.

Las plataformas de Xamarin no son ABI compatible con existentes de los ensamblados compilados para un perfil diferente. Debe volver a compilar el código fuente para generar ensamblados de destino es el perfil correcto (igual que es necesario volver a compilar el código fuente para tener como destino Silverlight y 3.5 de .NET por separado).

Se pueden compilar aplicaciones de Xamarin.Mac en tres modos: uno que usa Xamarin de curah perfil móvil, Xamarin.Mac .NET Framework 4.5 que permite tener como destino los ensamblados de escritorio completa existentes y uno compatible que usa la API de .NET se encuentra en un sistema de Mono instalación. Para obtener más información, consulte nuestra [plataformas de destino](~/mac/platform/target-framework.md) documentación.


## <a name="net-standard-libraries"></a>Bibliotecas estándar de .NET

Además de iOS, Android y Mac, enlaces, pueden consumir los proyectos de Xamarin [bibliotecas de .NET Standard](~/cross-platform/app-fundamentals/net-standard.md).

## <a name="portable-class-libraries"></a>Bibliotecas de clases portables
 
También pueden usar los proyectos de Xamarin [bibliotecas de clases portables de .NET](~/cross-platform/app-fundamentals/pcl.md), aunque esta tecnología está en desuso en favor de .NET Standard.

## <a name="supported-assemblies"></a>Ensamblados admitidos

> [!div class="mx-tdCol2BreakAll"]
> |Ensamblado|Compatibilidad con la API|Xamarin iOS|Xamarin Android|Mac de Xamarin|
> |--------|-----------------|-----------|---------------|-----------|
> |FSharp.Core.dll| |✓|✓|✓|
> |l18N.dll|Incluye CJK, Oriente, otros, es poco habitual, oeste|✓|✓|✓|
> |Microsoft.CSharp.dll| |✓|✓|✓|
> |Mono.CSharp.dll| |✓|✓|✓|
> |Mono.Data.Sqlite.dll|Proveedor de ADO.NET para SQLite; vea las limitaciones.|✓|✓|✓|
> |Mono.Data.Tds.dll|Compatibilidad de protocolo TDS; utilizado para [System.Data.SqlClient](xref:System.Data.SqlClient) soporte técnico en [System.Data](xref:System.Data).|✓|✓|✓|
> |Mono.Dynamic. &#8203;Interpreter.dll| |✓| | |
> |Mono.Security.dll|API criptográficas.|✓|✓|✓|
> |monotouch.dll|Este ensamblado contiene el enlace a la API CocoaTouch de C#. Esto solo está disponible en proyectos Classic de iOS.|✓| | |
> |MonoTouch. &#8203;1.dll del cuadro de diálogo| |✓| | |
> |MonoTouch. &#8203;NUnitLite.dll| |✓| | |
> |mscorlib.dll|[Silverlight](https://msdn.microsoft.com/library/cc838194(VS.95).aspx)|✓|✓|✓|
> |OpenTK-1.0.dll|El objeto de OpenGL/OpenAL orientada a servicios de API, ampliadas para proporcionar compatibilidad con dispositivos de iPhone.|✓|✓|✓|
> |System.dll|[Silverlight](https://msdn.microsoft.com/library/cc838194(VS.95).aspx), además de los tipos de los espacios de nombres siguientes:<br />System.Collections.Specialized<br />Sistema. &#8203;ComponentModel<br />System.ComponentModel.Design<br />System.Diagnostics<br />System.IO<br />System.IO.Compression<br />System.IO.Compression.FileSystem<br />System.Net<br />System.Net.Cache<br />System.Net.Mail<br />System.Net.Mime<br />System.Net. &#8203;NetworkInformation<br />System.Net.Security<br />System.Net.Sockets<br />System.Runtime. &#8203;InteropServices<br />System.Runtime.Versioning<br />System.Security. &#8203;AccessControl<br />System.Security.Authentication<br />System.Security. &#8203;Criptografía<br />System.Security.Permissions<br />System.Threading<br />System.Timers|✓|✓|✓|
> |Sistema. &#8203;ComponentModel. &#8203;Composition.dll| |✓|✓|✓|
> |System.&#8203;ComponentModel.&#8203;DataAnnotations.dll| |✓|✓|✓|
> |System.Core.dll|[Silverlight](https://msdn.microsoft.com/library/cc838194(VS.95).aspx)|✓|✓|✓|
> |System.Data.dll|[.NET 3.5](http://msdn.microsoft.com/library/ms229335.aspx) , con [alguna funcionalidad eliminado](~/ios/data-cloud/system.data.md).|✓|✓|✓|
> |System.Data. &#8203;Servicios. &#8203;Client.dll|Cliente de oData completa.|✓|✓|✓|
> |System.IO. &#8203;Compresión| |✓|✓|✓|
> |System.IO. &#8203;Compresión. &#8203;FileSystem| |✓|✓|✓|
> |System.Json.dll|[Silverlight](http://msdn.microsoft.com/library/cc838194(VS.95).aspx)|✓|✓|✓|
> |System.Net. &#8203;Http.dll| |✓|✓|✓|
> |Sistema. &#8203;Numerics.dll| |✓|✓|✓|
> |System.Runtime. &#8203;Serialization.dll|[Silverlight](http://msdn.microsoft.com/library/cc838194(VS.95).aspx)|✓|✓|✓|
> |Sistema. &#8203;ServiceModel.dll|Pila de WCF tal como está presente en [Silverlight](http://msdn.microsoft.com/library/cc838194(VS.95).aspx)|✓|✓|✓|
> |System.&#8203;ServiceModel.&#8203;Internals.dll| |✓|✓|✓|
> |Sistema. &#8203;ServiceModel. &#8203;Web.dll|[Silverlight](http://msdn.microsoft.com/library/cc838194(VS.95).aspx), además de los tipos de los espacios de nombres siguientes: <br />Sistema<br />System.ServiceModel.Channels<br />System.ServiceModel.Description<br />System.ServiceModel.Web|✓|✓|✓|
> |Sistema. &#8203;Transactions.dll|[.NET 3.5](http://msdn.microsoft.com/library/ms229335.aspx); forma parte de [System.Data](~/ios/data-cloud/system.data.md) admite.|✓|✓|✓|
> |System.Web. &#8203;Services.dll|Servicios Web básicos del perfil de .NET 3.5, con las características de servidor quitado.|✓|✓|✓|
> |Sistema. &#8203;Windows.dll| |✓|✓|✓|
> |Sistema. &#8203;Xml.dll|[.NET 3.5](http://msdn.microsoft.com/library/ms229335.aspx)|✓|✓|✓|
> |System.Xml. &#8203;Linq.dll|[.NET 3.5](http://msdn.microsoft.com/library/ms229335.aspx)|✓|✓|✓|
> |System.Xml.Serialization.dll| |✓|✓|✓|
> |Xamarin.iOS.dll|Este ensamblado contiene el enlace a la API CocoaTouch de C#. Esto solo se usa en proyectos de iOS unificado.|✓| | |
> |Java.Interop.dll| | |✓| |
> |Mono.Android.dll| | |✓| |
> |Mono.Android. &#8203;Export.dll| | |✓| |
> |Mono.Posix.dll| | |✓| |
> |System.&#8203;EnterpriseServices.dll| | |✓| |
> |Xamarin.Android. &#8203;NUnitLite.dll| | |✓| |
> |Mono.CompilerServices. &#8203;SymbolWriter.dll|Los programadores de compiladores.| | |✓|
> |Xamarin.Mac.dll| | | |✓|
> |Sistema. &#8203;Drawing.dll|System.Drawing API - API clásica solo. System.Drawing no se admite en la API unificada para Xamarin.Mac .NET 4.5 o plataformas móviles. Puede agregarse compatibilidad de System.Drawing para iOS y OS X mediante el [sysdrawing coregraphics](https://github.com/mono/sysdrawing-coregraphics) biblioteca|✓| |✓|
