---
title: Abrir con el explorador no funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694473"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir con el explorador no funciona

Si **abrir con el explorador** o **ver en el explorador de archivos** no funciona, asegúrese de que el servicio WebClient está configurado para **ejecutarse** siguiendo los pasos que se indican a continuación. Por ejemplo, puede tardar mucho tiempo en abrir una biblioteca de SharePoint o de OneDrive cuando el servicio no se está ejecutando. 
  
1. En el cuadro de búsqueda de Windows, escriba ejecutar, seleccione la aplicación de escritorio ejecutar, escriba Services. msc y, a continuación, seleccione **entrar**.
    
2. Desplácese hacia abajo hasta el servicio WebClient y Compruebe la columna **Estado** . Si el estado del servicio WebClient no se está **ejecutando**, haga doble clic en el servicio, haga clic en **iniciar**y, a continuación, haga clic en **Aceptar**. Habilite el servicio, si es necesario, seleccionando **manual** o **automático** en el cuadro **tipo de inicio** . 
    
> [!NOTE]
> Para solucionar problemas de apertura en el explorador de archivos, consulte [abrir en el explorador](https://go.microsoft.com/fwlink/?linkid=871665). Explore Sync como una alternativa mejor: [sincronizar archivos de SharePoint con el nuevo cliente de sincronización de OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

