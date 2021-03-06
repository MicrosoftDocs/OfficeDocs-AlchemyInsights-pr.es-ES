---
title: No funciona el uso compartido con usuarios externos
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691592"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Solucionar problemas de uso compartido de contenido de SharePoint con usuarios externos

Asegúrese de que el uso compartido externo está activado para su organización:
  
1. Vaya a la [ &amp; Página complementos de servicios en el centro de administración de Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)y haga clic en **sitios**.
    
2. Asegúrese de que la configuración esté activada como "ON". Si se selecciona "solo usuarios externos existentes", asegúrese de que el usuario externo aparece en el centro de administración de Microsoft 365.
    
Asegúrese de que el uso compartido externo esté activado para el sitio. Para una colección de sitios clásica:
  
1. En el panel izquierdo del nuevo centro de administración de SharePoint, haga clic en **sitios**.
    
2. Seleccione el sitio o los sitios y, en la cinta de opciones, haga clic en **compartir**.
    
Para un sitio de grupo que pertenece a un grupo de Microsoft 365 o a un sitio de comunicación:
  
- Estos nuevos tipos de sitio tienen la misma configuración de uso compartido que la configuración de toda la organización, a menos que la configuración de toda la organización permita compartir archivos mediante vínculos que no requieran el inicio de sesión. En este caso, los sitios permiten el uso compartido con usuarios externos nuevos y existentes que inician sesión. Para cambiar la configuración de sitios específicos, use el nuevo centro de administración de SharePoint o PowerShell. [Más información](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> La configuración de uso compartido externo de cualquier sitio puede ser más restrictiva que la configuración de toda la organización, pero no más permisiva que la configuración de toda la organización. 
  

