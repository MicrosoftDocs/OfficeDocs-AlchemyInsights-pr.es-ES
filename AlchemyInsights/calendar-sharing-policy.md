---
title: Directiva de uso compartido de calendario 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684247"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Error de directiva al compartir un calendario

1. Realice una de las acciones siguientes, según corresponda a su situación:
    - Conéctese a Exchange online mediante PowerShell remoto. Para obtener más información, vea [conectarse a Exchange online mediante PowerShell remoto](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - En el servidor local, abra el shell de administración de Exchange.
2. Determine la Directiva de uso compartido que está asignada al usuario. Para ello, ejecute el siguiente comando y observe la Directiva devuelta:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Actualice la Directiva de uso compartido para el usuario. Para ello, siga estos pasos:
    - Abra el Centro de administración de Exchange.
    - Haga clic en **organización**y, a continuación, haga doble clic en la directiva asignada al usuario bajo **uso compartido individual**. Esta es la Directiva que se ha devuelto en el paso 2.
    - En la página regla de uso compartido, seleccione el nivel de uso compartido del calendario que desea permitir en **Especifique qué información desea compartir**; Haga clic en **Guardar**.

Para obtener más información, vea: ["la Directiva no permite conceder permisos en este nivel a uno o más de los destinatarios" cuando el usuario intenta compartir el calendario](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
