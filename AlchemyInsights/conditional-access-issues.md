---
title: Problemas de acceso condicional
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013980"
---
# <a name="conditional-access-issues"></a>Problemas de acceso condicional

**Resolver problemas mediante el diagnóstico de inicio de sesión**

Puede averiguar rápidamente qué ha ocurrido o diagnosticar problemas relacionados con el inicio de sesión del usuario mediante el diagnóstico [de inicio de sesión:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Inicie el diagnóstico de inicio de sesión.
1. Busque el evento que se va a analizar especificando los detalles que tiene sobre el usuario, la aplicación, la hora de inicio de sesión, el identificador de solicitud o el identificador de correlación.
1. Revise los resultados de diagnóstico que muestran los detalles de lo que ha ocurrido y las acciones que puede realizar para realizar cambios (si es necesario).

**Pasos para solucionar problemas de un inicio de sesión** 

1. Vaya a la página de inicio de sesión de Azure AD.
1. Filtra los inicios de sesión por usuario, intervalo de tiempo, aplicación, estado, aplicación cliente, entre otros.
1. Seleccione un evento de inicio de sesión y vea la pestaña Acceso condicional para ver qué directivas se evaluaron.
1. Haga clic en la fila de una directiva para ver los detalles de la directiva y comprender por qué se aplicó.

**Herramientas para solucionar problemas de una directiva de acceso condicional**

- El modo de solo informe le permite evaluar una directiva sin afectar a los usuarios.
- La herramienta what-if le permite simular eventos de inicio de sesión y ver qué directivas se aplican.
- La información y el libro de informes muestran el impacto en tiempo real de cada directiva.

**Directivas de protección de línea base**

Las directivas de protección de línea base han quedado en desuso. Ya no se aplican y pronto se quitarán de Azure Portal. Se recomienda habilitar los [valores predeterminados de seguridad.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Para obtener más información sobre el acceso condicional, vea:

[Procedimientos recomendados para el acceso condicional en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condiciones en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controles en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Ubicaciones en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
