---
title: Configuración de directiva de reunión
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825460"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Administrar directivas de reuniones en Microsoft Teams

**Nota: Los cambios de directiva pueden tardar hasta 24 horas en tener efecto para los usuarios.** Es posible que no pueda realizar cambios en las directivas recién creadas inmediatamente; espere 4 horas e intente modificar una directiva recién creada de nuevo.

Las directivas de reunión se usan para controlar las características que están disponibles para los participantes de las reuniones programadas por los usuarios de la organización. Es posible que algunas características de directivas de reunión aún no se implementen en el Centro de administración de Teams (estas se etiquetan "próximamente" en la documentación). En este caso, o si recibe un error como "No podemos actualizar la directiva en este momento pero volver a intentarlo más adelante" en el Centro de administración de Microsoft Teams, se recomienda usar PowerShell para crear o modificar directivas de reunión de Teams. 

Para obtener más información acerca de las directivas de reunión, vea los siguientes recursos:

- Para obtener información sobre cómo crear directivas, realizar cambios y asignar usuarios a la directiva, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para realizar cambios de directiva con cmdlets de PowerShell, vea [Información general de PowerShell de Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Debe usar el módulo [de PowerShell de Skype Empresarial](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) para directivas de reuniones de Teams. 
    - Revise la [documentación de los cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obtener más información.

