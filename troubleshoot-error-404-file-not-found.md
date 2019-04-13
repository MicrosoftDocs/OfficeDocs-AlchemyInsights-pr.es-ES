---
title: Solucionar el error 404, no se encontró el archivo
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 467feb3cb436a2e0135162657876e5c45d8d56bd
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747255"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="42e31-102">Solucionar el error 404, no se encontró el archivo</span><span class="sxs-lookup"><span data-stu-id="42e31-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="42e31-103">Se recibe un error 404 cuando los usuarios intentan tener acceso a un sitio o archivo en SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="42e31-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="42e31-104">Esto suele deberse a que un sitio o un archivo o grupo se cambian de nombre, se mueven o se eliminan.</span><span class="sxs-lookup"><span data-stu-id="42e31-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="42e31-105">Por ejemplo: los usuarios experimentarán un error 404 al intentar obtener acceso a la colección de sitios raíz y se ha eliminado.</span><span class="sxs-lookup"><span data-stu-id="42e31-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="42e31-106">Para resolver el error 404 para un sitio que ha cambiado de nombre, se ha movido o eliminado:</span><span class="sxs-lookup"><span data-stu-id="42e31-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="42e31-107">Para los sitios clásicos que existen en el centro de administración clásico, vea [restaurar una colección de sitios eliminada](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="42e31-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="42e31-108">Para los sitios modernos (comunicaciones, grupos conectados u otros sitios) que existen en el nuevo centro de administración de SharePoint, vea [ver y restaurar sitios eliminados en el nuevo centro de administración de SharePoint](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="42e31-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="42e31-109">Para resolver el error 404 para un archivo (u otro elemento) que se ha cambiado de nombre, se ha movido o eliminado:</span><span class="sxs-lookup"><span data-stu-id="42e31-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="42e31-110">Vaya al sitio de SharePoint o de OneDrive y vea la papelera de reciclaje desde el contenido del sitio.</span><span class="sxs-lookup"><span data-stu-id="42e31-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="42e31-111">Vea [Restaurar elementos en la papelera de reciclaje de un sitio de SharePoint](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="42e31-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="42e31-112">Si sigue sin poder encontrar el elemento, puede buscar en el registro de auditoría si el registro está habilitado consulte, [Busque en el registro de auditoría en el centro de seguridad de Office 365 _AMP_ cumplimiento](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span><span class="sxs-lookup"><span data-stu-id="42e31-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>