---
title: Implementación de complementos para Aplicaciones Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233551"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="3a1c3-102">Implementación de complementos para Aplicaciones Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3a1c3-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="3a1c3-103">La implementación centralizada es la forma recomendada para implementar Office complementos para usuarios y grupos de la organización.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="3a1c3-104">Para implementar complementos, siga los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="3a1c3-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="3a1c3-105">**Nota:** Para instalar complementos para Office como un usuario individual, vea [Ver,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)administrar e instalar complementos en Office programas .</span><span class="sxs-lookup"><span data-stu-id="3a1c3-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="3a1c3-106">Además, asegúrate de que la adquisición individual de Office complementos de la Tienda está habilitada.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="3a1c3-107">Para obtener más información, vea [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="3a1c3-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="3a1c3-108">Asegúrese de que el entorno cumple los requisitos para la implementación de complementos mediante la implementación centralizada.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="3a1c3-109">Para obtener más información, vea [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="3a1c3-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="3a1c3-110">Ve a **Configuración** aplicaciones integradas Obtener aplicaciones en  >    >   el centro Microsoft 365 administración para implementar complementos.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="3a1c3-111">Notas:</span><span class="sxs-lookup"><span data-stu-id="3a1c3-111">Notes:</span></span> 

- <span data-ttu-id="3a1c3-112">Las aplicaciones integradas requieren que el administrador tenga permisos de administrador global Exchange administrador.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="3a1c3-113">Al implementar complementos para varios usuarios, se recomienda realizar asignaciones mediante grupos en lugar de usuarios individuales.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="3a1c3-114">Para obtener más información, vea [Consideraciones al asignar un complemento a usuarios y grupos](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="3a1c3-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="3a1c3-115">La implementación centralizada no admite usuarios de grupos anidados o grupos que tienen grupos primarios.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="3a1c3-116">Para obtener más información, vea [Asignaciones de usuarios y grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="3a1c3-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="3a1c3-117">Asegúrese de que Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') esté habilitado para que los usuarios inicien sesión.</span><span class="sxs-lookup"><span data-stu-id="3a1c3-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="3a1c3-118">Para obtener más información, consulta [Configurar las propiedades de la aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="3a1c3-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="3a1c3-119">Si tiene problemas para implementar complementos mediante aplicaciones integradas, intente implementar mediante [complementos](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="3a1c3-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="3a1c3-120">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="3a1c3-120">For more information, see:</span></span>

<span data-ttu-id="3a1c3-121">[Implementar complementos en el Centro de administración](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrar complementos en el Centro de administración](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Usar los cmdlets de PowerShell de implementación centralizada para administrar complementos](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office complementos mediante](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) la implementación centralizada a través del Centro Microsoft 365 administración 
 [Solución de problemas: el usuario no ve complementos](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Solucionar errores de usuario con Office complementos](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="3a1c3-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>