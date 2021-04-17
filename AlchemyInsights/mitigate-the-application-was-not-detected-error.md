---
title: Solucionar el error No se detectó la aplicación
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836368"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Solucionar el error "No se detectó la aplicación"

El error de instalación de la aplicación, "no se detectó la aplicación después de completar la instalación correctamente", generado por Intune, puede producirse en todas las plataformas de SO principales (Windows, iOS y Android).

Entre los escenarios más comunes que generan este error se incluyen:

- Se ha actualizado la aplicación fuera de Intune (desde una tienda de aplicaciones de terceros) después de la implementación inicial. Por ejemplo, algunas aplicaciones, como Google Chrome, pueden realizar actualizaciones automáticas.
- Un usuario ha desinstalado la aplicación después de la instalación inicial.

Para mitigar este problema, primero realice una revisión de los dispositivos afectados para determinar el escenario en el que se produce el error.

- Si la aplicación se ha actualizado fuera de Intune, la implementación de la aplicación puede configurarse para ignorar la versión de la aplicación. Para ello, en **Configuración de la aplicación > Información de la aplicación,** establezca **Ignorar versión de la aplicación** en **Sí**.
- Al dirigirse al cliente, puede ser apropiado implementar la aplicación como "necesaria" y asegurarse de que se implemente la versión más reciente.
- Por otra parte, en la plataforma de iOS, es posible usar la función **autoupdate** asociada al programa de compras por volumen de Apple, que se puede configurar para que actualice automáticamente a nuevas versiones de las aplicaciones cuando estén disponibles.

Para más información sobre la solución de problemas de instalación de aplicaciones, vea [Solucionar problemas de instalación de aplicación](https://docs.microsoft.com/intune/troubleshoot-app-install).
