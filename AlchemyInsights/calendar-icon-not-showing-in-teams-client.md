---
title: El icono de calendario no se muestra en el cliente de Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819970"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="f1efc-102">El icono de calendario no se muestra en el cliente de Teams</span><span class="sxs-lookup"><span data-stu-id="f1efc-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="f1efc-103">La pestaña Calendario de Teams requiere el acceso a un buzón de Exchange a través de servicios Web de Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1efc-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="f1efc-104">El buzón de Exchange puede ser en línea o local.</span><span class="sxs-lookup"><span data-stu-id="f1efc-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="f1efc-105">En el caso de los usuarios en línea que no vean la pestaña Calendario, asegúrese de que [tengan licencia para un buzón de Exchange Online y que el buzón esté habilitado](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="f1efc-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="f1efc-106">Si el usuario tiene un buzón válido en Exchange Online pero aún no puede ver la pestaña Calendario, es posible que esté experimentando un problema de red.</span><span class="sxs-lookup"><span data-stu-id="f1efc-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="f1efc-107">Use el [analizador de conectividad remota de Microsoft](https://testconnectivity.microsoft.com/) y ejecute las **pruebas de conectividad de servicios Web de Microsoft Exchange** para el usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="f1efc-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="f1efc-108">Por último, compruebe las [directivas de configuración de aplicación para aplicaciones de Teams](https://admin.teams.microsoft.com/policies/app-setup) para asegurarse de que la aplicación de Calendario no se haya quitado de la directiva que se ha aplicado al usuario (lo más probable es que sea **Global (predeterminada para toda la organización)**.</span><span class="sxs-lookup"><span data-stu-id="f1efc-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="f1efc-109">Si sus usuarios están alojados en un entorno local, debe confirmar que la configuración híbrida es correcta.</span><span class="sxs-lookup"><span data-stu-id="f1efc-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="f1efc-110">Use el [Asistente para la configuración híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar el problema.</span><span class="sxs-lookup"><span data-stu-id="f1efc-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="f1efc-111">Tenga en cuenta que [Teams requiere Exchange 2016 CU3 o una versión superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="f1efc-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
