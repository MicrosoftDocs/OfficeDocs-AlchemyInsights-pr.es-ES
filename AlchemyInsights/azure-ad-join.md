---
title: Unión a Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403832"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="dc44d-102">Unión a Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="dc44d-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="dc44d-103">Si configura los registros de dispositivos por primera vez, asegúrese de que ha revisado Introducción a la administración de dispositivos en [Azure Active Directory](/azure/active-directory/devices/overview) que le guiará sobre cómo obtener dispositivos bajo el control de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc44d-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="dc44d-104">Si vas a registrar dispositivos en Azure AD directamente e inscribirlos en Intune, deberás asegurarte de haber configurado [Intune](/mem/intune/enrollment/device-enrollment) y tener las licencias [en](/mem/intune/fundamentals/licenses-assign) primer lugar.</span><span class="sxs-lookup"><span data-stu-id="dc44d-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="dc44d-105">Asegúrese de que está autorizado a realizar operaciones en Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc44d-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="dc44d-106">Solo un administrador global de Azure AD puede administrar la configuración de los registros de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dc44d-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="dc44d-107">Para realizar la implementación de unirse a Azure AD, vea [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="dc44d-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="dc44d-108">Para obtener más información sobre cómo resolver problemas comunes con la unión a Azure AD, consulta Preguntas más frecuentes sobre la unión a [Azure Ad](/azure/active-directory/devices/faq) y para dispositivos profesionales de Windows 10, consulta No se puede unir la máquina de [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)a Azure AD - Necesidad de actualizar a - Microsoft Community .</span><span class="sxs-lookup"><span data-stu-id="dc44d-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>